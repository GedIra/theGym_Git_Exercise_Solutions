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
