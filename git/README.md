# Git Commands
* git add
  - add new file
  ``` bash
  $ git add my_file
  ```
  - revert added file
  ``` bash
  $ git reset my_file
  ```
* git commit
  - commit 
  - revert commit
    - soft: preserve index (added, staged)
    - mixed: cancel index (unadded, staged)
    - hard: cancel index (unadded, unstaged)
    - example
    ``` bash
    # show comit log
    $ git log
    # cancel only previous commit (added, staged)
    $ git reset --soft HEAD^
    # cancel last 2 previous commit (unadded, staged)
    $ git reset --mixed HEAD~2
    ```
  - show commit log
  ``` bash
  # not pushed log
  $ git log --branches --not --remotes
  # all previous log
  $ git log
  # show only commit message
  $ git log --oneline --graph --decorate
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
