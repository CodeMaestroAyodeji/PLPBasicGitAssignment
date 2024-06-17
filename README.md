# PLPBasicGitAssignment

This repository demonstrates the basic Git and GitHub workflow including repository creation, local setup, making changes, committing, and pushing to GitHub.

## Steps and Commands Used

### Task 1: Repository Setup

1. **GitHub Repository Creation:**
   - Log in to my GitHub account.
   - Create a new repository named `PLPBasicGitAssignment`.
   - Initialize it with a README file.

### Task 2: Local Setup

2. **Local Folder Setup:**
   - Create a new folder on your local machine named `PLPBasicGitAssignment`.
   - Open a terminal or command prompt and navigate to the created folder:
     ```bash
     cd path/to/PLPBasicGitAssignment
     ```

3. **Git Initialization:**
   - Initialize a new Git repository in your local folder:
     ```bash
     git init
     ```

4. **Connecting to GitHub:**
   - Link your local repository to the GitHub repository:
     ```bash
     git remote add origin https://github.com/CodeMaestroAyodeji/PLPBasicGitAssignment.git
     ```

### Task 3: Making Changes

5. **Create a File:**
   - Inside your local folder, create a new text file named `hello.txt`.
   - Add a simple text message "Hello, Git!" to the file.

6. **Committing Changes:**
   - Stage the changes:
     ```bash
     git add hello.txt
     ```
   - Commit the changes:
     ```bash
     git commit -m "Add hello.txt with a greeting"
     ```

### Task 4: Pushing to GitHub

7. **Pushing to GitHub:**
   - Pull the latest changes from the remote `main` branch and rebase your local changes on top:
     ```bash
     git pull origin main --rebase
     ```
   - Push the committed changes to your GitHub repository:
     ```bash
     git push -u origin main
     ```

### Task 5: Verification

8. **Verify on GitHub:**
   - Visit your GitHub repository in a web browser and confirm that the `hello.txt` file and commit message are visible.

### Additional Steps for Cleanup

9. **Rename `master` to `main`:**
   - If your local branch is named `master` and you want to consolidate to `main`:
     ```bash
     git branch -m master main
     ```
   - Push the `main` branch and set it to track the remote `main`:
     ```bash
     git push -u origin main
     ```

10. **Delete the remote `master` branch:**
    - Delete the remote `master` branch to avoid confusion:
      ```bash
      git push origin --delete master
      ```

11. **Prune remote-tracking branches:**
    - Remove any references to deleted branches from your local repository:
      ```bash
      git fetch -p
      ```

### Conclusion

By following these steps, you have successfully set up a Git and GitHub workflow, created and pushed changes to a repository, and consolidated your branches. If you encounter any issues, refer to the GitHub documentation or seek assistance.

---

Created and maintained by Ayodeji.