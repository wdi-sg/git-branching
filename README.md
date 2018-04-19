# git-branching

Let's try some branching. This workflow would be as if you were working in a solo project.

You are a cat blogger.
You are writing an entry in your cat blog.
Save the blog as a commit in git.

## Setting up the Repository

- Create a new repo:

1. `mkdir catworld`
1. `cd catworld`
1. `echo "Sweet beast yowling nonstop the whole night or lie on your belly and purr when you are asleep yet scratch at fleas, meow until belly rubs, hide behind curtain when vacuum cleaner is on scratch strangers and poo on owners food unwrap toilet paper. Ears back wide eyed pooping rainbow while flying in a toasted bread costume in space this human feeds me, i should be a god yet hide head under blanket so no one can see." >> text-sample.txt`
1. `git init`
1. `git add .`
1. `git commit -m "initial commit"`


## Changes
You wrote a blog, but you are thinking it needs some edits.
You want to keep your old blog, but want to see if the new editorial direction for your blog entry is good.

* Check out a new feature branch and add another line to the file.
```
git branch new-line
git checkout new-line
```
Make the changes:

```
sublime text-sample.txt
```
```
git add .
git commit
```

Merge your changes back into master
```
git checkout master
```
Now that you are in your master branch, see the current state of the file.
```
git merge new-line
```

### You might need to set your default terminal editor:
```
export VISUAL=sublime
export EDITOR="$VISUAL"
```

### Add it to github
Create a repo named `catworld`.

#### Add the github remote to your repo
Follow the part of the instructions for adding a remote.
It will look something like: `git remote add origin https://github.com/user/repo.git`

#### Push your local changes up
Follow the part of the instructions to force push up your current repo.
```
git push -u origin master
```

#### Make changes to your file with the github.com text editor
Pull them down from github
```
git pull origin master
```

#### Push your branch to github
```
git push origin new-line
```
