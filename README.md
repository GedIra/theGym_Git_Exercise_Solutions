# Gym Git Exercise Solutions
## Bundle 1
### Exercise 1

```bash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym$ mkdir theGym_Git_Exercise_Solutions
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym$ cd theGym_Git_Exercise_Solutions/
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch README.md
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git init
Initialized empty Git repository in /home/gedira/projects/TheGym/theGym_Git_Exercise_Solutions/.git/
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch -M master
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch -M master main
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add --all
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md

gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add README.md file"
[main (root-commit) d4bd039] Add README.md file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git remote add origin git@github.com:GedIra/theGym_Git_Exercise_Solutions.git
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 223 bytes | 223.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b dev
Switched to a new branch 'dev'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b test
Switched to a new branch 'test'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout dev
Switched to branch 'dev'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch
* dev
  main
  test
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch -D test
Deleted branch test (was d4bd039).
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch
* dev
  main
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$
```

### Exercise 2

```bash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch home.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add home.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash list
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch about.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add about.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash list
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash list
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash push -m "Team"
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash list
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash pop stash@{1}
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash pop stash@{1}
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add: home.html and about.html"
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git stash pop
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git reset --hard
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git status
```

## Bundle 2
### Exercise 1

```bash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch
  dev
* ft/bundle-2
  main
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch services.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add services.html 
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add: services.html page"
[ft/bundle-2 50e5f2f] Add: services.html page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 481 bytes | 240.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/GedIra/theGym_Git_Exercise_Solutions/pull/new/ft/bundle-2
remote: 
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
### Exercise 2
```bash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 2.55 KiB | 1.27 MiB/s, done.
From github.com:GedIra/theGym_Git_Exercise_Solutions
   d9588bc..29ff141  main        -> origin/main
   50e5f2f..b5a6a40  ft/bundle-2 -> origin/ft/bundle-2
Updating d9588bc..29ff141
Fast-forward
 README.md     | 284 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++-----------------------------------------------------------
 about.html    |  11 +++++
 home.html     |  11 +++++
 services.html |  11 +++++
 4 files changed, 175 insertions(+), 142 deletions(-)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 services.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add services.html 
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Update: Our new Services"
[ft/service-redesign ab8b301] Update: Our new Services
 1 file changed, 9 insertions(+), 1 deletion(-)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 560 bytes | 560.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/GedIra/theGym_Git_Exercise_Solutions/pull/new/ft/service-redesign
remote: 
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout  ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add services.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "update: Added our mission"
[main 5776a8b] update: Added our mission
 1 file changed, 2 insertions(+)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 391 bytes | 391.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
   29ff141..5776a8b  main -> main
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git merge main
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add services.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit
[ft/service-redesign 9f5a4f2] Merge branch 'main' into ft/service-redesign
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 442 bytes | 442.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
   ab8b301..9f5a4f2  ft/service-redesign -> ft/service-redesign
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$
```