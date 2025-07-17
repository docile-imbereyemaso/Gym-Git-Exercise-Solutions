# GIT Exercise
## Bundle 1
### Exercise 1

```Bash
user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning
$ git init 
Initialized empty Git repository in C:/Users/user/Desktop/The Gym-phase II/Git $ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)   

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git add README.md

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ gi commit -m"Initial commit"
bash: gi: command not found

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git commit -m"Initial commit"
[main (root-commit) c784115] Initial commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git remote add origin https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 217 bytes | 108.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
Writing objects: 100% (3/3), 217 bytes | 108.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git       
 * [new branch]      main -> main

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git       
 * [new branch]      main -> main

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git       
 * [new branch]      main -> main

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
 * [new branch]      main -> main

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git branch dev
$ git branch dev


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git branch test

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git checkout test
Switched to branch 'test'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (test)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git branch -D test
Deleted branch test (was c784115).

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$

## Bundle1

## Exercise 2

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
ng (dev)
$ git stash
No local changes to save
ng (dev)
$ git stash
No local changes to save

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -u
Saved working directory and index state WIP on dev: 89654ef Add the git commands  in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -u
Saved working directory and index state WIP on dev: 89654ef Add the git commands  in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -u
Saved working directory and index state WIP on dev: 89654ef Add the git commands  in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash  list 
stash@{0}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{1}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{2}: WIP on dev: 89654ef Add the git commands in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash@{1}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash@{0}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)   

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git add team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git shash list
git: 'shash' is not a git command. See 'git --help'.

The most similar command is
        stash

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash list
stash@{0}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{1}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{2}: WIP on dev: 89654ef Add the git commands in Readme file

$ git stash -m "Stash team.html file for temporary work" --team.html
error: unknown option `team.html'
usage: git stash list [<log-options>]
   or: git stash show [-u | --include-untracked | --only-untracked] [<diff-options>] [<stash>]
   or: git stash drop [-q | --quiet] [<stash>]
   or: git stash pop [--index] [-q | --quiet] [<stash>]
   or: git stash apply [--index] [-q | --quiet] [<stash>]
   or: git stash branch <branchname> [<stash>]
   or: git stash [push [-p | --patch] [-S | --staged] [-k | --[no-]keep-index] [-q | --quiet]
                 [-u | --include-untracked] [-a | --all] [(-m | --message) <message>]
                 [--pathspec-from-file=<file> [--pathspec-file-nul]]
                 [--] [<pathspec>...]]
   or: git stash save [-p | --patch] [-S | --staged] [-k | --[no-]keep-index] [-q | --quiet]
                 [-u | --include-untracked] [-a | --all] [<message>]
   or: git stash clear
   or: git stash create [<message>]
   or: git stash store [(-m | --message) <message>] [-q | --quiet] <commit>    

    -k, --[no-]keep-index keep index
    -S, --[no-]staged     stash staged changes only
    -p, --[no-]patch      stash in patch mode
    -q, --[no-]quiet      quiet mode
    -u, --[no-]include-untracked
                          include untracked files in stash
    -a, --[no-]all        include ignore files
    -m, --[no-]message <message>
                          stash message
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -m "Stash team.html file for temporary work" -- team.html
Saved working directory and index state On dev: Stash team.html file for temporary work

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)   

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git add about.html home.html 

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git commit -m "Adding about and home page"
[dev d3d977e] Adding about and home page
 2 files changed, 11 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash list
stash@{0}: On dev: Stash team.html file for temporary work
stash@{1}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{2}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{3}: WIP on dev: 89654ef Add the git commands in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash{3}
error: stash{3} is not a valid reference

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash@{3}
Already up to date.
home.html already exists, no checkout
error: could not restore untracked files from stash
On branch dev
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)   

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git log
commit d3d977ea55c531e09aa47912afd03143f4f8504a (HEAD -> dev)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 16:23:41 2025 +0200

    Adding about and home page

