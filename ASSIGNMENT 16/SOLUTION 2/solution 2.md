# SOLUTION 

## Git Workflow 
The Git workflow involves the use of three main components: the working directory, the staging area (also known as the index), and the repository.

### Working Directory
 - The working directory is the local directory on your computer where you have your Git repository. It contains all the files and directories that make up your project.
 - When you start working on a project, you interact with the files in the working directory. These files can be in one of three states: untracked, modified, or staged.

### Staging Area
 - The staging area is an intermediate area that sits between the working directory and the Git repository.
 - When you make changes to files in the working directory, Git recognizes these changes as "modified." However, these changes are not automatically included in the next commit.
 - The staging area allows you to selectively choose which changes you want to include in the next commit. You can think of it as a place to prepare your changes before committing them to the Git repository.
 - To stage changes, you use the `git add` command. This command moves changes from the working directory to the staging area, marking them as ready to be committed.

### Repository
 - The Git repository is where all the committed changes are stored. It includes a database that tracks changes to files over time, allowing you to view the entire history of the project.
 - After staging your changes in the staging area, you commit them to the repository using the `git commit` command. A commit is a snapshot of the project at a specific point in time. It includes the changes staged in the staging area along with a commit message that describes the changes.
 - Commits create a history of the project, and each commit is uniquely identified by a hash. This history is crucial for tracking changes, understanding when and why specific modifications were made, and for reverting to previous states if needed.

# Git Workflow Steps

1. **`Clone the Repository:`**

Clone the Git repository to your local machine using the following command:

```bash
git clone <repository-url>
```

2. **`Create a Feature Branch:`**

Create a new branch for your feature or bug fix. This helps isolate changes and prevents interference with the main codebase:

```bash
git checkout -b feature-branch
```

3. **`Work on the Feature:`**

Make changes, add new files, or modify existing ones in your feature branch within the local working directory.

4. **`Stage and Commit Changes:`**

Stage your changes using the `git add` command and commit them to your local branch with a descriptive message:

```bash
git add .
git commit -m "Description of changes made"
```

5. **`Push the Feature Branch:`**

Periodically, push your feature branch to the remote repository to make it available to others or to back up your work:

```bash
git push origin feature-branch
```

6. **`Create a Pull Request (PR) or Merge Request (MR):`**

Initiate a pull request or merge request to propose your changes for inclusion in the main branch. This allows for code review before merging.

7. **`Code Review:`**

Team members review your proposed changes, providing feedback and suggestions to ensure code quality and alignment with project goals.

8. **`Merge the Feature Branch:`**

After approval, merge your feature branch into the main branch (e.g., `main` or `master`):

```bash
git checkout main
git merge feature-branch
```

9. **`Push Changes to Remote Repository:`**

Push the merged changes to the remote repository to update the main branch:

```bash
git push origin main
```

10. **`Delete Feature Branch (Optional):`**

Once the feature is successfully merged, optionally delete the feature branch both locally and remotely:

```bash 
git branch -d feature-branch
git push origin --delete feature-branch
```

This Git workflow promotes collaboration, code isolation, and systematic integration of new features into the main codebase.
