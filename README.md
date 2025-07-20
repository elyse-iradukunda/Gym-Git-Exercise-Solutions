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

```

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch ft/service-redesign

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git status
On branch main
Your branch and 'origin/main' have diverged,
and have 3 and 2 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

nothing to commit, working tree clean

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git add services.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git commit -m'Adding services redesigned file'
[ft/service-redesign baafa3e] Adding services redesigned file
 1 file changed, 1 insertion(+), 1 deletion(-)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 16 threads

Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 2.62 KiB | 894.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git diff

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 3 and 2 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git merge ft/service-redesign
Updating 7b1107f..baafa3e
Fast-forward
 services.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

```

## Bundle 3
### Exercise 1
```

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch ft/team-page

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git checkout ft/team-page
M       README.md
Switched to branch 'ft/team-page'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git add team.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git push origin ft/team-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git commit -m'added new file team.html'
[ft/team-page 1264391] added new file team.html
 1 file changed, 2 insertions(+)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 339 bytes | 339.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
   f94d4e8..1264391  ft/team-page -> ft/team-page

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git branch ft/contact-page

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (main)
$ git checkout ft/team-page
M       README.md
Switched to branch 'ft/team-page'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git log
commit 126439162567d42da173d15d534dd69c31935099 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Sun Jul 20 14:17:20 2025 +0200

    added new file team.html

commit f94d4e81d191e13ab4d6d109f64c5420d1ae217a (origin/main, origin/HEAD, main, ft/contact-page)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 19:08:09 2025 +0200

    Bundle 2 - exercise 2

commit 4cba6bb9fb88e418b38a4e6d485298a028654c0c
Merge: baafa3e ea3b1a8
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 19:06:04 2025 +0200

    Bundle 2 - exercise 2

commit baafa3e110a40a9ff4847c8affcee69e896b1a15 (origin/ft/service-redesign, ft/service-redesign)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 18:27:55 2025 +0200

    Adding services redesigned file

commit 7b1107fa7c3e2ea8bcca593a68b104d30b959e77
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 18:08:31 2025 +0200

    End of Bundle 2 exercise 1

commit ea3b1a81ee2fa3770142bbbdbeb70a83a9221a35
Merge: ab09f62 052f083
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 17:07:32 2025 +0200

    Merge pull request #2 from elyse-iradukunda/ft/bundle-2

    Second bundle exercise 1 solution

commit 0161ce718d61aae93de8c0798fd366ad72bfc0ce (list)
Merge: a03ac26 ab09f62
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 17:06:35 2025 +0200

    merge

commit a03ac26268e8d53140a6d0b8007136ee2e87fd32
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:24:56 2025 +0200

    before going to dev

commit 052f083d6b698c021cca2db5a88061199389ba88 (origin/ft/bundle-2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo
(END)
2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200
Date:   Thu Jul 17 17:07:32 2025 +0200

    Merge pull request #2 from elyse-iradukunda/ft/bundle-2

    Second bundle exercise 1 solution

commit 0161ce718d61aae93de8c0798fd366ad72bfc0ce (list)
Merge: a03ac26 ab09f62
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 17:06:35 2025 +0200

    merge

commit a03ac26268e8d53140a6d0b8007136ee2e87fd32
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:24:56 2025 +0200

    before going to dev

commit 052f083d6b698c021cca2db5a88061199389ba88 (origin/ft/bundle-commit 052f083d6b698c021cca2db5a88061199389ba88 (origin/ft/bundle-commit 052f083d6b698c021cca2db5a88061199389ba88 (origin/ft/bundle-2, ft/bundle-2)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 16:09:29 2025 +0200

    Second bundle exercise 1 solution

commit ab09f622df39c613a5981dd13e41d5581a447376
Merge: b860d43 1b9438c
Author: Elyse Iradukunda <ellycreativity8@gmail.com>
Date:   Thu Jul 17 16:02:13 2025 +0200

    Merge pull request #1 from elyse-iradukunda/ft/bundle-2

    added new html files bundle 2

commit 1b9438c6706ba7e1adbceaf74fa8e19273577d5f
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:40:44 2025 +0200

    Add services.html file

commit 75e892396eb610629b7271112a267bdccbbe2156 (origin/dev)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 15:10:34 2025 +0200

    After adding all file and stashing

commit a6308cba4efe82ba7a7f59a0515861138b351f65
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:54:53 2025 +0200

    First bundle solutions exercise 1

commit b860d430dcc9dd3dbb478c640f0e456ded789062 (switch)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Thu Jul 17 12:42:30 2025 +0200

    feature: I added my first readme file in repo

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/team-page)
$ git checkout ft/contact-page
M       README.md
Switched to branch 'ft/contact-page'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git log ft/team-page -1
commit 126439162567d42da173d15d534dd69c31935099 (origin/ft/team-page, ft/team-page)
Author: Irael <user@LAPTOP-5DF3FEI>
Date:   Sun Jul 20 14:17:20 2025 +0200

    added new file team.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git cherry-pick 126439162567d42da173d15d534dd69c31935099
[ft/contact-page 73a54e0] added new file team.html
 Date: Sun Jul 20 14:17:20 2025 +0200
 1 file changed, 2 insertions(+)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git commit -m'some changes on contact-page'
On branch ft/contact-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 348 bytes | 348.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git branch ft/faq-page

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/contact-page)
$ git checkout ft/faq-page
M       README.md
Switched to branch 'ft/faq-page'

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/faq-page)
$ git add faq.html

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/faq-page)
$ git commit -m'adding faq page'
[ft/faq-page 97b527e] adding faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

[ft/faq-page 0b99c7a] Revert "added new file team.html"
 1 file changed, 2 deletions(-)

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/faq-page)
$ git commit -m'last for bundle 3 exercise 1'
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/faq-page)
$ git push --set-upstream
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 357 bytes | 357.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/elyse-iradukunda/Gym-Git-Exercise-Solutions.git
   97b527e..0b99c7a  ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

user@Irael MINGW64 /d/Coding/Gym_Git_Exercise_Solutions (ft/faq-page)
$

```