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


```
