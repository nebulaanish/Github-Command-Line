# Github-Command-Line-

- git config --global user.name Anish
- git config --global user.email "nebulaanish@gmail.com"   // useful to show contributions in github profile

- touch .gitignore
- git init  // initialize the git project and make .git hidden folder
- git add .     //upload every files except ignored in staging area
- git commit -m "Name of commit"
- git status   // shows the status of project on git
- git remote add origin [ssh link to the github]  // copy ssh link from the repository


[one time process]
// make ssh key for your pc and edit in the github global settings

- git push origin master


## How to initialise git in the computer: ##
1. git init

### Adding git username and setting up email:
1. git config --global user.name "YOUR_USERNAME"
2. git config --global user.email "your_email_address"

### How to check your username and email:
1. git config --global user.name
2. git config --global user.email

### 1."How to set proxy in git"
git config  --global http.proxy 172.16.20.2:3128

### 2."How to unset git proxy
git config --global --unset http.proxy

### Steps to make feature branch up-to-date with main branch
- First commit every changes into the development branch and change to main branch
git checkout main
- Fetch latest branches and their commit from remote repo
git fetch -p main
- merge changes from origin/main to local main branch, the local changes aren't harmed but synced with the remote repo
git merge origin/main
- change to feature branch
git checkout <branch_name>
- merge recently updated local main branch to local feature branch
git merge main
- text editor pops up, add a commit and then
git push origin <branch_name>

### 3."How to check current git proxy
git config --global --get http.proxy


## Steps to commit changes:

1. git showdown (git log --decorate --oneline --all --graph)
2. git add [location of files or folders].
3. git status
4. git commit -m "Description of commit".

## Steps for branching
For adding branch
1. git branch [branch name]
2. git checkout [branch name]
3. git branch -d [branch name]

## Steps for remote:
1. git remote add [remote name] [remote link]
2. git remote remove [remote name]

## Steps for pushing, fetching, pulling, merging and rebasing.
1. git push [remote name] [remote branch]
2. git pull [remote name] [remote branch]
3. git fetch [remote name] [remote branch]
4. git merge [remote name]/[remote branch]
5. git rebase [remote name]/[remote branch]

## Steps for updating the online branches of a repo:
git fetch [remote name]

## Steps for resetting :
#### for resetting every changes made currently:
1. git reset --hard
#### for resetting the repo to the last commit:
1. git reset --hard HEAD^
#### for resetting the repo to the last n commits(n is a number):
1. git reset --hard HEAD~3
