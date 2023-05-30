# GitHub Repository Setup and Content Guidelines

This document provides guidelines and considerations for creating and managing GitHub repositories. It covers important aspects such as repository configuration, audience, permissions, and content restrictions. By following these guidelines, you can ensure proper setup and adherence to security and data sensitivity requirements.

## Philosophy

You are encouraged to aim for a public repository, unless there are specific reasons or restrictions that require otherwise. Public repositories promote transparency, collaboration, and knowledge sharing throughout AD, the lab, and the internet. However, it is important to consider and follow the guidelines below while configuring the repository:

The primary philosophy behind our repository management is to promote transparency, collaboration, and knowledge sharing within the community. While the main goal is to have public repositories whenever possible, there may be certain situations or restrictions that require the use of private or internal repositories. We strive to strike a balance between openness and the need to protect sensitive or proprietary information.
To adhere to this philosophy, we emphasize the separation of base code from configuration files. Keeping configuration files separate allows for easier sharing, collaboration, and customization while maintaining a strong foundation of reusable code. It enables others to adapt and extend our projects to suit their specific needs, driving innovation and fostering a vibrant developer community.

## Repository content:

Here is a list of things to NOT put into a GitHub repository:

* Credentials/secrets/tokens
  * We recommend using [name a tool] for storing and retrieving this kind of information.
* Configuration
  * Coding best practices includes magic numbers in this category.
  * We recommend using [name a tool] for storing and retrieving this kind of information.
* IP addresses and hostnames
  * If the address is meant for public consumption, then it may be included. Addresses that are only used internally should not be included in code repositories.
  * We recommend using [name a tool] for storing and retrieving this kind of information.
* Controlled Unclassified Information (CUI) or Personally Identifiable Information (PII)
  * This kind of content should not be included ever.
  * If you must handle this kind of information then Fermilab training will guide you on handling this kind of data.
* Proprietary or licensed code
  * Please refer to the Office of Technology Transfer on this topic.

Cybersecurity contact: (?)

## Repository Setup:

You are encouraged to aim for a public repository, unless there are specific reasons or restrictions that require otherwise. Public repositories promote transparency, collaboration, and knowledge sharing throughout AD, the lab, and the internet. However, it is important to consider and follow the guidelines below while configuring the repository:

* Determine the intended audience for the repository.
  * Public, Fermilab employees and collaborators, specific group at Fermi, or select people
* Configure the folder structure and permissions and authorizations based on the repo data sensitivity.  (??)
* Configure the repository for the correct level of authentication/security based on the repository data sensitivity level:
  * Evaluate the sensitivity of the repository data and select the appropriate level of authentication and security measures.
  * If the software supports Controlled Unclassified Information (CUI) or requires moderate-level authentication, ensure the repository is appropriately configured. <https://computing.fnal.gov/cybersecurity-atwork/cui-homepage/>

   |            | Private Repository   | Public Repository   | Internal Repository (Fermi-only)   |
   |------------|----------------------|---------------------|------------------------------------|
   | Visibility | Restricted access to designated users or teams. | Accessible to anyone on the internet. | Limited access to users within the Fermi organization. |
   | Collaboration | Allows collaboration within designated users or teams. | Encourages open-source contributions from the community. | Facilitates collaboration within the organization. |
   | Data Sensitivity | Suitable for sensitive or proprietary information. | Typically contains non-sensitive or publicly shareable information. | Supports internal projects and may contain sensitive information. |
   | External Contributions | Limited to designated users or teams. | Allows contributions from the broader community. | Typically restricts contributions to internal teams or authorized users. |
   | Impact on Reputation | May have minimal public visibility, impacting reputation. | Enhances visibility and reputation in the open-source community. | Internal visibility within the organization, limited external impact. |
   | Accessibility | Limited to authorized users or teams. | Accessible to anyone on the internet. | Limited access to specific internal users or teams. |
   | Documentation | May require additional documentation and communication for access. | Publicly accessible and requires clear documentation. | Internal documentation within the organization. |

   Note: By default, all repositories within the Fermi Controls Organization are internal. If you intend to make a repository public, follow the transfer disclosure process with the Office of Technology Transfer.

* Create a [GitHub Team](https://docs.github.com/en/enterprise-cloud@latest/organizations/managing-user-access-to-your-organizations-repositories/managing-team-access-to-an-organization-repository). To provide write access to developers on repositories to facilitate their work, it is recommended to utilize GitHub Teams. GitHub Teams offer a convenient way to manage permissions and access levels for groups of users.
* [Adjust the repository settings accordingly to control access and visibility.](https://docs.github.com/en/enterprise-cloud@latest/repositories/managing-your-repositorys-settings-and-features/managing-repository-settings/setting-repository-visibility#changing-a-repositorys-visibility)
