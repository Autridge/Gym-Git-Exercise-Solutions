# Git Exercise

## Bundle 1

### Exercise 1

```bash
git init
touch index.html
git branch -m main master
git branch -m master main
git add index.html
git commit -m "Initial Commit"
git push https://github.com/Autridge/git-exercise main
git checkout -b dev
git checkout -b test
git checkout dev
git branch -d test
```

### Exercise 2

```bash
    git checkout dev
    touch home.html
    git add home.html
    git stash
    touch about.html
    git add about.html
    git stash
    touch team.html
    git add team.html
    git stash
    git stash pop
    git stash pop 'stash{0}'
    git add --all
    git commit -m "Adding the about and home pages"
    git stash pop
    git reset --hard
```
