Git
===

# Create a new repository on the command line

touch README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/sspark1973/GitHubTest.git
git push -u origin master


# Push an existing repository from the command line

git remote add origin https://github.com/sspark1973/GitHubTest.git
git push -u origin master

# make branch
git checkout -b roypark_rhea_bootup 
git push  <REMOTENAME> <LOCALBRANCHNAME>:<REMOTEBRANCHNAME> 
git push origin roypark_rhea_bootup:master

# Pushing to a remote

git branch
git remote

git pull origin master
git push  <REMOTENAME> <BRANCHNAME> 
git push origin master

# rebase
git pull --rebase

# rever
git revert <commit id>

# log
git log -- <file name>
git log -p
git log --stat
git log --pretty=oneline
git log <branch/tag/commit>

# reset
git reset --hard HEAD^
git reset --hard HEAD // undo ANY local changes and reset your workspace to the last commit on the branch.

# show
git show <commit ID> // will display the changes made in the specified commit

# tag
git tag -l // How to find out list of available tags

# diff / patch
patch -p0 < patch file
git diff > patchfile
git diff master..test
git diff HEAD
