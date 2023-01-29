## What is git rebase?

Git rebase is a process of changing the base commit of a branch to another commit.
When you create a new branch off a parent branch, the last commit id, let's use "12ab", would be the same for parent branch and child branch.
If you add more commits or features to the child branch with ids '37bc' and "87eb" the commit tree or log of the child branch would be in this manner, "12ab"-"37bc"-"87eb".
Now if a colleague then pushes to the parent branch, they'll create more commit ids "98yu", "43po". So the commit log for the parent branch would be in this manner, "12ab"-"98yu"-"43po".
Now remember the parent branch and child branch has this commit in commmon "12ab". If you do "git rebase parent" on the child branch, it changes the
commit tree of the child branch and makes the most recent commit of the parent branch it's base. i.e the commit log becomes
"12ab"-"98yu"-"43po"-"37bc"-"87eb" for the child branch.

## What is git cherry-picking?

Git cherry-picking allows you apply specific changes from one branch to another branch.
It works by selecting individual commits from one branch and applying them to another branch, rather than merging the entire branch.

## When or why do we use them?

Git cherry-picking is used when you want to apply specific changes from one branch to another, while Git rebasing is used when you want to integrate all changes from one branch into another.
