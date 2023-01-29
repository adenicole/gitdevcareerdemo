## TOPIC: GIT

## GIT REBASE:
Git rebase is a command that allows you to take the changes from a branch and apply them onto another branch.

Example:
You have a branch called "dev-career" and you want to apply the changes onto the "master" branch. You would run the command:
`git rebase master`

You want to squash several commits together into one commit on a branch called "dev-career". You would run the command:
`git rebase -i HEAD~3`
This command will open an editor where you can specify which commits to squash.

In both instances, the changes from the "dev-career" branch will be applied on top of the "master" branch or squashed into one commit.

## GIT CHERRY-PICKING:
Git cherry-picking allows you to select specific commits from one branch and apply them to another branch. Here's an example:
* Checkout the branch you want to cherry-pick from: 
`git checkout dev-career` (where `dev-career` is target branch)
* Use the command git log to view the commits on the branch
* Identify the commit hash of the commit you want to cherry-pick and then switch back to the target branch:
`git checkout target-branch`
* Use the command `git cherry-pick <commit-hash>` to apply the specific commit to the target branch.
* Use `git cherry-pick --continue` or `git cherry-pick --abort` as necessary.

## USE CASES:
* Git cherry-picking is used to select specific commits from a branch and apply them to another branch. This allows you to selectively merge changes from one branch into another without merging the entire branch.
* Git rebase is used to reapply commits on top of another base branch. This can be useful for cleaning up a messy commit history, or for integrating changes from one branch into another that were made at different times. It can also be used to update a feature branch with changes that were made to the base branch while the feature branch was being developed.
