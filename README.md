# Setup Instructions

## Prerequisites
1. **Install Git:** Ensure that Git is installed on your machine. You can download it from [git-scm.com](https://git-scm.com).

## Cloning the Repository
1. **Clone the Repository:** Open your terminal (or command prompt) and run the following command to clone the repository to your local machine:
  
   git clone https://github.com/yourusername/COMP3104_Group63_Assignment.git

## Navigate to the Project Directory
Change into the project directory:

cd COMP3104_Group63_Assignment

## Creating a Personal Branch
Create Your Personal Branch: Each member should create a personal branch using the naming convention `STUDENTID-Name`. Run the following command, replacing `STUDENTID` and `Name` with your actual student ID and name:
  ```bash
 git checkout -b STUDENTID-Name

```
## Working on Your Branch
1. **Make Changes or Add New Files:** Modify existing files or add new files as needed for the project.
2. **Stage and Commit Your Changes:** After making your changes, stage and commit them with clear commit messages:
   ```bash
   git add .
   git commit -m "Meaningful commit message"
   git push -u origin STUDENTID-Name
## Merging to Main
1. **Create a Pull Request (PR):** After pushing your branch, go to the GitHub repository page, and you will see an option to create a pull request. Click on "Compare & pull request."

2. **Review Process:**
   - Other members or the team leader will review the pull request. Make sure to address any comments or requested changes before merging.

3. **Resolve Merge Conflicts:**
   - If there are merge conflicts, resolve them locally by checking out the main branch, pulling the latest changes, and then merging your branch back into the main branch. Follow these commands:
   ```bash
   git checkout main
   git pull origin main
   git checkout STUDENTID-Name
   git merge main
## Resolving Merge Conflicts
- Resolve any conflicts that arise, then stage and commit the resolved files:
  ```bash
  git add .
  git commit -m "Resolved merge conflicts"
  git push
## Finalize the Merge
Once the PR is approved, it can be merged into the main branch.

## Final Notes
- Always ensure to keep your branch updated by regularly pulling from the main branch to avoid conflicts.
- Use meaningful commit messages to make it easier for others to understand your changes.