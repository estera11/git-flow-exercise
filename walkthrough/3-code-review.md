# 3. Code Review

| Date | Phase |
| --- | --- |
|  February 2<sup>nd</sup> | Development |

Now that all of the mods for the next release have been made, it is time to review and get code merged.

## :running: Activities

Follow along with the activities below to walk through the process of reviewing and merging a Pull Request.

### 1 - Review a Pull Request

__All Team Members__

Navigate to the source repository on GitHub, click the "Pull Requests" tab, and click on the Pull Request opened by your team mate.

Review the following things:

1. Verify that the user is requesting to merge their feature branch into the `develop` branch.
2. Check to see if there is any important information on the Conversation tab.
3. Check the Commits tab to get a high-level view of the individual changes that were made.
4. Verify that the changes on the Files Changed tab look correct to you.
5. Do the commit messages clearly describe what was committed?

If anything looks wrong, please make a quick comment outlining the issue. If there is a specific line of code, you can comment directly on the line from the Files Changed tab. 

In a real-world scenario the author of the changes would go back and make amendments based on the feedback, but for the purposes of this exercise we'll just take the feedback as a lesson what we can do better in future.

If the user is merging into the correct branch make a quick comment indicating that you believe the code is ready to be merged.


### 2 - Accept Pull Requests

Open each Pull Requests and click the green "Merge pull request" button. Assuming there are no merge conflicts, GitHub will automatically merge the code into the `develop` branch. If there are merge conflicts, for this exercise, close the pull request using the "Close pull request" button at the bottom.

In practice, merge conflicts should be corrected by the team member requesting to merge changes. Sometimes this is not feasible and a maintainer may have to merge the changes manually.

## Next

Next we will walk through the process of fetching the latest changes locally.

[Go](4-fetching-latest.md)

## Quick Links

- [Readme](../readme.md)
- [1. Setup](1-setup.md)
- [2. Feature Branches](2-feature-branches.md)
- [4. Fetching Latest](4-fetching-latest.md)
- [5. Hotfix](5-hotfix.md)
- [6. Release Branch](6-release-branch.md)
- [7. Release Bugs](7-release-bugs.md)
- [8. Completed Release](8-completed-release.md)
