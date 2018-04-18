# git-branching

Let's try some branching in rails. This workflow would be as if you were working in a solo project.

## Setting up the Repository

- Create a new repo:

1. `mkdir catworld`
1. `cd catworld`
1. `rails new ./ -d postgresql`
1. `bundle install`
1. `git add .`
1. `git commit -m "initial commit"`
1. `git remote add origin <the_url_to_your_repo>`
1. `git push -u origin master`

## Changes


* Check out a new feature branch and create a cats model.
```
git checkout -b new-model
```
Make the changes:

```
rails g model cat name weight:integer
rails db:create
rails db:migrate
```

Merge your changes back into master
```
git checkout master
git merge new-model
```
