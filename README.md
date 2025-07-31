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

## Bundle 3
### Exercise 1

```bash
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch ft/team-page
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  ft/team-page
  main  
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add team.html 
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add: Team Page"
[ft/team-page e021910] Add: Team Page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 447 bytes | 223.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/GedIra/theGym_Git_Exercise_Solutions/pull/new/ft/team-page
remote: 
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout main
Switched to branch 'main'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git log
commit e0219107e0d47b5cb0e054d1bce672d07b992faa (HEAD -> ft/team-page, origin/ft/team-page)
Author: GedIra <irankundag65@gmail.com>
Date:   Thu Jul 31 10:23:51 2025 +0200

    Add: Team Page

commit 9f5a4f25ed6c041f735675fe757380a7c48452aa (origin/ft/service-redesign, ft/service-redesign)
Merge: ab8b301 5776a8b
Author: GedIra <irankundag65@gmail.com>
Date:   Wed Jul 30 12:01:32 2025 +0200

    Merge branch 'main' into ft/service-redesign

commit 5776a8b31adca40723437d8152cd5a6c881f00f9
Author: GedIra <irankundag65@gmail.com>
Date:   Wed Jul 30 12:00:00 2025 +0200
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git cherry-pick e0219107e0d47b5cb0e054d1bce672d07b992faa
[ft/contact-page ee8559c] Add: Team Page
 Date: Thu Jul 31 10:23:51 2025 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add --all
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add: Contact Page & Team page"
[ft/contact-page 093b5b6] Add: Contact Page & Team page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin ft/contact-page 
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 724 bytes | 362.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/GedIra/theGym_Git_Exercise_Solutions/pull/new/ft/contact-page
remote: 
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ touch faq.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add --all
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Add: FAQ Page"
[ft/faq-page 23dc47f] Add: FAQ Page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 441 bytes | 441.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/GedIra/theGym_Git_Exercise_Solutions/pull/new/ft/faq-page
remote: 
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git revert e0219107e0d47b5cb0e054d1bce672d07b992faa
[ft/faq-page f6c17ca] Revert "Add: Team Page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git add --all
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git commit -m "Delete: Team Page"
[ft/faq-page d0cec10] Delete: Team Page
 1 file changed, 1 insertion(+), 1 deletion(-)
gedira@gedira-HP-EliteBook-840-G3:~/projects/TheGym/theGym_Git_Exercise_Solutions$ git push
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 548 bytes | 182.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
To github.com:GedIra/theGym_Git_Exercise_Solutions.git
   23dc47f..d0cec10  ft/faq-page -> ft/faq-page
```