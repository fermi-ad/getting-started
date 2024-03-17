# GitHub Repository Naming Guide

There are a few things to consider when naming your repo. We want repos to be easily findable. Consistency is key to making it easy for someone to find your repo. Because GitHub provides many of it's functions via generated URLs and REST APIs we should also consider what characters are used in repo names. Some characters are automatically replaced by GitHub, like spaces are turned into hyphens.

## General Principles:

- Clarity and Conciseness: Use a descriptive title that tells users what the project does.
- Readability: Separate words with hyphens (-) for clarity. See why hyphens: [./why-hyphens.md](./why-hyphens.md) for details.
- Consistency: Maintain a consistent structure across repositories.
- Future-proof: Opt for names adaptable to future changes (e.g., avoiding external dependencies).

## Structure:

- Core Name: A descriptive term representing the repository's function (e.g., api, data-pipeline, protocol-translator)
- Optional Suffix (e.g., language): -python (use sparingly based on specific logic)

## Specific Considerations:

- Minimize External Dependencies:
  - Avoid including dependency names to prevent technical debt from future changes.
  - Include the dependency only if the repo becomes unusable without it (e.g., acsys-python).
- Acronyms: Acceptable for common terms, but spell out if the name is solely the acronym.
- Searchability: Choose keywords relevant for someone searching for your repository.
- Name Collisions: Ensure your title is specific enough for future users to find it in a search.
- Avoid Extraneous Words: Focus on words that immediately describe the repo's goal.
- Capitalization: Discouraged to avoid case-sensitivity issues.

## Additional Considerations:

- Folder vs. Repo Name: Your folder name can differ from your repo name (e.g., linux repo cloned to my-linux folder). Refer to the git-scm docs for details: <https://git-scm.com/docs/git-clone#_examples>
- GitHub Topics: Use these (<https://github.com/topics/docs>) to help others find and contribute to your project.

