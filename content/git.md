# Git
**"Git"** is software that helps developers to work simultaneously while maintaining a complete history of their work, without overwriting each other’s work.

**“GitHub”** is a website that provides us a remote repository, so you can put all your work on the cloud, thereby it is backed up & interactive through its visual interface.
## Git installation and configuration
### Git configuration:
- Sample case 1
~~~
git --version
git config --list      #show you list
git config --global user.email "youruserid@yahoo.com
git config --global user.name "yournamehere"
git config -l
git config --edit --global   #Edit global setting
git remote -v
~~~

- Sample case 2
~~~
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
## Git commands:
~~~
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
~~~
- Demo command
~~~
mkdir projects
cd projects
mkdir project1
cd project1
git init                  # git initialize 깃으로 Track 하기 시작할때 
ls -al
rm -rf .git               # 깃으로 더이상 Track 하고 싶지 않는다면 .git 폴더를 삭제한다.

git add filename
git status
git rm --cached *.*       # staging 에서 untracked 로 옮겨오고 싶다면 
echo *.log > .gitignore   # 만약 로그 파일을 git/github 에 추가하고 싶지 않다면 .gitignore 파일에 화일명을 추가하면 된다.
git diff                  # 변경된 내용을 working directory 에서 확인하고 싶다면
git diff --staged         # 변경된 내용을 staging area 에서 확인하고 싶다면 
git diff --cached         # cached 는 staged 와 마찬가지로 사용된다.
git diff -h
~~~

## Git use case:
저장소가 이미 만들어져 있는 경우: 
`git remote add origin https://github.com/dial2vincent/lab.git`

저장소로 부터 코드를 가져올 경우:
`git clone https://github.com/dial2vincent/lab.git`

저장소를 변경할 경우 :
`git remote set-url origin <저장소위치.git>`

