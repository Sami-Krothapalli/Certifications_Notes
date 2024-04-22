---
sticker: lucide//git-branch
---
# Branches

Idea: make changes to the codebase without affecting the entire project

- Safe way to experiment with features or fixes

> [!tip]
> Alternatively you can create a new branch and check it out by using git doing:
> `git checkout -b newBranchName`

# Commits

> [!Definition]
> A change made to one or more files on a branch that has a unique ID

A commit is tracked along with the time and contributor.
- Provides a clear audit trail for anyone reviewing the history of a file or linked item

In a git repo a file can exist in several valid states as it goes through version control:
### States:
- **Untracked**: An initial state of a file when it is not yet part of the git repo (Git is unaware of its existence)
- **Tracked**: A tracked file are files that git monitors
	- **Unmodified:** File is tracked but has not been modified since the last commit
	- **Modified:** The fi.e has been changed since the last commit, but changes arent staged yet for next commit
	- **Committed:** File is in the repository database> it represents the latest committed version of the file
# Pull Requests:

> [!Definition ]
> A mechanism used to signal that the commits from one branch are ready to be merged into another branch

A team member submitting a pull request has one or more reviewers to verify the code and approve the merge. They comment on changes, add their own or use the pull request itself for further discussion

If changes have been approved the PR source branch (Compare Branch) is merged into the base branch 
# GitHub Flow
- A light weight workflow that allows for safe experimentation to test ideas and collaborate with the team by using branching, pr, and merging

### Steps for Git Flow:
1. Create a branch, so that the changes, features and fixes you create do not affect the main branch.
2. Make you're changes (deploy changes to your feature branch before merging into the main branch. => Will ensure the changes are valid in a production environment)
3. Create a pull request to ask collaborators for feedback. Pull Request Reviews are valuable that some repo's need to approve review before pull requests can be merged.
4. Reviewing and implementing the feedback from your collaborators.
5. Merge the pull request once its approved into the main branch
6. delete the feature branch created. Deleting your branch signals your work on the branch is completed and will prevent you or others from using old branches.