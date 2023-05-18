### BUNDLE 1
## EXERCISE 1
```
PS C:\Users\student\Downloads\git_exercise> git init
PS C:\Users\student\Downloads\git_exercise> echo "# Git-exercise" >> README.md
PS C:\Users\student\Downloads\git_exercise> git init
Initialized empty Git repository in C:/Users/student/Downloads/git_exercise/.git/
PS C:\Users\student\Downloads\git_exercise> git commit -m "my first commit"
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

PS C:\Users\student\Downloads\git_exercise> git add README.md
PS C:\Users\student\Downloads\git_exercise> git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

PS C:\Users\student\Downloads\git_exercise> git commit -m "my first commit"
[master (root-commit) c635570] my first commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
PS C:\Users\student\Downloads\git_exercise> git branch -m master main
PS C:\Users\student\Downloads\git_exercise> git remote add origin https://github.com/AL2002MI08/Git-exercise.git
PS C:\Users\student\Downloads\git_exercise> git push origin main
To https://github.com/AL2002MI08/Git-exercise.git
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git pull origin main
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 7 (delta 2), reused 4 (delta 1), pack-reused 0
From https://github.com/AL2002MI08/Git-exercise
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories
PS C:\Users\student\Downloads\git_exercise> git push origin main
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
 * branch            main       -> FETCH_HEAD
Enumerating objects: 5, done.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 401 bytes | 133.00 KiB/s, done.
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/AL2002MI08/Git-exercise.git
   c88a436..10bca56  main -> main
PS C:\Users\student\Downloads\git_exercise> git status
On branch main
nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise> git branch dev
PS C:\Users\student\Downloads\git_exercise> git checkout dev
PS C:\Users\student\Downloads\git_exercise> git branch test
PS C:\Users\student\Downloads\git_exercise> git branch -d test
Deleted branch test (was 10bca56).
PS C:\Users\student\Downloads\git_exercise> git add .   
PS C:\Users\student\Downloads\git_exercise> git commit -m "added dev branch"
On branch dev
nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise> git push origin dev
 ! [rejected]        dev -> dev (fetch first)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git push -f
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\student\Downloads\git_exercise> git push --set-upstream origin dev
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        dev -> dev (fetch first)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git pull
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 3 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 263 bytes | 0 bytes/s, done.
From https://github.com/AL2002MI08/Git-exercise
 * [new branch]      dev        -> origin/dev
There is no tracking information for the current branch.

    git pull <remote> <branch>

    git branch --set-upstream-to=origin/<branch> dev

PS C:\Users\student\Downloads\git_exercise> git push origin dev
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        dev -> dev (non-fast-forward)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git commit -m "updated readme"
On branch dev
nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise> git add .
PS C:\Users\student\Downloads\git_exercise> git commit -m "updated Readme file"
On branch dev
Changes not staged for commit:
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\student\Downloads\git_exercise> git add .
PS C:\Users\student\Downloads\git_exercise> git commit -m "update Readme"
 1 file changed, 0 insertions(+), 0 deletions(-)
PS C:\Users\student\Downloads\git_exercise> git push origin dev
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        dev -> dev (non-fast-forward)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git pull origin dev
From https://github.com/AL2002MI08/Git-exercise
 * branch            dev        -> FETCH_HEAD
warning: Cannot merge binary files: README.md (HEAD vs. 3535ed2b25b344ba0305d81f00b901d011f82889)
Auto-merging README.md
CONFLICT (content): Merge conflict in README.md
Automatic merge failed; fix conflicts and then commit the result.
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        dev -> dev (non-fast-forward)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\student\Downloads\git_exercise> git push --set-upstream origin dev
To https://github.com/AL2002MI08/Git-exercise.git
 ! [rejected]        dev -> dev (non-fast-forward)
error: failed to push some refs to 'https://github.com/AL2002MI08/Git-exercise.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\student\Downloads\git_exercise> git push --set-upstream origin dev -f
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 300 bytes | 100.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/AL2002MI08/Git-exercise.git
 + 3535ed2...044dd00 dev -> dev (forced update)
branch 'dev' set up to track 'origin/dev'
```
# Exercise 2
````
PS C:\Users\student\Downloads\git_exercise> git add home.html
PS C:\Users\student\Downloads\git_exercise> git stash 
README.md: needs merge
PS C:\Users\student\Downloads\git_exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:
        new file:   home.html

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   README.md

PS C:\Users\student\Downloads\git_exercise> git status
Your branch is up to date with 'origin/dev'.

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Changes to be committed:
        new file:   home.html

Unmerged paths:
  (use "git add <file>..." to mark resolution)

PS C:\Users\student\Downloads\git_exercise> git commit -m "merge readme files"
[dev 7645fa3] merge readme files
PS C:\Users\student\Downloads\git_exercise> git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 4 threads
Writing objects: 100% (6/6), 773 bytes | 85.00 KiB/s, done.
To https://github.com/AL2002MI08/Git-exercise.git
   044dd00..7645fa3  dev -> dev
