# Gym-Git-Exercise-Solutions

## Bundle1
### Exercise1

```bash script

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop
$ mkdir exercise-1

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop
$ cd exercise-1

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1
$ git init
Initialized empty Git repository in C:/Users/USER/Desktop/exercise-1/.git/

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (master)
$ git branch -m main

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ touch about-us.html index.html contact-us.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ ls
about-us.html  contact-us.html  index.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ mv about-us.html About_Us.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ ls
About_Us.html  contact-us.html  index.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ vi index.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git log
fatal: your current branch 'main' does not have any commits yet

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git add .
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git commit -m "Bundle1-Exercise1 project files"
[main (root-commit) 966758c] Bundle1-Exercise1 project files
 3 files changed, 69 insertions(+)
 create mode 100644 About_Us.html
 create mode 100644 contact-us.html
 create mode 100644 index.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git log
commit 966758c050c0bc04f2f5dd03c809b66f6e6ff823 (HEAD -> main)
Author: BaRemy <bahatiremy05@gmail.com>
Date:   Wed May 17 04:03:31 2023 +0200

    Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git remote add origin https://github.com/BaRemy/git-exercises.git

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git branch -M main

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 866 bytes | 866.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/BaRemy/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git branch dev

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git switch dev
Switched to branch 'dev'

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git branch
* dev
  main

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git switch -c test
Switched to a new branch 'test'

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (test)
$ git switch dev
Switched to branch 'dev'

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git branch -d test
Deleted branch test (was 966758c).

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$
```

## Bundle1
### Exercise2

```bash script

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop
$ cd exercise-1/

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ touch home.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ vi home.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git add home.html
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ vi about.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git add about.html
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 966758c Bundle1-Exercise1 project files
stash@{1}: WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ vi team.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git add team.html
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash
Saved working directory and index state WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 966758c Bundle1-Exercise1 project files
stash@{1}: WIP on dev: 966758c Bundle1-Exercise1 project files
stash@{2}: WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (6346649d041e2452aeca611152d9c81c732c16b5)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 966758c Bundle1-Exercise1 project files
stash@{1}: WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (8e7cb92c6888fce5981d443380c7eb78e01aa36d)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git commit -m "home and about page files"
[dev 8b5468e] home and about page files
 2 files changed, 23 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 594 bytes | 297.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/BaRemy/git-exercises/pull/new/dev
remote:
To https://github.com/BaRemy/git-exercises.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash list
stash@{0}: WIP on dev: 966758c Bundle1-Exercise1 project files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (46f51631d20d48e91ab2e168835c3a80b5cf4198)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git reset --hard
HEAD is now at 8b5468e home and about page files

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$
```

## Bundle2
### Exercise1

```bash script

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop
$ ls
 Discord.lnk*  'Internet Download Manager.lnk'*  'PuTTY (64-bit).lnk'*  'Visual Studio Code.lnk'*   desktop.ini   exercise-1/

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop
$ cd exercise-1/

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git branch
* dev
  main

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git branch ft/bundle-2

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (dev)
$ git switch ft/bundle-2
Switched to branch 'ft/bundle-2'

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git add services.html
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git stash
giSaved working directory and index state WIP on ft/bundle-2: 8b5468e home and about page files
t
USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git stash
No local changes to save

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git stash pop
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Dropped refs/stash@{0} (2c34bdc8261e4aa7f1410c8de3da060bca759213)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git add services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git status
On branch ft/bundle-2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git commit -m "created services page"
[ft/bundle-2 5eea384] created services page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 483 bytes | 483.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/BaRemy/git-exercises/pull/new/ft/bundle-2
remote:
To https://github.com/BaRemy/git-exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$
```
## Bundle2
### Exercise2
```

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git pull
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 636 bytes | 8.00 KiB/s, done.
From https://github.com/BaRemy/git-exercises
   5b9410f..106393c  main       -> origin/main
Updating 5b9410f..106393c
Fast-forward
 about.html    | 12 ++++++++++++
 home.html     | 12 ++++++++++++
 services.html | 12 ++++++++++++
 3 files changed, 36 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git switch -c ft/service-redesign
Switched to a new branch 'ft/service-redesign'

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ ls
About_Us.html  about.html  contact-us.html  home.html  index.html  services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ vi service.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   services.html


USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git commit -m "feat: added service list"
[ft/service-redesign 6b90744] feat: added service list
 1 file changed, 5 insertions(+)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 360 bytes | 120.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/BaRemy/git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/BaRemy/git-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ ls
About_Us.html  about.html  contact-us.html  home.html  index.html  services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git commit -m "feat: added different service list"
[main b9a3d3e] feat: added different service list
 1 file changed, 5 insertions(+)

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 368 bytes | 368.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/BaRemy/git-exercises.git
   106393c..b9a3d3e  main -> main

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git switch fft/service-redesign
fatal: invalid reference: ft/service-redesign

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (main)
$ git switch ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git diff

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign|MERGING)
$ vi services.html

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign|MERGING)
$ git diff
diff --cc services.html
index 9f498fe,4d292c0..0000000
--- a/services.html
+++ b/services.html
@@@ -8,10 -8,10 +8,15 @@@
  <body>
      <h1>This is a Service page</h1>
      <p>This a short paragraph for my Service page to be submited to The Gym Git Exercises</p>
 +    <ul>
 +          <li>Web development</li>
 +          <li>App development</li>
 +          <li>UI Design</li>
 +    </ul>
+     <ol>
+           <li>Architect</li>
+           <li>Maintanance</li>
+           <li>Prototyping</li>
+     </ol>
  </body>
  </html>

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign|MERGING)
$ git add .

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign|MERGING)
$ $ git commit -m "updated services|conflicts resolved"
bash: $: command not found

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign|MERGING)
$ git commit -m "updated services|conflicts resolved"
[ft/service-redesign 92d3844] updated services|conflicts resolved

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git merge main
Already up to date.

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 385 bytes | 385.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/BaRemy/git-exercises.git
   6b90744..92d3844  ft/service-redesign -> ft/service-redesign

USER@DESKTOP-CE1U6VD MINGW64 ~/Desktop/exercise-1 (ft/service-redesign)
$
```
