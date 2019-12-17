[Home](https://zx37.github.io/learning-journal/)

# GitHub Workflow

---

**Cloning Remote Repos**

Cloning a remote repo on GitHub allows you to work locally on code stored in the cloud. The initial cloning process downloads the repo locally, and ties it to the GitHub version. This allows you to sync any edits made locally back to the GitHub repo.

Fetching (`git fetch repo-name`) will pull the most recent data about a repo, allowing your local host to compare the local and GitHub repos. You can view any differences or additional info using `git status`.

---

**Adding, Committing, and Pushing Changes**

There are three necessary steps to merge changes back into the GitHub repo.
- First, the changed files must be staged to commit, using the command `git add filename` (or `git add *` to add all files).
- Next all added files will be committed, preferably with an explanatory message, using the command `git commit -m "message"`. - Finally, committed changes are merged from the local branch to the remote repo using the command `git push origin master`, where "origin" is the remote repository, and "master" is the local branch (both GitHub default).

---

**Merge Conflicts**

When files to be merged have multiple changes coming from different sources, there may be merge conflicts. Often (especially with proper planning), these changes do not interfere with eachother and git will automatically merge them cleanly. However, sometimes changes do conflict in a way where git cannot determine which change should be used. In this case, changes will have to be reviewed, and merged based on human arbitration. This can be done within most dvelopment-oriented text editors.
