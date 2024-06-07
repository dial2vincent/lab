# Git
**"Git"** is software that helps developers to work simultaneously while maintaining a complete history of their work, without overwriting each other’s work.

**“GitHub”** is a website that provides us a remote repository, so you can put all your work on the cloud, thereby it is backed up & interactive through its visual interface.
## Git installation and configuration

## Git commands:
~~~
git --version
git config -l
git config --edit --global   #Edit global setting
git remote -v


git config --list      #show you list
git config --global user.email "youruserid@yahoo.com
git config --global user.name "yournamehere"
git config -l
git config --edit --global   #Edit global setting

mkdir folder1
cd folder
git init        # If you want to undo init> rm -rf .git 
git status
git add .
git commit -m 'Updated comment'
git remote add origin x # replace x with copy the HTTPS URL of the repository created
git remote add origin https://github.com/dial2vincent/lab.git
git remote -v
git push -u origin master


git config --list
git config --global -e
code .                                           # 비주얼 스튜디오를 사용한다면 
git config --global core.editor "code"           # VS를 주 에딕터로 사용한다면 
git config --global core.editor "code --wait"      
git --global user.name "Vincent Lee"
git --global user.email "dial2vincent@yahoo.com"
git config --global alias.st status              # 단축키로 st 만치면 status가 나타난다. 
git st
git config -h
~~~
