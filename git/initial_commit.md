# Initial Commit to Github
---

## 1. Prerequisites
- install Git:
Make sure Git is installed. Open your terminal and type:
```bash
git --version
```
If Git isn't installed, download it.

## 2. Initialize Git in Your Local Project
- Open Your Project
    - Start VS Code and open the folder containing your project.
- Open the Source Control panel
    - Click the Source Control icon on the sidebar (or press Ctrl+Shift+G).
- Initialize the Repository:
    - If your project isn't already a Git repository, click Initialize Repository. This command created a hidden .git folder in your project, enabling Git version tracking.
 
## 3. Create a Repository on Github
- Log in to GitHub
    -Go to GitHub and sign in.
- Create a New Repository:
    - Click on the New repository button (or navigate to github.com/new).
    - Fill in the repository Name, Description (optional), and decide whether it will be Public or Private.
    - Tip: Leave “Initialize this repository with a README” unchecked if you plan to push your existing project; this avoids potential merge conflicts during the first push.
 
## 4. Connect Your VS Code Project to GitHub
- Open the Integrated Terminal:
    - In VS Code, open the terminal by pressing Ctrl+.
- Add the GitHub Remote:
    - Link your local repository to the GitHub repository by adding a remote. Replace  `your-username` and `your-repo` with your details:
```bash
git remote add origin https://github.com/your-username/your-repo.git
```
Verify the connection with:
```bash
git remote -v
```

## 5. Commit and Push your Code
- Stage Your Changes:
    - ```bash
      git add .
      ```
- Commit Your Code:
    - ```bash
      git commit -m "initial commit"
      ```
- Push to GitHub:
    - ```bash
      git push -u origin main
      ```



