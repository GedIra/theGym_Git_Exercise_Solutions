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
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin dev
branch 'dev' set up to track 'origin/dev'.
Everything up-to-date
```