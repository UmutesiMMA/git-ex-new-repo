# The-gym-git-exercise-solutions
## Bundle 1
### Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/Project

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project
$ git init
Initialized empty Git repository in C:/Users/user/Documents/TheGym/Project/.git/

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (master)
$ git branch -m "master" "main"

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch start.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch story.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch notes.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch review.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
lamp.jpeg  review.txt  step.jpeg   trees-lamp.jpeg
notes.txt  start.html  story.html
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git mv review.txt feedback.txt

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   feedback.txt
        new file:   lamp.jpeg
        new file:   notes.txt
        new file:   start.html
        new file:   step.jpeg
        new file:   story.html
        new file:   trees-lamp.jpeg


user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "First"
[main (root-commit) d1e51b8] First
 7 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 feedback.txt
 create mode 100644 lamp.jpeg
 create mode 100644 notes.txt
 create mode 100644 start.html
 create mode 100644 step.jpeg
 create mode 100644 story.html
 create mode 100644 trees-lamp.jpeg

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git remote add origin https://github.com/UmutesiMMA/The-gym-git-exercise-solution.git

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git branch -M main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 5.00 MiB | 1.07 MiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git switch -c dev
Switched to a new branch 'dev'

 user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git push origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 5.00 MiB | 682.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/d
ev
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      dev -> dev

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git switch -c test
Switched to a new branch 'test'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/t
est
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      test -> test

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (test)
$ git switch dev
Switched to branch 'dev'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git branch -d test
Deleted branch test (was d1e51b8).

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git push origin --delete test
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 - [deleted]         test
```

### Exercise 2

```bash
user@DESKTOP-TQVNUUS MINGW64 ~
$ cd ~/Documents/TheGym/Project/

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch home.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash
Saved working directory and index state WIP on main: d1e51b8 First

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch about.hhtml

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch about.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add about.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash -m "about page"
Saved working directory and index state On main: about page

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ touch team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add team.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash -m "team page"
Saved working directory and index state On main: team page

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (708dd030faf601bbf98cc41067442e5c4df45abf)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash list
stash@{0}: On main: team page
stash@{1}: WIP on main: d1e51b8 First

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (e014cca4c5401550881d92b1cc4a8435d657429f)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "Team page not included"
[main 35a55b2] Team page not included
 2 files changed, 32 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git fetch origin
remote: Enumerating objects: 10, done.
remote: Counting objects: 100% (10/10), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (9/9), 3.20 KiB | 25.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   d1e51b8..42f1a9b  main       -> origin/main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
Merge made by the 'ort' strategy.
 README.md | 212 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 212 insertions(+)
 create mode 100644 README.md

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.04 KiB | 266.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   42f1a9b..d63f8d9  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$
```
## Bundle 2
### Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
$ git switch -c ft/bundle-2
Switched to a new branch 'ft/bundle-2'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ touch service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git add service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git commit -m "Service page"
[ft/bundle-2 fac79a3] Service page
 1 file changed, 18 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$ git push origin ft/bundle-2
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 4 threads
Compressing objects: 100% (18/18), done.
Writing objects: 100% (18/18), 4.53 KiB | 356.00 KiB/s, done.
Total 18 (delta 9), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (9/9), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/bundle-2
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
$
```

