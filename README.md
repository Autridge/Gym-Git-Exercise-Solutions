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

## Bundle 2

### Exercise 1

```bash
    git checkout -b ft/bundle
    touch services.html
    git add services.html
    git commit -m "Adding the services page"
    git push -u origin ft/bundle-2
    https://github.com/Autridge/git-exercise/pull/new/ft/bundle-2
```

### Exercise 2

```bash
    git checkout main
    git pull
    git checkout -b ft/service-redesign
    git add services.html
    git commit -m "Added new features to the services page"
    git push -u origin ft/service-redesign
    git checkout main
    git add service.html
    git commit -m "Additional updates on the services page"
    git push -u origin main
    git checkout ft/service-redesign
    git merge main
         Auto-merging services.html
         CONFLICT (content): Merge conflict in services.html
        Automatic merge failed; fix conflicts and then commit the result.
    git checkout ft/service-redesign
    git diff
    git merge main
    git add --all
    git commit -m "Resolved Issue"
    git push
```

## Bundle 3

### Exercise 1

```bash
    git checkout -b ft/team-page
    touch team.html
    git add team.html
    git commit -m "Add team.html page with initial content"
    git push -u origin ft/team-page
    git checkout main
    git checkout -b ft/contact-page
    git checkout ft/team-page
    git log --oneline -1
    git cherry-pick f3f2138
    touch contact.html
    git add contact.html
    git commit -m "Added contact.html page with initial content"
    git push -u origin ft/contact-page
    git checkout -b ft/faq-page
    touch faq.html
    git add faq.html
    git commit -m "Added faq.html with initial content"
    git psuh -u origin ft/faq-page
    git revert f3f2138 --no-edit
    git push origin ft/faq-page
```

### Exercise 2

```bash
    git checkout -b ft/home-page-redesign
    git checkout main
    git add index.html
    git commit -m "Update homepage with new design"
    git push origin main
    git checkout ft/home-page-redesign
    git rebase main
    git add index.html
    git commit -m "Redesign homepage with modern layout and features"
    git push -u origin ft/home-page-redesign
```
