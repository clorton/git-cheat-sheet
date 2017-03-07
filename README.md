# Git Cheat Sheet
Basic command and operations in Git

##Getting Started with a New Project##
1) Navigate to the project on GitHub (e.g. [HIV-Kenya](https://github.com/InstituteforDiseaseModeling/HIV-Kenya)).

2) Fork the project to have your personal copy on GitHub.

![fork project](https://github.com/clorton/git-cheat-sheet/raw/master/images/github-fork.png)

3) Copy the project URL in order to clone the repository on your local machine.

![copy url](https://github.com/clorton/git-cheat-sheet/raw/master/images/github-copy-url.png)

4) Clone the project on your local machine.

![clone in SourceTree](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-clone.png)
![Clone/Add/Create dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-clone-dialog.png)

5) Add the original project repository as a remote.

![Menu tree for Add Remote...](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-add-remote-menu.png)
![Repository Settings dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-repository-settings-dialog.png)
![Remote details dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-remote-details-dialog.png)
![Repository Settings with new remote](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-remote-details-dialog.png)

##Working with a Project##
1)	Fetch from the project repository to make sure your subsequent work is based on the latest code/scripts/data found on the ```master``` branch in the project repository.

![Fetch button](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-fetch.png)
![Fetch dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-fetch-dialog.png)

2)	Create a branch (branch early, branch often) – corollary: do not work in branch ```master```. Right click _in the graph view_ to create a branch based on the selected commit in the graph.

![branch](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-branch.png)

Give the new branch a short name descriptive of the work you are about to do.

![branch dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-new-branch-dialog.png)

3)	Create/update/delete files associated with the project.

4)	Commit the changes locally (this creates a record of the changes you made along with a comment about the purpose of the changes). This involves selecting the changes you want to record, _staging_ them, and committing them with a descriptive commit message.

![Unstaged changes](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-unstaged-changes.png)

Select the added, modified, or deleted files you want to include in the commit.

![Select and stage](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-stage.png)

Now you should see the files you selected in the "Staged files" windows above.

![Staged files](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-staged.png)

Enter a descriptive commit message and click "Commit."

![Commit message and button](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-commit-message.png)

5)	Rinse and repeat steps 2 & 3 as you see fit. It can be useful to checkpoint work in progress.

6)	Push the commit(s) to _your_ repository on GitHub – this serves two purposes: it makes a backup of the work you have done and it makes it possible to share the work with other people.

Right-click on the branch name _under "BRANCHES"_ to the left of the graph view. Select _your_ repository under the "Push to" menu option.

![Push options](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-push.png)

Double check that you have the right repository (the name and URL are shown at the top) and the branch you want to push.

![Push dialog](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-push-dialog.png)

7)	Rinse and repeat steps 2 through 5 as you see fit.

8)	Fetch from the project repository to see if other changes have gone in since you started working (see step 1).

9)	If there are changes in the project repository, rebase _your_ work on those changes and (re-)push your work to your repository on GitHub.

With your working branch checked out (should be in *bold* under "BRANCHES"), right-click on ifdm/master and choose "Rebase..."

![Rebase menu](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-rebase-menu.png)

If you have merge conflicts, SourceTree will inform you:

![Merge conflicts](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-merge-conflicts.png)

You can see the files with merge conflicts when you select "Working Copy" under "FILE STATUS". Files with merge conflicts will have one or more sections marked with ```<<<<<<<```, ```=======```, and ```>>>>>>>```. The changes in master will be the first section between ```<<<<<<<``` and ```=======```. Your changes will be in the second section between ```=======``` and ```>>>>>>>```.

![Edit merge conflicts](https://github.com/clorton/git-cheat-sheet/raw/master/images/merge-conflicts.png)

Once you have resolved all the conflicts (and staged all the previously conflicted files - see step 4), tell SourceTree to continue the rebase.

![Continue Rebase](https://github.com/clorton/git-cheat-sheet/raw/master/images/source-tree-continue-rebase.png)

10)	Create a pull request on GitHub for getting your changes into the project repository and onto the ```master``` branch.

![GitHub view](https://github.com/clorton/git-cheat-sheet/raw/master/images/github-initiate-pull-request.png)
![GitHub  open pull request](https://github.com/clorton/git-cheat-sheet/raw/master/images/github-open-pull-request.png)

11)	Once the pull request has been accepted and your work is on the ```master``` branch in the project repository, return to step 1.
