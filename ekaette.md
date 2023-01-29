## DevCareers Cloud DevOps Assignment

What is git rebase?
what is git cherry-pick?

when or why do we use them.


### Git Rebase

Synopsis:
	git rebase [--option] <branchToRebase> <>

*git rebase* provides convenience in updating your commit history of your branch to that of the parent branch. As the name suggests it shifts the base commit of your branch to the most recent commit of the parent. If branch is specified, *git rebase* performs an automatic switch to the specified branch before executing the command.
	This is important in instances where the 

### Git Cherry-pick

Synopsis:
	git cherry-pick <!commit>

*git cherry-pick* is used to apply the specified commit to the current branch. This means that it modifies the current branch by adding one commit which could originate from another branch.
