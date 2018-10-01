# Git Commands
* cancel `git add my_file`  
``` bash
$ git reset my_file
```

* git stash (untracked or modifed files)  
  - apply stash 
  ``` bash
  $ git stash
  ```
  - show list
  ``` bash
  $ git stash list
  ```
  - show stashed contents
  ``` bash
  $ git stash show stash@{N]
  ```
  - unstash
  ``` bash
  # removed from stashed list 
  $ git stash pop stash@{N}
  # remains at stashed list
  $ git stash apply stash@{N}
  ```

* git branch
  - create origin branch
  ``` bash
  # create new local branch
  $ git checkout -b my_branch
  # create new remote branch
  $ git push origin my_branch
  ```
  - delete origin brach
  ``` bash
  # checkout for delete
  $ git checkout another_branch
  # remove local branch
  $ git branch -D my_branch
  # remove remote branch
  $ git push origin :my_branch
  ```
