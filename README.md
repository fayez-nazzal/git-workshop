# Git & GitHub workshop

## Prerequisites

- Install Git: https://git-scm.com/downloads
- Install VSCode: https://code.visualstudio.com/download

## Git Add

```bash
    git add . # Stage all files in the working directory
    git add "file name" # Stage one file
    git add "folder name" # Stage a folder
```

## Git commit

```bash
    git commit -m "Message"
```

## Git Branches

Branches allow you to develop features, fix bugs, or experiment with new ideas in isolation from your main codebase.

### Basic Branch Commands
```bash
git branch  # List all local branches
git branch -a  # List all branches (local and remote)
git branch branch-name  # Create a new branch
git branch -d branch-name  # Delete a branch (safe)
git branch -D branch-name  # Force delete a branch
```

### Switching Branches
```bash
git checkout branch-name  # Switch to an existing branch
git checkout -b new-branch  # Create and switch to a new branch
git switch branch-name  # Modern command to switch branches
git switch -c new-branch  # Modern command to create and switch
```

### Branch Naming Conventions
Common branch naming patterns:
- `feature/feature-name` - For new features
- `bugfix/bug-description` - For bug fixes
- `hotfix/issue-description` - For urgent fixes
- `release/version-number` - For release preparations

### Best Practices
- Keep branches focused on a single purpose
- Regularly sync with the main branch
- Delete branches after merging
- Use descriptive names that reflect the purpose

## git push

```bash
git push origin branch-name  # Push commits to remote repository
git push -u origin branch-name  # Set upstream and push commits
git push --force  # Force push (use with caution!)
```
Pushes your committed changes to a remote repository. The remote repository is typically hosted on platforms like GitHub.

## git pull

```bash
git pull origin branch-name  # Fetch and merge changes from remote
git pull --rebase  # Pull changes and rebase local commits
```
Fetches changes from a remote repository and merges them into your current branch. It's essentially a combination of `git fetch` and `git merge`.

## git merge

```bash
git merge branch-name  # Merge specified branch into current branch
git merge --no-ff branch-name  # Create a merge commit even if fast-forward is possible
git merge --abort  # Abort the merge in case of conflicts
```
Combines changes from different branches. Common scenarios include:
- Merging feature branches into main/master
- Incorporating upstream changes into your feature branch

### Handling Merge Conflicts
If Git cannot automatically merge changes, you'll need to resolve conflicts manually:
1. Open conflicting files and look for conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)
2. Choose which changes to keep or combine them
3. Remove conflict markers
4. Stage and commit the resolved files

## GitHub Pull Requests

Pull Requests (PRs) are a GitHub feature that lets you:
- Propose changes to a repository
- Review code collaboratively
- Discuss modifications
- Ensure quality through code review

### Creating a Pull Request
1. Push your branch to GitHub
2. Navigate to the repository on GitHub
3. Click "New Pull Request"
4. Select the base and compare branches
5. Add title and description
6. Create the pull request

### Best Practices
- Keep PRs focused and reasonably sized
- Write clear descriptions
- Reference related issues
- Respond to review comments
- Keep the PR updated with the base branch

## Additional Resources
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [GitHub Pull Request Documentation](https://docs.github.com/en/pull-requests)
- [git.fayez.io](https://git.fayez.io) - Slides link
- [fayez.io](https://fayez.io) - My website
