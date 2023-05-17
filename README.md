# Gym-Git-Exercise-Solutions

## Bundle1
### Exercise

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
