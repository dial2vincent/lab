# Automation Tools 
- [Puppet](https://github.com/dial2vincent/lab/blob/master/content/puppet.md)
- [Puppet Sample Code](https://github.com/dial2vincent/lab/blob/master/content/puppet-sample-code.md)

# Puppet Testing a sample manifest
- Story: 3 Oracle Linux virtual machines in the lab installed a Puppet server and two Puppet client virtual machines.
- Location: 
- Oracle Linux Puppet server (188): /etc/puppetlabs/code/environments/production/manifests
- Oracle Linux Puppet client 1 (78): /opt/puppetlabs/bin/puppet
- Oracle Linux Puppet client 2 (34): /opt/puppetlabs/bin/puppet

## Puppet Server 

### Steps: Create a sample puppet program and apply the file from a client machine.
 1. Create hello.pp on 
  `sudo nano  /etc/puppetlabs/code/environments/production/manifests/hello.pp`
 2. Add content below to the hello.pp:
~~~
node default {
  file { '/tmp/hello_world.txt':
    ensure  => 'file',
    content => "Hello, Puppet World!\n",
  }

# manage_user
   user { 'cloudlee':
     ensure     => 'present',
     managehome => true,
     home       => '/home/cloudlee',
     shell      => '/bin/bash',
  }

}
~~~

## Puppet Client
### Steps: Apply the manifest from a client machine.
 1. Log into the client machine (78) 
  `ssh root@puppetclient1`
 2. Request a catalog, compile, and apply catalog to the Puppet master
  `sudo /opt/puppetlabs/bin/puppet agent --test`
