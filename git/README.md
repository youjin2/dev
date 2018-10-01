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
