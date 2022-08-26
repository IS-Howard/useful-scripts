# Easy git commands

* basic
```Shell
git init
```
```Shell
git add .
git add -A
```
```Shell
git status
git log
```
```Shell
git commit -m "~~~"
```
```Shell
git remote add origin https:/github-site
git remote
git push -u origin main //set default
git push
```
```Shell
//cancel add
git reset -- <filename>
```
```Shell
//discard change (reset first)
git checkout -- <filename>
```
```Shell
//undo last commit
git reset -- HEAD~1
```

* branch
```Shell
git checkout -b <new branch>
```
```Shell
git branch
git branch -a
// include remote
```
```Shell
git push -u origin HEAD
// HEAD : last commit on current branch 
```

* merge - pull request
```Shell
//switch to base
git switch main

//update main
git pull

git switch <branch>

git rebase main

// edit conflict manually

// force push (not recommend)
git push -f

//on github => create new request => merge

//delete branch
git branch -d <branch>
```

* merge - git merge
```Shell
git merge <branch>

// update
git pull --rebase

// edit conflict manually

git commit

git push
```
