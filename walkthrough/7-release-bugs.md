# 7. Release Bugs

| Date | Phase |
| --- | --- |
|  February 24<sup>th</sup> | Release |

The magazine is happy with the work that has been done, but has asked that the recipes picked for january appear on the home screen under the heading "Last Month's Favorites". Oh and by the way, John Lemon has been fired so please would you remove him from the application.

## :running: Activities

Follow along with the activities below to walk through the process of fixing issues in the release branch.

### 1 - Fix Issues in Feature Branches

__All Team Members__

Fetch the latest from origin and create a local tracking branch for the release:

```sh
$ git fetch origin
# fetch latest from origin

$ git checkout release-1.1.0
# checkout the release branch
```

Each team member should address one issue.

- Developer 1:
    1. Create a feature branch off of `release-1.1.0` named `last-months-favorites`.
    2. Commit the following changes to the feature branch:
        1. Create a section in [`/app/index.md`](/app/index.md) titled "Last Month's Favorites".
        2. Copy the text that was published last release and paste under "Last Month's Favorites". Be sure not to include John Lemon.

- Developer 2:
    1. Create a feature branch off of `release-1.1.0` named `remove-john-lemon`.
    2. Commit the following changes to the feature branch:
        1. Delete the file `/app/writer/john-lemon.md`.
        2. Remove references to John Lemon from [`/app/index.md`](/app/index.md)



### 2 - Publish & Request to Merge Feature Branches

__Developers__

The two developers from the last step should now publish their feature branches to GitHub and open up Pull Requests to merge into the `release-1.1.0` branch in the source repository:



### 3 - Merge Feature Requests into Release Branch

__Maintainers__

Review the developer Pull Requests and merge them into `release-1.1.0`.

## Next

Finally, we will walk through the process of completing a release: merging into master, back down into develop, and creating a GitHub release tag.

[Go](8-completed-release.md)

## Quick Links

- [Readme](../readme.md)
- [1. Setup](1-setup.md)
- [2. Feature Branches](2-feature-branches.md)
- [3. Code Review](3-code-review.md)
- [4. Fetching Latest](4-fetching-latest.md)
- [5. Hotfix](5-hotfix.md)
- [6. Release Branch](6-release-branch.md)
- [8. Completed Release](8-completed-release.md)
