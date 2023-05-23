# ToDo List
This document provides a step-by-step guide for migrating your code repository to GitHub.
Please follow these instructions to make the migration of code repositories to Github go smoothly:

- [ ] Get added to FNAL Controls organization (TBD).
- [ ] Determine if your repository should be on-premises or in the cloud (TBD)
- [ ] Verify GitHub credentials and configurations
   - Ensure that you have valid GitHub credentials (username and password).
   - In your development environment,  set your user name and email address:
  ```
  git config --global user.name "Your Name"
  git config --global user.email "your-email@fnal.gov"
  ```
- [ ] Migrate the code from an existing git repository (Redmine or ghe-pip2)
   1. Identify the source repository that needs to be migrated.
   2. Create a new repository within the FNAL Controls organization on GitHub. (as empty repo)
   3. Clone the source repository locally to begin the migration process.
   4. Add the new repository as a remote destination for the code migration.
    ```
    $ git remote rm origin
    $ git remote add origin https://github.com/fermi-controls/<name of the repo>.git
    $ git remote -v
    origin	https://github.com/fermi-controls/<name of the repo>.git (fetch)
    origin	https://github.com/fermi-controls/<name of the repo>.git(push)
    ```
    5. Push the code from the source repository to the new repository.
    TBD add steps to push all branches
    ```
    $ git push
    ```
- [ ] Fix local working directories to point to the new repository. TBD.. same as previous step
- [ ] Optional. Working from Controls network - proxy setup . TBD 
