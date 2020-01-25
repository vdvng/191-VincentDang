# Git Kata: 3-Way Merge

## Setup

1. Run `. setup.sh` (or `.\setup.ps1` in PowerShell)

## The task
You again live in your own branch, this time we will be doing a bit of juggling with branches, to show how lightweight branches are in git.

1. Create a branch called greeting and check it out
2. Edit the greeting.txt to contain your favorite greeting
3. Add greeting.txt files to the staging area
4. Commit
5. Switch back to the master branch
6. Create a file README.md with information about this repository
7. Add the README.md file to staging area and make the commit
8. What is the output of `git log --oneline --graph --all`?
*   ab2b967 (HEAD -> master) Merge branch 'master' of https://github.com/praqma-training/git-katas
|\  
| * f8712d5 (origin/master, origin/HEAD) Add missing shebang in squashing/setup.sh
* | 254d05f (greeting) Add missing shebang in squashing/setup.sh
|/  
* e060df6 Word ordering
* 6ccb858 Mention `less` in SHELL-BASICS.md
* f805e2a Added kata for .gitattributes
* 9669044 Simplify `git lol` alias
* 892d64f Fix link in squashing-README
| * c13fcff (origin/Expand_on_submodule_kata) Fix three typos
| * d9711cd Expand  on  submodules kata
|/  
* 1f9ead1 Minor improvements to submodules/README.md
* 956ac8d Removed reference to 'git rev-pars'
* 9313b5a Improved squashing/README.md
* eb6c517 Added kata about git tags.
* 451a2b0 Update README.md
* 5ccbc50 Changed "git" to "Git" in detached-head/README
* f94e033 Added to the task detached-head/README.
* 1b921a4 Added The task in save-my-commit/README.md 

9. Diff the branches
10. Merge the greeting branch into master

## Useful commands
- `git branch`
- `git branch <branch-name>`
- `git branch -d <branch-name>`
- `git checkout <branch-name>`
- `git checkout -b <branch-name>`
- `git branch -v`
- `git add`
- `git commit`
- `git commit -m`
- `git merge <branchA> <branchB>`
- `git diff <branchA> <branchB>`
- `git log --oneline --graph --all`
