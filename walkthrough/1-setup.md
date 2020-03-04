# 1. Setup

In order to contribute you need to create a GitHub Fork of this project. When you Fork a project on Github you create a copy of the repository under your personal account. You can then make contributions to your own copy without them affecting the original.

## :running: Activities

Follow along with the activities below to get yourself ready for the rest of the walkthrough.


### 1 - Fork a Source Repository and Add a collaborator

__One Team Member__

Fork the source repository:
   1. Visit https://github.com/neiloconnor/git-flow-exercise
   2. Click the "fork" button, and choose your personal GitHub account if prompted

Add a contributor:
   1. Read the Github guide on adding collaborators https://help.github.com/en/github/setting-up-and-managing-your-github-user-account/inviting-collaborators-to-a-personal-repository
   2. Add the other team member as a collaborator on your copy of the repository
   3. Make sure they accept the invitation email before proceeding

### 2 - Clone your Fork

__All Team Members__

Clone this project to your local machine. Note that this is cloning your forked copy, not the original:
```sh
$ cd Z:/my/parent/directory
$ git clone https://github.com/your-username/git-flow-exercise.git
# clone the fork repository from GitHub

$ cd repository-name
# change working directory to the cloned repository
```

View existing branches:
```sh
$ git branch
# show local branches
* master

$ git branch -r
# show remote branches
origin/HEAD -> origin/master
origin/develop
origin/master
```


### 4 - Configure Local Branches

__All Team Members__

By now you should have noticed that you do not have a local `develop` branch
```sh
$ git branch
* master
```

Checkout the `develop` branch to get a local copy:
```sh
$ git checkout develop 
```

You should now be ready to move on to the rest of the walkthrough. If you'd like to see the repository you've created on your local machine in GitHub desktop, you can add a repository by choosing a local path.


## Next

Next we will walk through the process of creating feature branches, publishing changes to GitHub, and making a request to merge changes into the source repository using a Pull Request.

[Go](2-feature-branches.md)

## Quick Links

- [Readme](../readme.md)
- [2. Feature Branches](2-feature-branches.md)
- [3. Code Review](3-code-review.md)
- [4. Fetching Latest](4-fetching-latest.md)
- [5. Hotfix](5-hotfix.md)
- [6. Release Branch](6-release-branch.md)
- [7. Release Bugs](7-release-bugs.md)
- [8. Completed Release](8-completed-release.md)
