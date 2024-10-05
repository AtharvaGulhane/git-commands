# Git & GitHub Learning Roadmap

This roadmap provides a step-by-step guide to learning and using Git commands along with GitHub. Each section introduces essential commands with examples.

---

## 1. Initial Setup

### 1.1 Configure Git

Before using Git, configure your username and email. These details will be attached to your commits.

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Check your configuration:

```bash
git config --list
```

---

## 2. Creating or Cloning a Repository

### 2.1 Create a New Repository

```bash
git init
```

### 2.2 Clone an Existing Repository

To clone a repository from GitHub, use:

```bash
git clone https://github.com/username/repository.git
```

---

## 3. Basic Workflow: Add, Commit, Push

### 3.1 Add Files to Staging Area

After modifying or adding files, you can stage them for commit:

```bash
git add filename
# Add all files
git add .
```

### 3.2 Commit Changes

Commit the changes with a meaningful message:

```bash
git commit -m "Your commit message"
```

### 3.3 Push to GitHub

To send your changes to GitHub, use:

```bash
git push origin branch_name
```

---

## 4. Branching

### 4.1 Create a New Branch

Branching allows you to work on different versions of your project simultaneously.

```bash
git branch new_feature
```

### 4.2 Switch Branches

```bash
git checkout new_feature
```

### 4.3 Create and Switch to a New Branch

```bash
git checkout -b new_feature
```

### 4.4 List All Branches

```bash
git branch
```

---

## 5. Merging & Pull Requests

### 5.1 Merge Branches

To merge a feature branch into the main branch:

```bash
git checkout main
git merge new_feature
```

### 5.2 Delete a Branch After Merging

```bash
git branch -d new_feature
```

### 5.3 Create a Pull Request

To merge code through GitHub, push your branch and create a pull request from the repository’s GitHub page.

---

## 6. Collaborating with Others

### 6.1 Fetch and Pull Changes from GitHub

Fetch the latest changes without merging:

```bash
git fetch
```

Pull changes and merge them:

```bash
git pull origin main
```

---

## 7. Undoing Changes

### 7.1 Unstage a File

If you added a file to the staging area but want to remove it:

```bash
git reset filename
```

### 7.2 Revert the Last Commit

```bash
git revert HEAD
```

### 7.3 Discard Changes in a File

```bash
git checkout -- filename
```

---

## 8. Advanced Git

### 8.1 Rebase

Rebase is used to integrate changes from one branch to another:

```bash
git rebase branch_name
```

### 8.2 Squash Commits

Squash multiple commits into one:

```bash
git rebase -i HEAD~n
# Replace "pick" with "squash" for commits to combine
```

---

## 9. GitHub Authentication (SSH Keys)

### 9.1 Set Up SSH

Generate SSH keys for GitHub authentication:

```bash
ssh-keygen -t rsa -b 4096 -C "your.email@example.com"
```

Add the SSH key to your GitHub account by copying the key content from:

```bash
cat ~/.ssh/id_rsa.pub
```

Add it to GitHub under `Settings > SSH and GPG keys`.

### 9.2 Clone with SSH

After setting up SSH, clone repositories using:

```bash
git clone git@github.com:username/repository.git
```

---

## 10. GitHub Pages (For Hosting)

### 10.1 Deploy Your Project Using GitHub Pages

Create a branch named `gh-pages`:

```bash
git checkout -b gh-pages
git push origin gh-pages
```

Enable GitHub Pages in the repository’s settings.

---

## 11. Working with Submodules

### 11.1 Add a Submodule

```bash
git submodule add https://github.com/username/repository.git path_to_submodule
```

### 11.2 Update Submodules

```bash
git submodule update --remote
```

---

## 12. Git Tags

### 12.1 Create a Tag

```bash
git tag -a v1.0 -m "Version 1.0 release"
```

### 12.2 Push Tags to GitHub

```bash
git push origin --tags
```

---

## 13. Dealing with Conflicts

### 13.1 Resolve Merge Conflicts

When you encounter conflicts during a merge, Git will mark the conflicts in the affected files. Manually resolve them and then:

```bash
git add conflict_file
git commit
```

---

This roadmap provides a starting point for learning Git & GitHub. Follow the steps in order, and use the commands as examples to gain hands-on experience.
```
