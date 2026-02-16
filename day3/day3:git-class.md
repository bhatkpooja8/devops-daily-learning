
main → feature branch → PR → review → merge → deploy

first be in main branch
Create a feature branch
git checkout -b feature/day3


create a file 

next
Commit:
git add .
git commit -m "Day3: add git workflow notes"

git push -u origin feature/day3

What is a PR?

A request to merge feature branch into main

Rebase vs Merge:
Merge

Combines two branches as they are

Creates a merge commit

History is preserved exactly

Example:

main      A---B---C
               \
feature          D---E


After merge:

main      A---B---C------M
               \        /
feature          D---E--


 You can see who did what and when


Rebase

Moves your commits on top of latest main

Rewrites history

No merge commit

Before:

main      A---B---C
               \
feature          D---E


After rebase:

main      A---B---C---D---E


 Looks clean, like feature was written after main


 git stash – temporary save (VERY common)

Used when:

You’re halfway through work

Urgent bug comes

You need clean working tree

git stash
git checkout main


Bring back:

git stash pop

git revert (production safe)

Undo a commit safely:

git revert <commit-id>


git cherry-pick:
Pick one specific commit from another branch and apply it to current branch.

git log --oneline — What it does

It shows the commit history in a short, clean format.

git cherry-pick --continue