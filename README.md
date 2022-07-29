# branch-and-merge
Instructions and examples on creating branches and merging code with git

Branches
- branch names should be descriptive and potentially reference the related issue or the user working on that branch
- create a branch using: git branch [branch name], then git checkout [branch name] (can also use git switch [branch name]), or using git checkout -b [branch name] which combines the command to create the branch and switch over to that branch
- branches should be used for new features or bug fixes, and should generally be narrow in scope
- check current branch (and all branches) using: git branch
- delete branches once they have been merged into another branch or are no longer in uses

Merge Conflicts
- merge conflicts occur when there are conflicting changes at the same region of a file
- push branch and add to remote repo using: git push -u origin [branch name]
- pull main into a branch using: git checkout [branch name] (needed if not already on that branch), then git pull origin main
- merge conflicts will show up in the code with the 7 iterations of the characters <, >, =
  - <<<<<<< to ======= are the local changes
  - ======= to >>>>>>> are the changes from the repo/other branch that you are merging with
- can fix merge conflicts in the github interface or within the local scripts


![git branches](/git_branches.png?raw=true "Git Branches")