PS C:\Users\student\Downloads\git_exercise> ls


    Directory: C:\Users\student\Downloads\git_exercise


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----


PS C:\Users\student\Downloads\git_exercise> git stash
PS C:\Users\student\Downloads\git_exercise> git -r home.html
unknown option: -r
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]
PS C:\Users\student\Downloads\git_exercise> git rm home.html
PS C:\Users\student\Downloads\git_exercise> git add home.html
PS C:\Users\student\Downloads\git_exercise> git status
Your branch is up to date with 'origin/dev'.
Changes to be committed:

PS C:\Users\student\Downloads\git_exercise> git stash
Saved working directory and index state WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash list
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git add about.html
PS C:\Users\student\Downloads\git_exercise> git status
Your branch is up to date with 'origin/dev'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

PS C:\Users\student\Downloads\git_exercise> git stash
Saved working directory and index state WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash apply
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

PS C:\Users\student\Downloads\git_exercise> git stash list
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git add about.html
Saved working directory and index state WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash list    
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
stash@{1}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git add team.html
PS C:\Users\student\Downloads\git_exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

PS C:\Users\student\Downloads\git_exercise> git stash
Saved working directory and index state WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash list    
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
stash@{1}: WIP on dev: 2d9bcb2 remove stash file
stash@{2}: WIP on dev: 2d9bcb2 remove stash file
stash@{3}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise> git stash drop stash@{1}
usage: git stash drop [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors

PS C:\Users\student\Downloads\git_exercise> git stash drop stash@{1}
error: unknown switch `e'
usage: git stash drop [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors

PS C:\Users\student\Downloads\git_exercise> git stash drop stash@{1}
error: unknown switch `e'
usage: git stash drop [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors

PS C:\Users\student\Downloads\git_exercise> git stash drop {1}      
error: unknown switch `e'
usage: git stash drop [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors

PS C:\Users\student\Downloads\git_exercise> git stash drop <1>      
+ git stash drop <1>
+                 ~
Missing file specification after redirection operator.
At line:1 char:16
+ git stash drop <1>
+                ~
At line:1 char:19
+ git stash drop <1>
+                   ~
Missing file specification after redirection operator.
    + CategoryInfo          : ParserError: (:) [], ParentContainsErrorRecordException
    + FullyQualifiedErrorId : MissingFileSpecification

PS C:\Users\student\Downloads\git_exercise> git stash drop 1
PS C:\Users\student\Downloads\git_exercise> git stash list
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
stash@{2}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash pop stash@{1}
error: unknown switch `e'
usage: git stash pop [--index] [-q | --quiet] [<stash>]

    -q, --quiet           be quiet, only report errors
    --index               attempt to recreate the index

PS C:\Users\student\Downloads\git_exercise> git stash pop 1        

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
Dropped refs/stash@{1} (7883ff1f66790b5655f7090eb1241cb161552e29)
PS C:\Users\student\Downloads\git_exercise> git stash list
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
stash@{1}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash pop 1
On branch dev
Your branch is up to date with 'origin/dev'.

  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

PS C:\Users\student\Downloads\git_exercise> git add --all
[dev 47a393d] created new files and stash save
 2 files changed, 19 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
PS C:\Users\student\Downloads\git_exercise> git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Writing objects: 100% (4/4), 639 bytes | 213.00 KiB/s, done.
To https://github.com/AL2002MI08/Git-exercise.git
   2d9bcb2..47a393d  dev -> dev
PS C:\Users\student\Downloads\git_exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise> git stash list
stash@{0}: WIP on dev: 2d9bcb2 remove stash file
PS C:\Users\student\Downloads\git_exercise> git stash pop 0
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (23b421edea73de80af9662a438773c6c7aeebe10)
PS C:\Users\student\Downloads\git_exercise> git reset --hard
HEAD is now at 47a393d created new files and stash save
PS C:\Users\student\Downloads\git_exercise> git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean
PS C:\Users\student\Downloads\git_exercise>
```
### Bundle 2
## Exercise 1 
´´´
PS C:\Users\student\Downloads\git_exercise> git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add" to track)
PS C:\Users\student\Downloads\git_exercise> git add services.html
PS C:\Users\student\Downloads\git_exercise> git commit -m "service page added"
[ft/bundle-2 12f6c5c] service page added
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
PS C:\Users\student\Downloads\git_exercise> git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\student\Downloads\git_exercise> git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 485 bytes | 161.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/AL2002MI08/Git-exercise/pull/new/ft/bundle-2
remote:
To https://github.com/AL2002MI08/Git-exercise.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
PS C:\Users\student\Downloads\git_exercise>
´´´

