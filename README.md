# Git Structure
Working Tree	Staging Area	Repository
|-> main.py     git add —>	            git commit —>	
|-> recipe.txt		
|-> .git		

## Working Tree
- Holds the current checked-out version of the project's files
- Contains the content of the latest commit
- Plus, any new changes made locally

## Staging area, Index
- Place where changes are stored before being committed
- Allows users to “stage” changes to be tested, modified, and/or combined before committing
- Ensures all changes from multiple developers are consistent and complete

## Commits
- Atomic (very small) changes
- Different conventions, e.g. Jira Ticket ID

## Repository
- Stores data such as source code
- Centralised location to share resources
- Allows for collaboration and version control

## Branches
- Copy of files that serves as a repository for changes
- For developing different features in isolation
- Merging back to main branch when complete
- Be ahead of main branch
- Update branch by merging main into branch: git pull origin main

## Parents
Every commit has two parent references 
    - One for the previous commit 
    - One for commits that have been merged in 
Examining the relationship between these parent references allows you to identify ancestry and branching history.
￼
## Merges
- A + B = ?
- Merge requests less than 24 hours
- Incremental (small) changes, preferably 
- Refactoring and changing in separate branches
- Pull request - attempt to merge into main branch 
    - Updating by rebasing or merging

## Pull request
- Method of submitting proposed changes for review
- Developer submits their changes to the project maintainer
- Review then accept or reject proposed changes

# Hashes in Git functionality
Git relies heavily on hashing when it comes to tracking data. It creates a hash of each commit, an MD5 hash that functions as an identifier for that particular commit ID. It also allows Git to identify any file changes in that particular commit. It also uses these hashes to link objects, such as commits and branches, and to track a repository’s history.