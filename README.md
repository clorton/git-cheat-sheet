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
1.	Fetch from the project repository to make sure your subsequent work is based on the latest code/scripts/data found on the ```master``` branch in the project repository.
2.	Create a branch (branch early, branch often) – corollary: do not work in branch ```master```.
3.	Create/update/delete files associated with the project.
4.	Commit the changes locally (this creates a record of the changes you made along with a comment about the purpose of the changes).
5.	Rinse and repeat steps 2 & 3 as you see fit. It can be useful to checkpoint work in progress.
6.	Push the commit(s) to _your_ repository on GitHub – this serves two purposes: it makes a backup of the work you have done and it makes it possible to share the work with other people.
7.	Rinse and repeat steps 2 through 5 as you see fit.
8.	Fetch from the project repository to see if other changes have gone in since you started working.
9.	If there are changes in the project repository, rebase _your_ work on those changes and (re-)push your work to your repository on GitHub.
10.	Create a pull request on GitHub for getting your changes into the project repository and onto the ```master``` branch.
11.	Once the pull request has been accepted and your work is on the ```master``` branch in the project repository, return to step 1.
