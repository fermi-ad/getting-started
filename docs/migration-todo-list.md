# GitHub Migration ToDo List

  **Note:**
  Currently, there are no plans to retire Redmine or ghe-pip2. However, we highly recommend initiating the migration of repositories from these platforms to GitHub in the near future.

This document provides a step-by-step guide for migrating your code repository to GitHub.
Please follow these instructions to make the migration of code repositories to GitHub go smoothly:

- For newcomers to GitHub, we recommend following the [inital setup guide](./initial-setup.md).
- Migrate the code from an existing git repository (Redmine or ghe-pip2)
  1. Identify the source repository that needs to be migrated.
  1. Create a new repository within the Fermi-Controls organization on GitHub. (as empty repo)
  1. Clone the source repository locally to begin the migration process.
  1. Add the new repository as a remote destination for the code migration.

        ```sh
        $ git remote set-url origin https://github.com/fermi-controls/<name of the repo>.git
        $ git remote -v
        origin https://github.com/fermi-controls/<name of the repo>.git (fetch)
        origin https://github.com/fermi-controls/<name of the repo>.git(push)
        ```

  1. Push the code from the source repository to the new repository. The options `--all` and `--tags` pushes all your branches and tags.

        ```sh
        git push origin --all
        git push --tags
        ```

- Communicate with collaborators to update their local working directories:

    ```sh
    git remote set-url origin https://github.com/fermi-controls/<name of the repo>.git
    ```

- Retire your old repository: Once you have successfully migrated your repositories to GitHub, delete or archive the old repositories and communicate the retirement to your team and stakeholders.
