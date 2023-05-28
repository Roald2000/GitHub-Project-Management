## Git Commands for Project Management

This tutorial provides a guide on using Git commands throughout the life cycle of a project. You can follow these steps to create a project repository, work on features/changes, collaborate with others, and resolve issues. The commands are presented in Markdown format for easy integration into your README.md file.

### Creating a Project Repository

1. Create a new repository on a remote server (e.g., GitHub, GitLab).
2. Clone the remote repository to your local machine:
   ```shell
   git clone <repository_url>
   ```
3. Initialize Git in the project directory:
   ```shell
   git init
   ```
4. Add and commit your project files:
   ```shell
   git add .
   git commit -m "Initial commit"
   ```
5. Link the local repository to the remote repository:
   ```shell
   git remote add origin <repository_url>
   git push -u origin master
   ```

### Working on Features/Changes

1. Create a new branch for a new feature or bug fix:
   ```shell
   git branch <branch_name>
   git checkout <branch_name>
   ```
2. Make changes to the files and stage them:
   ```shell
   git add .
   ```
3. Commit the changes to the branch:
   ```shell
   git commit -m "Implement feature XYZ"
   ```
4. Push the branch to the remote repository:
   ```shell
   git push origin <branch_name>
   ```

### Merging Changes

1. Switch to the main branch:
   ```shell
   git checkout main
   ```
2. Fetch the latest changes from the remote repository:
   ```shell
   git fetch
   ```
3. Merge the changes from the feature branch:
   ```shell
   git merge <branch_name>
   ```
4. Resolve any merge conflicts if they occur.
5. Push the merged changes to the remote repository:
   ```shell
   git push origin main
   ```

### Collaborating with Others

1. Fetch the latest changes from the remote repository:
   ```shell
   git fetch
   ```
2. Create a new branch based on the latest changes:
   ```shell
   git branch <new_branch>
   git checkout <new_branch>
   ```
3. Make changes, commit, and push to the new branch:
   ```shell
   git add .
   git commit -m "Implement feature XYZ"
   git push origin <new_branch>
   ```
4. Create a pull request or merge request on the remote repository to propose changes.

### Resolving Issues and Rollbacks

1. Identify the commit that introduced the issue:
   ```shell
   git log
   ```
2. Create a new branch to fix the issue:
   ```shell
   git branch <fix_branch>
   git checkout <fix_branch>
   ```
3. Make changes, commit, and push to the fix branch:
   ```shell
   git add .
   git commit -m "Fix issue ABC"
   git push origin <fix_branch>
   ```
4. Merge the fix branch into the main branch or relevant branches once tested:
   ```shell
   git checkout main
   git merge <fix_branch>
   git push origin main
   ```

Feel free to integrate these Git commands into your project's README.md file and use them as a reference for your team's Git workflows. For more detailed information on each command, refer to the Git documentation or use `git --help` in your command-line interface.

Happy coding!