commit 89654efbf9344178c57ea9eef4eaaa636ef610ec (origin/dev)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 15:39:50 2025 +0200

    Add the git commands  in Readme file

commit c7841159917e1e2ddd395e2af41183a621e88fe5 (origin/main, main)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 15:26:03 2025 +0200

    Initial commit

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash 
No local changes to save

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -u
Saved working directory and index state WIP on dev: d3d977e Adding about and home page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash list
stash@{0}: WIP on dev: d3d977e Adding about and home page
stash@{1}: On dev: Stash team.html file for temporary work
stash@{2}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{3}: WIP on dev: 89654ef Add the git commands in Readme file
stash@{4}: WIP on dev: 89654ef Add the git commands in Readme file

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash{0}
error: stash{0} is not a valid reference

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash apply stash@{0}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git log --oneline
d3d977e (HEAD -> dev) Adding about and home page
89654ef (origin/dev) Add the git commands  in Readme file
c784115 (origin/main, main) Initial commit

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset --hard d3d977e
HEAD is now at d3d977e Adding about and home page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git rm team.html
fatal: pathspec 'team.html' did not match any files

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git ls-files
README.md

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ ls
README.md  team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ rm team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git add team.html 

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git checkout main
A       team.html
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git rm team.html 
error: the following file has changes staged in the index:
    team.html
(use --cached to keep the file, or -f to force removal)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git rm -f team.html
rm 'team.html'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git status
On branch dev
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash -u
Saved working directory and index state WIP on dev: d3d977e Adding about and home page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout dev
Switched to branch 'dev'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git stash pop
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped refs/stash@{0} (b06e9b2d7b4044a5064f115dc09a2a2ec7a4b26f)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$ git reset

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (dev)
$


```
## Bundle 3

## Exercise 

``` Bash

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/service-redesign)

$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git add team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git commit -m "feat: add the team page"
[ft/team-page 708b8f8] feat: add the team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 466 bytes | 466.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:        
remote:      https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git checkout main
error: Your local changes to the following files would be overwritten by checkout:
        team.html
Please commit your changes or stash them before you switch branches.
Aborting

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git status
On branch ft/team-page
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)        
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git add .

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git status
On branch ft/team-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html

[ft/team-page 6492ee9] feat : add the team page
 1 file changed, 1 insertion(+), 1 deletion(-)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git status
On branch ft/team-page
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log 
commit 6492ee95fb63105b249e77c76fb15610e9920757 (HEAD -> ft/team-page)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 22:48:13 2025 +0200

    feat : add the team page

commit 708b8f8e6416a78a29249c486090bd740f4e5b81 (origin/ft/team-page)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 22:45:54 2025 +0200

    feat: add the team page

commit b529d840954cc4ecd5c3894d8f1de3e37605878b (origin/main, main, ft/contact-page)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 18:07:22 2025 +0200

    Updates the service page

commit c307f6e78055ee9c5b1dae72fff7a019e797bc4d
Merge: 7b861b8 d4eabb4
Author: docile imbereyemaso <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 18:03:26 2025 +0200

    Merge pull request #4 from docile-imbereyemaso/ft/service-redesign

    Add the content to service page

commit d4eabb44eb2b94b25517b19403ff4927dbe1e823
Merge: 6b77220 7b861b8
Author: docile imbereyemaso <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 18:03:02 2025 +0200

    Merge branch 'main' into ft/service-redesign

commit 6b772201e7b2f236557a407816e1515693144dce
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 18:01:22 2025 +0200

    Add the content to service page

commit 7b861b82dae4e73530eb98a3823cf984f78770c5
Merge: 1f4b4e9 5af78d3
Author: Dosite Iradukunda Cyiza <145858744+dosite-cyiza@users.noreply.github.com>
Date:   Thu Jul 17 17:52:35 2025 +0200

    Merge pull request #3 from docile-imbereyemaso/ft/bundle-2

    Adding the content to service page

