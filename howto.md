$ cd KotlinAsFirst2020


$ git remote add upstream-my https://github.com/Ken4ikS/KotlinAsFirst2021.git
$ git fetch upstream-my
$ git checkout -b backport
$ git cherry-pick d535f359...FETCH_HEAD
$ git remote add upstream-theirs https://github.com/KrolTryCode/KotlinAsFirst2021.git
$ git fetch upstream-theirs
$ git checkout master
$ git merge backport upstream-theirs/master
$ git add .
$ git remote -v > remotes
$ touch howto.md
