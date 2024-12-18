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

### Exercise 2
```bash
git checkout main

git pull origin main

git checkout -b ft/service-redesign

git add services.html

git commit -m "changed services.html"

git push origin ft/service-redesign

git switch main

git add services.html 

git commit -m "changed services"

git push origin main

git switch ft/service-redesign

git difftool main

git switch main

git merge ft/service-redesign

git commit -m "merged with ft/service-redesign"

git push origin main
```

## Bundle 3

### Exercise 1
```bash
git branch ft/team-page

git switch ft/team-page

touch team.html

git add team.html

git commit -m "added team.html"

git push origin ft/team-page

git checkout main

git branch ft/contact-page

git switch ft/team-page

git log --oneline

git checkout ft/contact-page 

git cherry-pick 6dfe41a

git add team.html 

git commit -m "changed team.html"

git push origin ft/contact-page 

git checkout -b ft/faq-page

touch faq.html

git add faq.html 

git commit -m "add faq.html"

git push origin ft/faq-page

git switch ft/contact-page

git log

git switch ft/faq-page

git revert 05747e1

git commit -m "revert to one commit before ft/contact-page HEAD"

git push origin ft/faq-page
```

### Exercise 2
```bash
git branch ft/home-page-redesign

git switch main

git add file1.txt 

git switch ft/home-page-redesign

git rebase main

git add home.html

git commit -m "change home.html"

git push origin ft/home-page-redesign
```