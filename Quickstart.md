

## Git basics 

1. Initialize the repository: The very first step in git is git initialization. It is done using the git init command. The command creates a new .git subdirectory in your current working directory
```shell
git init
```

2. Clone an existing repository: If instead you want to start by collaborating on an existing project, you can use git clone followed by the URL of the project you want to start working on.
```shell
git clone https://github.com/user/repo.git
```
3. Status check: Before making any changes, you would like to check the status of your files. This is done using git status.
```shell
git status
```
4. Add files: Once you've made some changes or created new files, you want to add them to what will be your next commit. This can be done with git add.
```shell
git add filename.ext
git add .
```
5. Commit changes: After you added, you stage those changes. Now, to capture the state of the project at this point in time, use git commit, followed by a message that describes what you've changed.
```shell
 git commit -m "commit message"
```
6. Connect with remote repository: Now, you need to connect your local repository to a remote server (eg, GitHub) using the git remote add command.
```shell
git remote add origin https://github.com/user/repo.git
```
7. Push changes to the Remote Repository: If you are connected with the remote server and want to share your developments with your team members or to keep your code safe and accessible from other places, you push your changes using git push.
```shell
git push origin branch_name
```
8. Pull changes from Remote Repository: If you are working in a team, then you need to pull changes from the remote server to keep your repository updated using git pull.ù
```shell
git pull origin branch_name
```

9. Branching: When you want to add a new feature or fix a bug—no matter how big or how small—you spawn a new branch to encapsulate your changes using git branch and git checkout -b.
```shell
git branch
git checkout -b branch_name
```
10. Merging: Merging is Git's way of putting a forked history back together again. The git merge command lets you take the contents of another branch (or any committed snapshot) and combine it with where you currently are (another branch or commit).
```shell
git merge branch_name
```
11. Resolving conflicts: If the same part of the same file is modified in two different branches that you're trying to merge together, Git won't be able to merge them cleanly. So it will mark the file as having a conflict - which you'll have to resolve manually.
12. Reverting and resetting: If you made a mistake and need to undo commits, you may use git revert or git reset.
```shell
git revert commit_hash
git reset commit_hash
```
Remember to replace `branch_name` with the appropriate branch name and  `filename.ext` with the appropriate filename and extension