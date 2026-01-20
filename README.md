# 🧩 Essential Git Commands

## 🏁 Initialization and status

- **git init**: Creates a new Git repository in the current directory.
- **git status**: Shows the working tree status (modified, staged, untracked files, ...).

## ➕ Add and confirm changes

- **git add `<file>`**: Adds the specified file contents to the staging area.
- **git add `.`**: Adds all changes in the current directory (new, modified, and deleted files) to the staging area.
- **git commit -m "message"**: Records a snapshot of the staged changes with a descriptive message.

## 🔍 History and logs

- **git log --graph --oneline --decorate --all**: Displays the commit history in a compact, graphical format.
- **git reflog**: Shows the history of updates to HEAD and branch references (commits, resets, checkouts, ...).

## 🌿 Branches

- **git branch**: Lists local branches.
- **git branch `<name>`**: Creates a new branch.
- **git checkout `<name>`**: Switches to an existing branch.
- **git checkout -b `<name>`**: Creates a new branch and switches to it.
- **git switch `<name>`**: Switches to an existing branch (recommended alternative to checkout).
- **git branch -d `<name>`**: Deletes a local branch if it has been fully merged.
- **git branch -D `<name>`**: Forces deletion of a local branch, even if it is not merged.

## 🔗 Merging and synchronizing

- **git merge `<branch>`**: Merges the specified branch into the current branch.
- **git rebase `<branch>`**: Reapplies commits on top of another base branch, creating a linear history.

## 📦 Synchronization with remote

- **git remote add origin `<url>`**: Adds a remote named origin pointing to the given URL.
- **git remote set-url origin `<url>`**: Changes the URL of the origin remote.
- **git remote show origin**: Shows information about the origin remote.
- **git fetch**: Downloads objects and refs from the remote without modifying the working tree.
- **git pull**: Fetches from the remote and integrates changes into the current branch (merge or rebase).
- **git push**: Uploads local commits to the configured remote branch.
- **git fetch --all --prune --tags**: Fetches all remotes, removes obsolete remote-tracking references, and updates tags.
- **git remote update origin --prune**: Fetches updates from origin and removes deleted remote-tracking branches.

## 🧳 Stash (temporary changes)

- **git stash**: Saves local modifications away and reverts the working tree to match HEAD.
- **git stash list**: Lists all stashed change sets.
- **git stash pop**: Applies the most recent stash and removes it from the stash list.
- **git stash apply stash@{n}**: Applies a specific stash without removing it from the list.
- **git stash drop**: Removes the most recent stash.
- **git stash clear**: Removes all stashed entries.

## 🧨 Revert and recover

- **git reset `<file>`**: Unstages the specified file while keeping local changes (equivalent to git reset HEAD `<file>`).
- **git reset --hard `<hash>`**: Resets HEAD, index, and working tree to the specified commit, discarding changes.
- **git checkout -- `<file>`**: Restores the file in the working tree to the last committed state.
- **git revert `<hash>`**: Creates a new commit that undoes the changes introduced by the specified commit.

## 🤝 Collaboration and contributions

- **git clone `<url>`**: Creates a local copy of a remote repository.

## 💡 Aliases and productivity

- **git config --global alias.st "status -sb"**: Creates a short alias for a concise status output.
- **git config --global alias.lg "log --oneline --graph --decorate --all"**: Creates an alias for a visual commit history.

## 🏷️ Tags

- **git tag `<name>`**: Creates a lightweight tag pointing to the current commit.
- **git tag -a `<name>` -m "message"**: Creates an annotated tag with a message (recommended).
- **git push origin --tags**: Pushes all local tags to the remote repository.

---

✨ *Quick reference Git cheat sheet, aligned with official Git documentation.*
