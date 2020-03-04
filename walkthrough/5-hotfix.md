# 5. Hotfix

| Date | Phase |
| --- | --- |
|  February 5<sup>th</sup> | Hotfix |

This morning the project manager received a frantic call from the EIC of _Flavor_ magazine. The app was so successful that the writers have been inundated with emails from readers submitting their own recipes for consideration. The number of emails has been so great that their inboxes are completely useless. The magazine wants your team to remove the writers' email addresses from the app ASAP.

## :running: Activities

Start by looking at the diagram from the GitFlow article and find the hotfix. 

Follow along with the activities below to walk through the process of creating a hotfix branch, then merging the hotfix into both the `master` and `develop` branches.

### 1 - Create the Hotfix Branch

__One Team Member__

Create a branch off of `master` named `hotfix-1.0.1`:
```sh
$ git checkout master
# switch to master branch

$ git checkout -b hotfix-1.0.1
# create & switch to hotfix branch
```

Bump the patch number contained in the [VERSION](/app/VERSION) file:
```
major=1
minor=0
patch=1
```

Stage and commit your change:
```
$ git add app/VERSION
# stage changes to the version file

$ git commit -m "Bump version to 1.0.1"
```

After removing the email addresses from the main page ([/app/index.md](/app/index.md)), stage and commit the change:
```sh
$ git add app/index.md

$ git commit -m "Remove email addresses from app"
```


### 2 - Publish the Hotfix Branch and create Pull Request

Push the branch to origin (Github):

```sh
$ git push origin hotfix-1.0.1
```

Navigate to your GitHub fork and open the pull request. On the Pull Request interface, make sure that the base fork is `your-username\git-flow-exercise` and the base branch is `master`. This means that you are requesting to merge your changes into the `master` branch of your forked copy of the repository. 

We also want to merge the hotfix changes into `develop`, so create a second Pull Request making sure that the base fork is `your-username\git-flow-exercise` and the base branch is `develop`. 


### 5 - Accept Pull Requests

Open each Pull Request in the Github interface and click the green "Merge pull request" button. Once the hotfix is merged into `master` we can assume that the app is updated and the issue of writers receiving too much email is resolved.

Fetch the latest changes in master and develop branches to your local device, like you did in [4. Fetching Latest](4-fetching-latest.md).


## Next

Next we will walk through the process of cutting a new release branch.

[Go](6-release-branch.md)

## Quick Links

- [Readme](../readme.md)
- [1. Setup](1-setup.md)
- [2. Feature Branches](2-feature-branches.md)
- [3. Code Review](3-code-review.md)
- [4. Fetching Latest](4-fetching-latest.md)
- [6. Release Branch](6-release-branch.md)
- [7. Release Bugs](7-release-bugs.md)
- [8. Completed Release](8-completed-release.md)
