## Step 1: Creating a New Branch
Before you start working on a new feature or fix, you should create a new branch. This keeps your changes organized and separate from the main codebase until they’re ready to be merged.

```bash
git checkout main  # Start from the main branch
git pull origin main  # Ensure you have the latest changes
git checkout -b your-branch-name  # Create and switch to your new branch for e.g git checkout -b Rabina_development
```
### Step 2: Making Changes and Committing
After you’ve made your changes, you’ll want to save them in your local repository. This involves staging the changes and then committing them with a clear message.

```bash
git add .  # Stages all your changes for commit
git commit -m "Describe the changes you made"

```

### Step 3: Pushing Changes to GitHub
Once you’ve committed your changes locally, you need to push them to the remote repository (GitHub). This makes them available to other team members.

```bash
git push origin your-branch-name  # Pushes your branch and changes to GitHub
```

Step 4: Creating a Pull Request
Go to the GitHub repository in your web browser. You’ll see an option to 'Compare & pull request' for your newly pushed branch. Click on it, review your changes, and then submit the pull request (PR) for review.

### Step 5: Reviewing and Merging the Pull Request
After your pull request (PR) is submitted, it should be reviewed by another developer. This ensures that someone else has looked over the changes, potentially catching errors or suggesting improvements that the original developer may have missed.

If the PR is approved, the best practice is for the reviewer, not the person who made the PR, to merge it into the main branch. This approach reinforces the principle of peer review and adds an extra layer of quality control before changes are incorporated into the main codebase. Merging is often done through the GitHub interface.

### Step 6: Keeping Your Branch Up-to-Date
To avoid conflicts, it’s a good practice to keep your branch up-to-date with the main branch. This involves pulling the latest changes from main into your branch.

```bash
git checkout main  # Switch to the main branch
git pull origin main  # Pull the latest updates
git checkout your-branch-name  # Go back to your branch
git merge main  # Merge changes from main into your branch
```
### Step 7: Resolving Merge Conflicts
If there are conflicts during the merge, Git will ask you to resolve them. After resolving any conflicts, add the resolved files, and then commit the merge.

```bash
git add .  # After resolving conflicts, stage the resolved files
git commit -m "Resolved conflicts while merging main into your-branch-name"

```

### Step 8: Push Updated Branch
After merging and resolving conflicts, push the updated branch back to GitHub.

```bash
git push origin your-branch-name
```
By following these steps, you’ll be able to manage your changes efficiently and keep your branch aligned with the main codebase. Let me know if you need further clarification on any of these steps!
