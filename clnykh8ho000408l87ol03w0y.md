---
title: "Git It Right"
datePublished: Fri Oct 20 2023 12:08:06 GMT+0000 (Coordinated Universal Time)
cuid: clnykh8ho000408l87ol03w0y
slug: git-it-right
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/wX2L8L-fGeA/upload/f574a9986456bc6c42c055d546aab965.jpeg
tags: github, version-control, git, versioning

---

## **Getting Started with Git:**

### **Understanding Version Control**

Before we dive into the world of Git, it's essential to understand the concept of version control. Version control systems (VCS) help you track and manage changes in your codebase, making collaboration and project management more efficient. Git is one of the most popular VCS, known for its speed, flexibility, and robust branching and merging capabilities.

Version control provides the following benefits:

* **History Tracking:** You can see the entire history of changes, who made them, and why they were made.
    
* **Collaboration:** Multiple developers can work on the same project simultaneously without interfering with each other.
    
* **Safety Net:** Mistakes happen, but with version control, you can always revert to a previous state of your project.
    
* **Branching:** You can create separate branches for different features or bug fixes, allowing you to work on multiple aspects of your project in parallel.
    

---

### **Installing Git**

To get started with Git, you'll need to install it on your computer. The installation process varies depending on your operating system.

**Windows:**

