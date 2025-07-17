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