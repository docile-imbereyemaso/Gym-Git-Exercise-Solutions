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
