git authorization:

> git config --global user.name "Your_Name"
> git config --global user.email "email_address@domain.com"

# git commit to github

git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/kclogics/new.git
git push -u origin master


# git-imp-commands

git show HEAD@{"3 hours ago"}


git log --graph --decorate --oneline
git blame merge.md ///show when the changes are made

git diff

git log   /// git log commands most powerfl tool in git
git log --patch
git log --grep ar2 --oneline
git log -Gar2 --patch

git commit --amend /// To commit all the files...

imp......do it more often
git rebase -i ar1   //super power history editing...(rebase means change history) these are interactibe rebases



git reflog  // git reflog to access the ref log and fix seemingly recoverable mistakes
git reflog HEAD// git revert to create new commits that rever changes 
in previous commits...



git reflog HEAD@{15}

git reflog refs/heads/master

changing history in git:
1)with interactive rebaase that is based on very first commit in the history and remove this commit tha add the file while you
do the interactive rebase....dis dvantages:will create the entire new line of new commmits and entire new history....
and will change the shared history
2)edit the menu,remove the lines from menu and create a new commit,
the old broken commit stays in history,but at least it gets fixd later on
------------
git revert // git will do that autoatically

git revert 5720fdf //changes exactly the opposite of the original file

Be careful with  git reverse
reverse doesn't mean undo

it cannot revert the structure of data...
if reverse the merge,then merge can remove all the data
was added by the merge but it cannot remove the merge 
commit itself...

if merge is still there it can caouse confusion if you try to merge again...

888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888888


Distributd Model:
-Centalized

Branching Model:
-One Integrated Branch(master)
-One Feature Branch per Feature

Constraints:
-Keep master stable, fix it ASAP 
-integrate feature banches every few days
-Use merge over rebase by default

