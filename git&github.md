```git subtree push --prefix public origin gh-pages```

**Note**: Dist is the dir where you keep your index.html

**Fix a Git detached head?**
* Run ```git log -n 1``` ; this will display the most recent commit on the detached HEAD. ```Copy-and-paste``` the commit hash.
* Run ```git checkout master```
* Run ```git branch tmp <commit-hash>```. This will save your changes in a new branch called tmp.
If you would like to incorporate the changes you made into master, run ```git merge tmp``` from the master branch. You should be on the master branch after running ```git checkout master```.


**Delete Local Branch**
To delete the local branch use one of the following:

```
$ git branch -d branch_name
$ git branch -D branch_name
```
Note: The -d option is an alias for --delete, which only deletes the branch if it has already been fully merged in its upstream branch. You could also use -D, which is an alias for --delete --force, which deletes the branch "irrespective of its merged status." [Source: man git-bran
