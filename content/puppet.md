# Automation Tools 
- [Puppet](https://github.com/dial2vincent/lab/blob/master/content/puppet.md)
- [Puppet Sample Code](https://github.com/dial2vincent/lab/blob/master/content/puppet-sample-code.md)
# Puppet
puppet installation on Ubuntu 24.04 and Oracle 7.9

## Puppet Installation on Ubuntu
- Story: The instruction is to reinstall the puppet on Ubuntu 24.04 because I failed to test the puppet to request the cert multiple times.
  Finally, this reinstallation was successfully completed on the Ubuntu VM as a puppet master. 

### Step 1: Remove Puppet Server
 1. Stop Puppet Server Service
~~~
sudo systemctl stop puppetserver
sudo systemctl stop puppet
~~~
 2. Remove Puppet Package
`sudo apt-get purge -y puppetserver puppet-agent puppet `
 3. Remove Puppet Directory
~~~
sudo rm -rf /etc/puppetlabs
sudo rm -rf /opt/puppetlabs
sudo rm -rf /var/log/puppetlabs
sudo rm -rf /var/lib/puppetlabs
~~~
### Step 2: Reinstall Puppet Server and Agent
 1. Add Puppet Repository
~~~
wget https://apt.puppet.com/puppet8-release-focal.deb
sudo dpkg -i puppet8-release-focal.deb
sudo apt-get update
~~~
 2. Install Puppet Server and Agent
`sudo apt-get install -y puppetserver`
 3. Install Puppet Agent
`sudo apt-get install -y puppet-agent`
### Step 3: Configure Puppet Server
 1. Edit Puppet Configuration:
`sudo nano /etc/puppetlabs/puppet/puppet.conf`
 1.1 Ensure to add the followings
~~~
[main]
dns_alt_names = puppet,puppetmaster

[master]
certname = puppetmaster
~~~
 2. Set Java Memory Allocation
`sudo nano /etc/default/puppetserver`
 Modify the 'JAVA_ARGS'
~~~
JAVA_ARGS="-Xms2g -Xmx2g -XX:MaxPermSize=256m"
~~~
 4. Start Puppet Server
~~~
sudo systemctl start puppetserver
sudo systemctl enable puppetserver
~~~
### Step 4: Configure Puppet Agent
 1. Edit Puppet Agent Configuration:
`sudo nano /etc/puppetlabs/puppet/puppet.conf`
- Ensure to add the following:
~~~
[main]
server = puppetmaster
~~~
 2. Start Puppet Agent
~~~
sudo systemctl start puppet
sudo systemctl enable puppet
~~~
### Step 5: Test the setup
 1. Run Puppet Agent: on Agent
`sudo /opt/puppetlabs/bin/puppet agent --test --waitforcert 60`
 2. Sign Certificate on Puppet Master:
`sudo /opt/puppetlabs/bin/puppetserver ca sign --all`
 3. Run Puppet Agent again: On Agent

Completed to add installation on the Ubuntu

---

#### Sample manifests on your puppet master
- Location: /etc/puppetlabs/code/environments/production/manifests/site.pp
1. Create Manifests site.pp
~~~
node 'puppetmaster', 'puppetclient1', 'puppetclient2' {  # Replace 'agent-node-fqdn' with your Puppet agent's fully qualified domain name
  class { 'ntp':
    servers => ['0.pool.ntp.org', '1.pool.ntp.org'],
  }
}
~~~
2. Install NTP module
`sudo puppet module install puppetlabs-ntp`
3. Apply the manifest on the Puppet agent
   `sudo /opt/puppetlabs/bin/puppet agent --test`
4. Verify the set up
   `sudo systemctl status ntp`
To check the package installed:
~~~
dpkg -l | grep ntp  # On Debian/Ubuntu
rpm -qa | grep ntp  # On CentOS/RHEL
~~~
### Puppet Commands:
- `sudo /opt/puppetlabs/bin/puppetserver ca list --all` To find Puppet Clients from the Puppet Master
- `rm -r *` 현재 디렉터리의 파일과 하위 디렉터리 모두를 삭제한다. 사용할 때 주의해야 한다.
- `man sudo sudo` 명령 사용에 관련된 매뉴얼 문서를 보여준다.

