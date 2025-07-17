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
```
