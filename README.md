# Git Practical Exam
##  1) Make example of pull request and two branch merge event.

- Created an empty repository on GitHub.
- Cloned the repository.
- Created a html file and pushed in the remote branch.
- Create a new branch named pr-merge-task.
- Created a CSS file and linked it to HTML file in the pr-merge-task branch.
- Pushed it to the remote branch.
```git
    git push origin pr-merge-task
```
- Opened GitHub.com and created a pull request.
- There were no conflicts between two branches.
- Merged the pull request.
## 2) Try to rebase feature branch with master branch

- Created a branch named rebase-task.
- Created an empty JavaScript file.
- Replaced the text of the h1 tag using JavaScript.
- Made a commit.
- Rebased the branch to main branch.
```git
    git rebase rebase-task
```
- pushed the main branch to remote branch.
```git
    git push origin main
```
## 3) Change commit message

- Created a new branch named change-commit-msg-task
- Craeted a about.html file.
- Added a paragraph with dummy data in about.html file.
- Made commit with message "Added a paragraph with dummy data in about.html file"
- Then in terminal ran the command given below
```git
    git commit --amend
```
- Then the vim editor was opened.
- Changed the commit message to "Added a p tag in about.html file"
- Then closed the vim editor with escape key and with
```vim
    :wq
```
- The commit message was changed.
## 4) Pick some commits from feature branch to master branch

- Created a new branch named cherry-pick-task
- Created a contact.html file and made a commit
- Added email address in the contact.html file and made a commit
- logged all the commit of cherry-pick-task branch and copied the commit id of the first commit
- Checked out to the main branch and ran the command
```git
    git cherry-pick [commit id]
```
- The commit was picked to the main branch from cherry-pick-task branch
## 5) Remove some commit from feature branch.

- Created a new branch named remove-commit-task
- Created a file named blog.html and made a commit
- Added some dummy links for blogs in blog.html and made a commit
- Then ran a command in command line
```git
    git rebase -i HEAD~2
``` 
- This command will open text editor with last to commits, Like below
![Terminal Image](https://simformsolutionspvtltd-my.sharepoint.com/:i:/r/personal/munir_v_simformsolutions_com/Documents/Git%20Practical%20Exam/Screenshot%202023-03-01%20at%204.38.15%20PM.png?csf=1&web=1&e=OLHg4o)
- Now put "drop" instead of "pick" in which commit we want to remove
- Exit the text editor
- The commit has been removed