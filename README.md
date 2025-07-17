# Git exercises
## Bundle 1 

### exercise 1


```user@Irael MINGW64 /d/Coding (master)
$ mkdir Gym_Git_Exercise_Solutions

user@Irael MINGW64 /d/Coding (master)
$ git init
Reinitialized existing Git repository in D:/Coding/.git/

user@Irael MINGW64 /d/Coding (master)
$ git add README.md
fatal: pathspec 'README.md' did not match any files

user@Irael MINGW64 /d/Coding (master)
$ ls
Codewars_KATA/               JS_DOM/               course-JS-and-the-DOM/
Gym_Git_Exercise_Solutions/  OnlineCalculatorApp/  css_cloning_phase2/

user@Irael MINGW64 /d/Coding (master)
$ cd Gym_Git_Exercise_Solutions/

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ ls
README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git add README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git branch master main
fatal: not a valid object name: 'main'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git checkout main
error: pathspec 'main' did not match any file(s) known to git

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git checkout master
error: pathspec 'master' did not match any file(s) known to git

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git checkout -a master
error: unknown switch `a'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --[no-]guess          second guess 'git checkout <no-such-branch>' (default)
    --[no-]overlay        use overlay mode (default)
    -q, --[no-]quiet      suppress progress reporting
    --[no-]recurse-submodules[=<checkout>]
                          control recursive updating of submodules
    --[no-]progress       force progress reporting
    -m, --[no-]merge      perform a 3-way merge with the new branch
    --[no-]conflict <style>
                          conflict style (merge, diff3, or zdiff3)
    -d, --[no-]detach     detach HEAD at named commit
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -f, --[no-]force      force checkout (throw away local modifications)
    --[no-]orphan <new-branch>
                          new unborn branch
    --[no-]overwrite-ignore
                          update ignored files (default)
    --[no-]ignore-other-worktrees
                          do not check if another worktree is using this branch
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --[no-]patch      select hunks interactively
    --[no-]ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git switch main
fatal: invalid reference: main

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git branch -m master main

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch -m main  master

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git branch -m master main

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ../Codewars_KATA/
        ../JS_DOM/
        ../OnlineCalculatorApp/
        ../course-JS-and-the-DOM/
        ../css_cloning_phase2/


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git add README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git commit -m'feature: I added my first readme file in repo'

[main (root-commit) a3593f3] feature: I added my first readme file in repo
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Gym_Git_Exercise_Solutions/README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote add orinin https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push  origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote -v
orinin  https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git (fetch)
orinin  https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git (push)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote add orinin https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
error: remote orinin already exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch -M main

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git init
Initialized empty Git repository in D:/Coding/Gym_Git_Exercise_Solutions/.git/

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git add . README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git commit -m'feature: I added my first readme file in repo'                  [master (root-commit) b860d43] feature: I added my first readme file in repo
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (master)
$ git branch -M main

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote add orinin https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push -u origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote remove orinin

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git remote add origin https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 240 bytes | 240.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch dev

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git switch main dev
fatal: only one reference expected

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch -m main dev
fatal: a branch named 'dev' already exists

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git switch dev
Switched to branch 'dev'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git branch test

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git branch -m dev

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git branch -D test
Deleted branch test (was b860d43).

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$
```

### exercise 2

```

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git stash
README.md: needs merge
error: could not write index

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git stash save "My new document inserted!"
README.md: needs merge
error: could not write index

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ ^C


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git merge --abort
fatal: There is no merge to abort (MERGE_HEAD missing).

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git stash
README.md: needs merge
error: could not write index

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ ^C


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git switch -m dev
README.md: needs merge
error: you need to resolve your current index first

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git add README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git chechout -m dev
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git checkout -m dev
fatal: cannot continue with staged changes in the following files:
README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git stash
Saved working directory and index state WIP on main: b860d43 feature: I added my first readme file in repo

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git switch -m dev
Switched to branch 'dev'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
No local changes to save

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git add README.md

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
No local changes to save

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git add home.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: a6308cb First bundle solutions exercise 1

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
No local changes to save

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash -m'second file"
>
>
>
> git stash -m'second file"


> git stash -m'second file"



git stash -m'second file"


fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'file



git stash -m'second file'
>
> git stash -m'second file"



^C

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
No local changes to save

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git add --all

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: a6308cb First bundle solutions exercise 1
stash@{1}: WIP on main: b860d43 feature: I added my first readme file in repo

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git add team.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: a6308cb First bundle solutions exercise 1

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped refs/stash@{0} (fd6dad6e9ae71a90850b61adb62a0247971d76c3)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: a6308cb First bundle solutions exercise 1
stash@{1}: WIP on main: b860d43 feature: I added my first readme file in repo

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git chechout stash@{n} -- home.html
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git checkout stash@{n} -- home.html
fatal: invalid reference: stash@{n}

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git checkout stash@{0} -- home.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git commit -m'After adding all file and stashing'
[dev 75e8923] After adding all file and stashing
 3 files changed, 33 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git push --set-upstream origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 16 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 630 bytes | 210.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
   a6308cb..75e8923  dev -> dev
branch 'dev' set up to track 'origin/dev'.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: a6308cb First bundle solutions exercise 1
stash@{1}: WIP on main: b860d43 feature: I added my first readme file in repo

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git stash
No local changes to save

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git reset --hard
HEAD is now at 75e8923 After adding all file and stashing

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$


```


## bundle 2

### exercise 1

```

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git branch ft/bundle-2

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (dev)
$ git switch -m ft/bundle-2
M       README.md
Switched to branch 'ft/bundle-2'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/bundle-2)
$ git add services.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/bundle-2)
$ git commit -m'Add services.html file'
[ft/bundle-2 1b9438c] Add services.html file
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/bundle-2)
$ git push origin  ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 437 bytes | 218.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/bundle-2)
```
### Exercise 2

