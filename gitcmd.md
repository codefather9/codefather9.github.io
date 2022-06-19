//some useful git commands

git init
git clone <url>
git status
git diff [file name]
git add [file name(s) <optional>]
git commit -m "<message for commit>"
git log [-<number optional>]
git show [commit id]
git branch 	// shows current branch with green color
git checkout -b [new branch name] 	// create a new branch from current branch and change the working branch to new branch
git checkout [branch name] 	// change branch
git branch -d [branch name] 	// delete branch, can only be done when on a different branch
git branch [new branch name] 	// creates a new branch branch but does not change the working branch
git merge [branch to merge in the current branch] 	// if you want to merge branch B changes to A branch, then checkout A and run the command 'git merge B'
git reset --hard HEAD^ 	// removes/deletes the latest commit and code changes, resets the branch to previous commit
git reset --soft [commit id] 	// removes just the commit and changes branch head to [commit id], code changes remain in staging
git restore --staged [file name] 	// removes file from staging
git restore [file name] 	// removes the changes in files
git pull 	// gets all the commits from remote repo
git push 	// pushes local commits to remote repo
git commit --ammend 	// adds the current staging changes to previous commit, after this we need to save using [ESC]wq
git push --set-upstream origin [branch name]	// push a new branch to remote and set it as upstream origin
git remote add origin [git repository url ending with .git] // push a newly initailized repo in local to remote git server