commit 5af78d3ea256d2f3ee07bfd90aeff5ae3db69a79 (origin/ft/bundle-2, ft/bundle-2)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 17:47:02 2025 +0200

    Adding the content to service page

commit 1f4b4e90fef360372ab17c627268719303159b6b
Merge: f1efa4e 08d432e
Author: docile imbereyemaso <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 17:10:41 2025 +0200

    Merge pull request #2 from docile-imbereyemaso/ft/bundle-2

    Adding new page page service.html

commit 08d432e711edd33651537ae072e336cedbe10437
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 17:08:03 2025 +0200

    Adding new page page service.html

commit f1efa4ecc069e040f541a0264937d79d69a07a3f
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 16:59:34 2025 +0200

    Add the commands of Bundle1 Exercise2 in readme file

commit c56e5660915463ecd7fd29f8ded6e1205a9d13f9
Merge: c784115 89654ef
Author: docile imbereyemaso <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 15:52:20 2025 +0200

    Merge pull request #1 from docile-imbereyemaso/dev

    Add the git commands  in Readme file

commit 89654efbf9344178c57ea9eef4eaaa636ef610ec (origin/dev)
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 15:39:50 2025 +0200

    Add the git commands  in Readme file

commit c7841159917e1e2ddd395e2af41183a621e88fe5
Author: Docile123 <imbereyemasoo@gmail.com>
Date:   Thu Jul 17 15:26:03 2025 +0200

    Initial commit

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log --oneline
6492ee9 (HEAD -> ft/team-page) feat : add the team page
708b8f8 (origin/ft/team-page) feat: add the team page
b529d84 (origin/main, main, ft/contact-page) Updates the service page
c307f6e Merge pull request #4 from docile-imbereyemaso/ft/service-redesign     
d4eabb4 Merge branch 'main' into ft/service-redesign
6b77220 Add the content to service page
7b861b8 Merge pull request #3 from docile-imbereyemaso/ft/bundle-2
5af78d3 (origin/ft/bundle-2, ft/bundle-2) Adding the content to service page   
1f4b4e9 Merge pull request #2 from docile-imbereyemaso/ft/bundle-2
08d432e Adding new page page service.html
f1efa4e Add the commands of Bundle1 Exercise2 in readme file
c56e566 Merge pull request #1 from docile-imbereyemaso/dev
89654ef (origin/dev) Add the git commands  in Readme file
c784115 Initial commit

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log --oneline -h
usage: git log [<options>] [<revision-range>] [[--] <path>...]
   or: git show [<options>] <object>...

    -q, --[no-]quiet      suppress diff output
    --[no-]source         show source
    --[no-]use-mailmap    use mail map file
    --[no-]mailmap        alias of --use-mailmap
    --clear-decorations   clear all previously-defined decoration filters      
    --[no-]decorate-refs <pattern>
                          only decorate refs that match <pattern>
    --[no-]decorate-refs-exclude <pattern>
                          do not decorate refs that match <pattern>
    --[no-]decorate[=...] decorate options
    -L <range:file>       trace the evolution of line range <start>,<end> or function :<funcname> in <file>


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log --oneline --reverse
c784115 Initial commit
89654ef (origin/dev) Add the git commands  in Readme file
c56e566 Merge pull request #1 from docile-imbereyemaso/dev
f1efa4e Add the commands of Bundle1 Exercise2 in readme file
08d432e Adding new page page service.html
1f4b4e9 Merge pull request #2 from docile-imbereyemaso/ft/bundle-2
5af78d3 (origin/ft/bundle-2, ft/bundle-2) Adding the content to service page   
7b861b8 Merge pull request #3 from docile-imbereyemaso/ft/bundle-2
6b77220 Add the content to service page
d4eabb4 Merge branch 'main' into ft/service-redesign
c307f6e Merge pull request #4 from docile-imbereyemaso/ft/service-redesign     
b529d84 (origin/main, main, ft/contact-page) Updates the service page
708b8f8 (origin/ft/team-page) feat: add the team page
6492ee9 (HEAD -> ft/team-page) feat : add the team page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

 in tree.
