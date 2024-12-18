# Git Exercises

## Bundle 1 

### Exercise 1
```bash

git init

echo "text file" > file1.txt 

git status

git branch -M master

git branch -M main

git add .

git commit -m "add file1"

git remote add origin https://{MY TOKEN}@github.com/MohamDahALU/b1e1.git

git push origin main

git checkout -b dev

git push origin dev

git checkout -b test

git push origin test

git checkout dev

git branch -d test

git push origin --delete test

```

### Exercise 2
```bash
touch home.html

git stash -u

echo "pretend this is html" > about.html

git stash -u

echo "this is html too" > team.html

git stash -u

git stash pop stash@{1}

git stash pop stash@{1}

git add .

git commit -m "add about and home"

git push origin dev

git stash pop

git add team.html

git reset --hard
```

## Bundle 2

### Exercise 1
```bash
git branch ft/bundle-2 

git switch ft/bundle-2 

touch services.html

git add services.html

git commit -m "add services.html"

git push origin ft/bundle-2

```
