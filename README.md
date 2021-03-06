Git
===

https://help.github.com/articles/generating-ssh-keys
 Generating SSH Keys
 Step 1: Check for SSH keys
 Step 2: Generate a new SSH key
 Step 3: Add your SSH key to GitHub

http://wiki.eclipse.org/EGit/User_Guide#GitHub_Tutorial
 Working with remote Repositories

https://help.github.com/articles/changing-a-remote-s-url
 Changing a remote's URL
 Switching remote URLs from HTTPS to SSH

https://help.github.com/articles/error-permission-denied-publickey
 Error: Permission denied (publickey)

install the Eclipse ADT Bundle
  http://developer.android.com/sdk/installing/index.html?pkg=adt
How to completely uninstall eclipse?
  http://askubuntu.com/questions/282951/how-to-completely-uninstall-eclipse 

Add new file
  테스트 파일을 로컬에 카피
  git  add/commit/push

Create a new repository on the command line

touch README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/sspark1973/GitHubTest.git
git push -u origin master


Push an existing repository from the command line

git remote add origin https://github.com/sspark1973/GitHubTest.git
git push -u origin master

make branch
  git checkout -b roypark_rhea_bootup 
  git push  <REMOTENAME> <LOCALBRANCHNAME>:<REMOTEBRANCHNAME> 
  git push origin roypark_rhea_bootup:master

Pushing to a remote

  git branch
  git remote

  git pull origin master
  git push  <REMOTENAME> <BRANCHNAME> 
  git push origin master

rebase
  git pull --rebase

revert
  git revert <commit id>

log
  git log -- <file name>
  git log -p
  git log --stat
  git log --pretty=oneline
  git log <branch/tag/commit>

reset
  git reset --hard HEAD^
  git reset --hard HEAD // undo ANY local changes and reset your workspace to the last commit on the branch.

show
  git show <commit ID> // will display the changes made in the specified commit

tag
  git tag -l // How to find out list of available tags

diff / patch
  patch -p0 < patch file
  git diff > patchfile
  git diff master..test
  git diff HEAD