### Exercise 2
```bash

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git commit -m "new changes in service redesign branch"
[ft/service-redesign dff22e4] new changes in service redesign branch
 1 file changed, 20 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 563 bytes | 187.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/service-redesign
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/bundle-2)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
README.md   feedback.txt  lamp.jpeg  start.html  story.html
about.html  home.html     notes.txt  step.jpeg   trees-lamp.jpeg

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
remote: Enumerating objects: 13, done.
remote: Counting objects: 100% (12/12), done.
remote: Compressing objects: 100% (9/9), done.
remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (9/9), 3.26 KiB | 37.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   d63f8d9..de9b1d9  main                 -> origin/main
 * [new branch]      revert-3-ft/bundle-2 -> origin/revert-3-ft/bundle-2
Updating d63f8d9..de9b1d9
Fast-forward
 README.md    | 78 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 service.html | 18 ++++++++++++++
 2 files changed, 96 insertions(+)
 create mode 100644 service.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ ls
README.md   feedback.txt  lamp.jpeg  service.html  step.jpeg   trees-lamp.jpeg
about.html  home.html     notes.txt  start.html    story.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "changes on same line different branches"
[main 3c7d551] changes on same line different branches
 1 file changed, 2 insertions(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 361 bytes | 120.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   de9b1d9..3c7d551  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git diff ft/service-redesign main
diff --git a/README.md b/README.md
index c510bc8..34c5cea 100644
--- a/README.md
+++ b/README.md
@@ -207,6 +207,84 @@ $ git commit -m "Team page not included"
  2 files changed, 32 insertions(+)
  create mode 100644 about.html
  create mode 100644 home.html
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git fetch origin
+remote: Enumerating objects: 10, done.
+remote: Counting objects: 100% (10/10), done.
+remote: Compressing objects: 100% (9/9), done.
+remote: Total 9 (delta 5), reused 0 (delta 0), pack-reused 0
+Unpacking objects: 100% (9/9), 3.20 KiB | 25.00 KiB/s, done.
+From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
+   d1e51b8..42f1a9b  main       -> origin/main
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git push origin main
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+ ! [rejected]        main -> main (non-fast-forward)
+error: failed to push some refs to 'https://github.com/UmutesiMMA/The-gym-git-exerc
ise-solutions.git'
+hint: Updates were rejected because the tip of your current branch is behind
+hint: its remote counterpart. Integrate the remote changes (e.g.
+hint: 'git pull ...') before pushing again.
+hint: See the 'Note about fast-forwards' in 'git push --help' for details.
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git pull
+Merge made by the 'ort' strategy.
+ README.md | 212 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
+ 1 file changed, 212 insertions(+)
+ create mode 100644 README.md
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$ git push origin main
+Enumerating objects: 8, done.
+Counting objects: 100% (8/8), done.
+Delta compression using up to 4 threads
+Compressing objects: 100% (6/6), done.
+Writing objects: 100% (6/6), 1.04 KiB | 266.00 KiB/s, done.
+Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
+remote: Resolving deltas: 100% (2/2), completed with 1 local object.
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+   42f1a9b..d63f8d9  main -> main

+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
+$
+
```
## Bundle 2
### Exercise 1
```bash
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (main)
+$ git switch -c ft/bundle-2
+Switched to a new branch 'ft/bundle-2'
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ touch service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git add service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git commit -m "Service page"
+[ft/bundle-2 fac79a3] Service page
+ 1 file changed, 18 insertions(+)
+ create mode 100644 service.html
+
+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$ git push origin ft/bundle-2
+Enumerating objects: 19, done.
+Counting objects: 100% (19/19), done.
+Delta compression using up to 4 threads
+Compressing objects: 100% (18/18), done.
+Writing objects: 100% (18/18), 4.53 KiB | 356.00 KiB/s, done.
+Total 18 (delta 9), reused 0 (delta 0), pack-reused 0
+remote: Resolving deltas: 100% (9/9), completed with 1 local object.
+remote:
+remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
+remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/
f
+t/bundle-2
+remote:
+To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
+ * [new branch]      ft/bundle-2 -> ft/bundle-2

+user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/project (ft/bundle-2)
+$
diff --git a/service.html b/service.html
index 89fdab2..59a54fe 100644
--- a/service.html
+++ b/service.html
@@ -8,13 +8,12 @@
 </head>
 <body>

-    <di> Services we provide</di>
+    <di> Services that our company provides include:</di>
     <ul><li>Sell</li>
         <li>Repair</li>
         <li>Make from scratch</li>
+        <li> Buy </li>

     </ul>
-    <div>Coupons:</div>
-    <div>How to access out services</div>
 </body>
 </html>
\ No newline at end of file

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git merge main
Auto-merging service.html
CONFLICT (add/add): Merge conflict in service.html
Automatic merge failed; fix conflicts and then commit the result.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign|MERGING)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign|MERGING)
$ git commit -m "Merging main with ft/service-redesign"
[ft/service-redesign bf35848] Merging main with ft/service-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/service-redesign)
$ git push origin ft/service-redesign
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 233 bytes | 116.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   dff22e4..bf35848  ft/service-redesign -> ft/service-redesign
```
### Bundle3
## Exercise 2
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/faq-page)
$ git checkout -b ft/home-redesign
Switched to a new branch 'ft/home-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "changes to home page"
[main 7b6219d] changes to home page
 1 file changed, 2 insertions(+), 1 deletion(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 402 bytes | 201.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   1bc787e..7b6219d  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git switch ft/home-redesign
Switched to branch 'ft/home-redesign'

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git rebase main
Successfully rebased and updated refs/heads/ft/home-redesign.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git add home.html

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git commit -m "nav bar on home page"
[ft/home-redesign fed2d79] nav bar on home page
 1 file changed, 8 insertions(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git push origin ft/home-redesign
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 1.45 KiB | 370.00 KiB/s, done.
Total 12 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-redesign' on GitHub by visiting:
remote:      https://github.com/UmutesiMMA/The-gym-git-exercise-solutions/pull/new/f
t/home-redesign
remote:
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 * [new branch]      ft/home-redesign -> ft/home-redesign

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$
```
### Bundle4
## Exercise 1
```bash
user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (ft/home-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git remote add git-copy https://github.com/UmutesiMMA/git-ex-new-repo.git

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git remote
git-copy
origin

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git add .

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git commit -m "slogan on home page"
[main c4b8190] slogan on home page
 1 file changed, 2 insertions(+)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/UmutesiMMA/The-gym-git-exerci
se-solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 1.15 KiB | 98.00 KiB/s, done.
From https://github.com/UmutesiMMA/The-gym-git-exercise-solutions
   7b6219d..fe5888c  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 97 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++-------
 1 file changed, 87 insertions(+), 10 deletions(-)

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 638 bytes | 319.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/UmutesiMMA/The-gym-git-exercise-solutions.git
   fe5888c..b6a7060  main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push origin main
Everything up-to-date

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$ git push git-copy
Enumerating objects: 49, done.
Counting objects: 100% (49/49), done.
Delta compression using up to 4 threads
Compressing objects: 100% (48/48), done.
Writing objects: 100% (49/49), 5.01 MiB | 752.00 KiB/s, done.
Total 49 (delta 24), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (24/24), done.
To https://github.com/UmutesiMMA/git-ex-new-repo.git
 * [new branch]      main -> main

user@DESKTOP-TQVNUUS MINGW64 ~/Documents/TheGym/Project (main)
$

```

## Exercise 2
```bash


```