error: could not apply 6492ee9... feat : add the team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
hint: Disable this message with "git config advice.mergeConflict false"        

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ gti status
bash: gti: command not found

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 6492ee9.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
Unmerged paths:
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by us:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/team-page
team.html: needs merge
error: you need to resolve your current index first

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git stash
team.html: needs merge
error: could not write index

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit 6492ee9.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Unmerged paths:
  (use "git add/rm <file>..." as appropriate to mark resolution)
        deleted by us:   team.html

no changes added to commit (use "git add" and/or "git commit -a")

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --continue
U       team.html
error: Committing is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.      

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --abort

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)
$ git checkout main
Switched to branch 'main'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (main)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)
$ git status
On branch ft/team-page
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)
$ git commit --oneline --reverse
error: unknown option `oneline'
usage: git commit [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
                  [--dry-run] [(-c | -C | --squash) <commit> | --fixup [(amend|reword):]<commit>]
                  [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
                  [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
                  [--date=<date>] [--cleanup=<mode>] [--[no-]status]
                  [-i | -o] [--pathspec-from-file=<file> [--pathspec-file-nul]]
                  [(--trailer <token>[(=|:)<value>])...] [-S[<keyid>]]
                  [--] [<pathspec>...]

    -q, --[no-]quiet      suppress summary after successful commit
    -v, --[no-]verbose    show diff in commit message template

Commit message options
    -F, --[no-]file <file>
                          read message from file       
    --[no-]author <author>
                          override author for commit   
    --[no-]date <date>    override date for commit     
    -m, --[no-]message <message>
                          commit message
    -c, --[no-]reedit-message <commit>
                          reuse and edit message from specified commit
    -C, --[no-]reuse-message <commit>
                          reuse message from specified commit
    --[no-]fixup [(amend|reword):]commit
                          use autosquash formatted message to fixup or amend/reword specified commit
    --[no-]squash <commit>
                          use autosquash formatted message to squash specified commit
    --[no-]reset-author   the commit is authored by me now (used with -C/-c/--amend)
    --trailer <trailer>   add custom trailer(s)        
    -s, --[no-]signoff    add a Signed-off-by trailer  
    -t, --[no-]template <file>
                          use specified template file  
    -e, --[no-]edit       force edit of commit
    --[no-]cleanup <mode> how to strip spaces and #comments from message
    --[no-]status         include status in commit message template
    -S, --[no-]gpg-sign[=<key-id>]
                          GPG sign commit

Commit contents options
    -a, --[no-]all        commit all changed files     
    -i, --[no-]include    add specified files to index for commit
    --[no-]interactive    interactively add files      
    -p, --[no-]patch      interactively add changes    
    -o, --[no-]only       commit only specified files  
    -n, --no-verify       bypass pre-commit and commit-msg hooks
    --verify              opposite of --no-verify      
    --[no-]ahead-behind   compute full ahead/behind values
    --[no-]porcelain      machine-readable output
    --[no-]long           show status in long format (default)
    -z, --[no-]null       terminate entries with NUL
    --[no-]amend          amend previous commit
    --no-post-rewrite     bypass post-rewrite hook
    --post-rewrite        opposite of --no-post-rewrite    -u, --[no-]untracked-files[=<mode>]
                          show untracked files, optional modes: all, normal, no. (Default: all)
    --[no-]pathspec-from-file <file>
                          read pathspec from file
    --[no-]pathspec-file-nul
                          with --pathspec-from-file, pathspec elements are separated with NUL character


user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log  --oneline --reverse
c784115 Initial commit
89654ef (origin/dev) Add the git commands  in Readme file
c56e566 Merge pull request #1 from docile-imbereyemaso/dev
f1efa4e Add the commands of Bundle1 Exercise2 in readme file
08d432e Adding new page page service.html
1f4b4e9 Merge pull request #2 from docile-imbereyemaso/ft/bundle-2
5af78d3 (origin/ft/bundle-2, ft/bundle-2) Adding the content to service page   
7b861b8 Merge pull request #3 from docile-imbereyemaso/ft/bundle-2
6b77220 Add the content to service page
d4eabb4 Merge branch 'main' into ft/service-redesign
c307f6e Merge pull request #4 from docile-imbereyemaso/ft/service-redesign     
b529d84 (origin/main, main, ft/contact-page) Updates the service page
708b8f8 (origin/ft/team-page) feat: add the team page
6492ee9 (HEAD -> ft/team-page) feat : add the team page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git cherry-pick 708b8f8
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
error: could not apply 708b8f8... feat: add the team page
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".
hint: Disable this message with "git config advice.mergeConflict false"        

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page|CHERRY-PICKING)
$ git cherry-pick --abort

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git reset --hard HEAD~1
HEAD is now at 708b8f8 feat: add the team page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git log --oneline --reverse
c784115 Initial commit
89654ef (origin/dev) Add the git commands  in Readme file
c56e566 Merge pull request #1 from docile-imbereyemaso/dev
f1efa4e Add the commands of Bundle1 Exercise2 in readme file
08d432e Adding new page page service.html
1f4b4e9 Merge pull request #2 from docile-imbereyemaso/ft/bundle-2
5af78d3 (origin/ft/bundle-2, ft/bundle-2) Adding the content to service page   
7b861b8 Merge pull request #3 from docile-imbereyemaso/ft/bundle-2
6b77220 Add the content to service page
d4eabb4 Merge branch 'main' into ft/service-redesign
c307f6e Merge pull request #4 from docile-imbereyemaso/ft/service-redesign     
b529d84 (origin/main, main, ft/contact-page) Updates the service page
708b8f8 (HEAD -> ft/team-page, origin/ft/team-page) feat: add the team page    

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git status
On branch ft/team-page
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git cherry-pick 708b8f8
[ft/contact-page 31197cb] feat: add the team page      
 Date: Thu Jul 17 22:45:54 2025 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ ld
bash: ld: command not found

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ ls
README.md  service.html  team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git -a -m "feat: add the content to team page"
unknown option: -a
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--no-lazy-fetch]
           [--no-optional-locks] [--no-advice] [--bare] [--git-dir=<path>]
           [--work-tree=<path>] [--namespace=<name>] [--config-env=<name>=<envvar>]
           <command> [<args>]

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git commit -a -m "feat: add the content to team page"
[ft/contact-page 3e43961] feat: add the content to team page
 1 file changed, 1 insertion(+), 1 deletion(-)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git push origin ft/contact-page
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 741 bytes | 741.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page       
remote:
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git status
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git commit -am "feat: add the faq file"
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git commit -a -m "feat: add the faq file"
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git add faq.html 

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git commit -m "feat: add the faq file"
[ft/faq-page e9891a1] feat: add the faq file
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 494 bytes | 494.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page        

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)
$ git log --oneline --reverse
c784115 Initial commit
89654ef (origin/dev) Add the git commands  in Readme file
c56e566 Merge pull request #1 from docile-imbereyemaso/dev
f1efa4e Add the commands of Bundle1 Exercise2 in readme file
08d432e Adding new page page service.html
c307f6e Merge pull request #4 from docile-imbereyemaso/ft/service-redesign     
b529d84 (origin/main, main) Updates the service page
708b8f8 (HEAD -> ft/team-page, origin/ft/team-page) feat: add the team page    

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git revert 708b8f8
[ft/team-page 40c88ba] Revert "feat: add the team page" 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git status
On branch ft/team-page
nothing to commit, working tree clean

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 256 bytes | 256.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/docile-imbereyemaso/Gym-Git-Exercise-Solutions.git       
   708b8f8..40c88ba  ft/team-page -> ft/team-page

user@User MINGW64 ~/Desktop/The Gym-phase II/Git learning (ft/team-page)       
$
```