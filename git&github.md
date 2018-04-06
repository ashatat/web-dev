```git subtree push --prefix public origin gh-pages```

**Note**: Dist is the dir where you keep your index.html

**Fix a Git detached head?**
* Run ```git log -n 1``` ; this will display the most recent commit on the detached HEAD. ```Copy-and-paste``` the commit hash.
* Run ```git checkout master```
* Run ```git branch tmp <commit-hash>```. This will save your changes in a new branch called tmp.
If you would like to incorporate the changes you made into master, run ```git merge tmp``` from the master branch. You should be on the master branch after running ```git checkout master```.
