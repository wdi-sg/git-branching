# Repo Collaboration

#### Add a collaborator

Add a person as a collaborator to your github project.

- open up your repo page on github
- click to the `settings` tab
- on the right-hand side-bar click `Collaborators & teams`
- add your partner to your project

#### As a collaborator

Checkout someone else's repo and make changes on a branch. Push those changes.

- click on the email to accept the invitation
- go to that repo (not the original one, not *your own* forked repo)
- click the link button to copy the repo url
- run the `git clone` command in your terminal (it must **not** be in a folder that already has a repo with the same name)
- `cd` into the folder created by `git clone` and create a branch `git checkout -b my-branch`
- make and commit some changes
- `git push` thopse changes up to github
- make a pull request for the branch you just created

