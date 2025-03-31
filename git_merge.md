# How to Merge a Branch into the Main Branch

This guide explains how to merge your current branch into the `main` branch using Git.

## Steps to Merge a Branch into `main`

### 1. Switch to the `main` Branch
First, ensure you are on the `main` branch where you want to merge the changes.


```bash
git checkout main
```

### 2. Switch to the `main` branch
Change to the `main` branch using this command:

   ```bash
   git pull origin main
   ```

### 3. Merge your current branch into `main`
Combine the changes from your branch into `main.` Replace  with your branch name:

```bash
git merge <current-branch>