1. Download the Git for Windows installer from [Git for Windows](https://gitforwindows.org/).
    
2. Run the installer and follow the installation steps.
    

**MacOS:**

1. Git often comes pre-installed on Macs. Open your terminal and type `git --version` to check if it's already installed.
    
2. If not installed, you can download it from the [official website](https://git-scm.com/), or use a package manager like [Homebrew](https://brew.sh/).
    

**Linux (Ubuntu):**

Open a terminal and run the following command to install Git.

```bash
sudo apt-get install git
```

---

### **Setting Up Your First Repository**

Now that Git is installed, you're ready to create your first Git repository. A Git repository is essentially a folder that Git tracks. Here's how you can set up a new repository:

1. **Create and Navigate to Your Project Directory:** Before initializing a new Git repository, ensure that you've created and navigated to the directory or folder where you want to manage your project.
    

> If you don't specify a location, the repository will be created in the default location of your terminal or command prompt. Use the `cd` command to change directories to your desired location. For example:

```bash
cd /your_project_folder/
```

1. **Initialize a New Repository:** Open your terminal or command prompt and navigate to the folder where you want to create your new repository. Use the `git init` command to initialize a new Git repository.
    
    ```bash
    git init
    ```
    
    This creates a `.git` directory in your project folder, where Git stores all the information it needs to manage your project.
    
2. **Adding Files:** Create some files in your repository or add existing files to it. Use `git add` to stage changes for a commit.
    
    ```bash
    git add <filename>
    ```
    
    Staging means telling Git that you want to include these changes in your next commit.
    
3. **Commit Your Changes:** Once you've added your files, commit them to create a snapshot of your project. This snapshot includes all the changes you've staged with `git add`.
    
    ```bash
    git commit -m "Initial commit"
    ```
    
    Congratulations! You've now created your first Git repository and made your initial commit.
    
4. **Logging In via Browser, Creating a Repository, and Pushing Code**
    
    1. **Create a GitHub Account:** If you don't already have a GitHub account, sign up for one at [GitHub](https://github.com/).
        
    2. **Log In to GitHub:** Ensure that you are logged in to your GitHub account in your web browser. If not, log in.
        
    3. **Create a New Repository:** If you don't have a repository to push your code to, you can create one directly from the GitHub website. Here's how:
        
        * Click the "+" (plus) sign in the upper right corner of the GitHub homepage.
            
        * Select "New repository."
            
        * Follow the prompts to create a new repository. You can set a name, description, visibility (public or private), and choose to initialize it with a README or .gitignore file.
            
5. **Adding a Remote Repository:** To push your code to the GitHub repository you created or to an existing one, add a reference to the remote repository. Replace `<repository-url>` with the URL of your GitHub repository:
    
    ```bash
    git remote add origin <repository-url>
    ```
    
    The term "origin" is a common convention for the default remote repository.
    
6. **Push Your Code:** Now that you've added the remote, you can push your code to GitHub:
    
    ```bash
    git push -u origin main
    ```
    
    * `-u` sets up tracking, so you can use `git push` and `git pull` without specifying the remote and branch every time.
        
    * Replace `main` with the name of the branch you want to push (e.g., `master` or `main` are common names for the main branch).
        
7. **GitHub Login Prompt:** When you execute `git push`, if you haven't logged in to GitHub via the web browser, Git will prompt you to do so. It will open a new browser window and ask you to log in with your GitHub username and password.
    
8. **Authorize the Access:** After logging in, you may be prompted to authorize access for Git to connect to your GitHub account. This step is essential for authentication.
    
9. **Return to the Terminal:** After authorizing access in the browser, return to your terminal or command prompt. The push operation will proceed automatically.
    

---

## **Next Steps: Working with Git After Your Initial Commit**

You'll typically continue working on your project, making changes, and committing them as needed. Here's what you can do next:

1. **Continue Working on Your Code:** You'll likely continue writing, modifying, and improving your code as your project progresses.
    
2. **Stage and Commit Changes:** Whenever you make changes that you want to save, you should stage them using `git add` and then commit them using `git commit`. This creates a new snapshot of your project with the latest changes.
    
    ```bash
    git add <filename>
    git commit -m "Description of changes"
    ```
    
3. **Create and Switch Branches:** If you're working on different features or fixes simultaneously, you can create new branches using `git branch` and switch between them using `git checkout`.
    
    ```bash
    git branch feature-branch  # Create a new branch
    git checkout feature-branch  # Switch to the new branch
    ```
    
4. **Merge Branches:** When a feature or fix is complete, you can merge the changes from your feature branch back into the main branch (usually `main` or `master`) using `git merge`.
    
    ```bash
    git checkout main  # Switch to the main branch
    git merge feature-branch  # Merge changes from the feature branch
    ```
    
5. **View the Commit History:** You can use `git log` to view the history of commits in your project. This is helpful for tracking changes and understanding who made them.
    
    ```bash
    git log
    ```
    
6. **Collaboration:** If you're working with others on the project, you can push your changes to a remote repository, collaborate through pull requests, and pull their changes into your local repository. This involves using remote repository hosting platforms like GitHub, GitLab, or Bitbucket.
    
    ```bash
    git push origin main  # Push your changes to the remote repository
    ```
    
7. **Resolving Merge Conflicts:** Occasionally, when merging branches, you may encounter merge conflicts if two people have made changes to the same part of a file. You'll need to resolve these conflicts manually.
    
    ```bash
    # After resolving conflicts, commit the changes
    git add <filename>
    git commit -m "Resolved merge conflict"
    ```
    
8. **Tagging and Releases:** You can use tags to mark specific commits, often to indicate releases or important milestones in your project.
    
    ```bash
    git tag v1.0  # Create a tag for version 1.0
    git push --tags  # Push tags to the remote repository
    ```
    

Remember, Git is a powerful tool with many features, and your workflow will evolve as your project grows and as you gain experience. Continue using `git status`, `git diff`, and other Git commands to keep track of your project and manage your code effectively.

---

## Commonly used Git Commands:

| Git Command | Explanation |
| --- | --- |
| `git init` | Initializes a new Git repository. |
| `git clone <repository URL>` | Creates a copy of a remote repository locally. |
| `git add <file>` | Stages changes for the next commit. |
| `git commit -m "<message>"` | Records staged changes in a new commit. |
| `git status` | Shows the status of your working directory. |
| `git log` | Displays a history of commits. |
| `git pull` | Fetches changes from a remote repository and merges them into the current branch. |
| `git push` | Pushes local changes to a remote repository. |
| `git branch` | Lists all local branches. |
| `git checkout <branch>` | Switches to a different branch. |
| `git merge <branch>` | Merges changes from one branch into the current branch. |
| `git diff` | Shows the differences between the working directory and the last commit. |
| `git remote -v` | Lists remote repositories and their URLs. |
| `git fetch` | Retrieves changes from a remote repository without merging. |
| `git reset <file>` | Unstages changes for a specific file. |
| `git reset <commit>` | Moves the branch pointer to a specific commit. |
| `git stash` | Temporarily saves changes without committing. |
| `git tag <tagname>` | Creates a new tag for a specific commit. |
| `git pull --rebase` | Fetches changes and applies local commits on top of the fetched changes. |
| `git remote add <name> <URL>` | Adds a new remote repository with a name and URL. |
| `git push --tags` | Pushes tags to a remote repository. |
| `git rebase <branch>` | Applies the changes from one branch on top of another. |
| `git cherry-pick <commit>` | Applies a specific commit to the current branch. |
| `git clean -n` | Shows a preview of untracked files to be deleted. |
| `git clean -f` | Removes untracked files from the working directory. |

These are some of the most commonly used Git commands. Note that Git has many more commands and options, but these should cover most basic version control and collaboration needs.

---

# Error Handling:

### Author identity unknown.

```bash
git config --global user.email "your@email"
```