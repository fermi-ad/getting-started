# GitHub Repository Naming Guide

There are a few things to consider when naming your repo. We want repos to be easily findable. Consistency is key to making it easy for someone to find your repo. Because GitHub provides many of it's functions via generated URLs and REST APIs we should also consider what characters are used in repo names. Some characters are automatically replaced by GitHub, like spaces are turned into hyphens.

- Use hyphens to separate words
  - See [why hyphens](./why-hyphens.md) for more details on why we use hyphens.
  - Some programming frameworks require your parent folder to have a specific naming structure. Your folder name does not have to be the same as your repo name. See the example in the git-scm docs where the `linux` repo is cloned to a folder named `my-linux`. <https://git-scm.com/docs/git-clone#_examples>
- Avoid using external dependencies in your repo name
  - This causes a technical debt because your dependency may change or the name may change and then your repo name needs to be updated.
  - If your repo doesn't make sense if the dependency changes, then it's fine to include. For example, acsys-python is a Python client library and if the client is no longer Python, then this code isn't meaningful anymore, so acsys-python having "python" in the name is fine.
  - An example of something to not include in a repo name is the host name of a system. We see this in the transition from "Beams Division" to "Accelerator Division" because some things were named "BD" we have to explain the legacy for users to understand the name.
  - Your repo name should come first. In the case where you include a dependency in the repo name, it should come at the end.
- Your repo title should be descriptive and tell people what the project does.
  - If your repo has an associated acronym, spell it out in the title of the repo. If you need to reference a tool in the title and its acronym is commonly known, that’s acceptable.
- Consider potential name collisions.
  - Is your title specific enough for future users to know what it is in a search? Is your title broad enough to provide the correct context? Don’t include extraneous words that don’t immediately describe the goal of the repo.

Consider using [GitHub repo topics](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics) as a way to help other people find and contribute to your project.
