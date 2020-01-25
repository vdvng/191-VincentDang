# Git Kata: Basic Commits
This kata will introduce you to the `git add` and `git commit` commands.

This is a very introductory kata. if you have used `git status`, `git log --oneline --graph`, `git add` and `git commit` extensively you should probably skip it.

You can look at the bottom of this file, if you have not yet done basic git configuration.

## Setup:

1. Run `. setup.sh` (or `.\setup.ps1` in PowerShell)

## The task

1. Use `git status` to see which branch you are on.
2. What does `git log` look like?

commit ab2b967f17a987dfd88271aab8e4c3dbc96661d2 (HEAD -> master)
Merge: 254d05f f8712d5
Author: Vincent <dangvh1@uci.edu>
Date:   Fri Jan 24 20:53:22 2020 -0800

    Merge branch 'master' of https://github.com/praqma-training/git-katas

commit 254d05f8ade365cd4a7c0ff000ffafe31fc5661b (greeting)
Author: Vincent <dangvh1@uci.edu>
Date:   Fri Jan 24 20:49:07 2020 -0800

    Add missing shebang in squashing/setup.sh
    
    `setup.sh` should be executable according to the instructions given in README.md

commit f8712d5c4df74fa0d49c8cc9ba3b1a5b2c571072 (origin/master, origin/HEAD)
Author: Frank Theile <ftheile@grundfos.com>
Date:   Mon Dec 9 10:30:13 2019 +0100

    Add missing shebang in squashing/setup.sh
    
    `setup.sh` should be executable according to the instructions given in READM:


3. Create a file
4. What does the output from `git status` look like now?

On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store
	file.txt

no changes added to commit (use "git add" and/or "git commit -a")

5. `add` the file to the staging area
6. How does `git status` look now?

On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	new file:   file.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store

7. `commit` the file to the repository
8. How does `git status` look now?

On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store

no changes added to commit (use "git add" and/or "git commit -a")


9. Change the content of the file you created earlier
10. What does `git status` look like now?

On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md
	modified:   file.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store

no changes added to commit (use "git add" and/or "git commit -a")

11. `add` the file change
12. What does `git status` look like now?

On branch master
Your branch is ahead of 'origin/master' by 3 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

	modified:   file.txt

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store
13. Change the file again
14. Make a `commit`
15. What does the `status` look like now? The `log`?

[master ad680e5] added more changes
 1 file changed, 1 insertion(+), 1 deletion(-)
vincentdang@Vincents-MacBook-Pro basic-commits % git status
On branch master
Your branch is ahead of 'origin/master' by 4 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

	modified:   ../3-way-merge/README.md
	modified:   file.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	../.DS_Store

no changes added to commit (use "git add" and/or "git commit -a")
16. Commit the newest change

## Useful commands
- `git add`
- `git commit`
- `git commit -m "My commit message"`
- `git log`
- `git log -n 5`
- `git log --oneline`
- `git log --oneline --graph`
- `touch filename` to create a file (or `sc filename ''` in PowerShell)
- `echo content > file` to overwrite file with content (or `sc filename 'content'` in PowerShell)
- `echo content >> file` to append file with content (or `ac filename 'content'` in PowerShell)


## Git Initial Configuration
1. `git config --global user.name "John Doe"`
1. `git config --global user.email "johndoe@example.com`

For the vim scared:
- `git config --global core.editor nano`

For the windows peeps:
- `git config --global core.editor notepad`

Other editor options:
- `git config --global core.editor "atom --wait"`
- `git config --global core.editor "'C:/Program Files/Notepad++/notepad++.exe' -multiInst"`
