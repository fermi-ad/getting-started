# GitHub Repository Setup and Content Guidelines

This document provides guidelines and considerations for creating and managing GitHub repositories. It covers important aspects such as repository configuration, audience, permissions, and content restrictions. By following these guidelines, you can ensure proper setup and adherence to security and data sensitivity requirements.

## Repository creation:

Here is a list of things to think about creating a GitHub repository:
* Configure the repo for the correct audience :
   * Determine the intended audience for the repository (internal, specific collaborators, Fermi-only, or public).(internal, fermi only, specific collaborators only, public, etc.)
   * Adjust the repository settings accordingly to control access and visibility.
   * Create a GITHUB TEAM(??)
* Configure the folder structure and permissions and authorizations based on the repo data sensitivity.  (??)
* Configure the repo for the correct level of authentication/security based on the repo data sensitivity level (If software supports CUI, should have moderate level auth to repo, encryption, etc.) https://computing.fnal.gov/cybersecurity-atwork/cui-homepage/ 
 
Note: By default, all repositories within the Fermi Controls Organization are private (WHAT PRIVATE MEANS, FERMI ONLY?). If you intend to make a repository public, follow the transfer disclosure process with the Office of Technology Transfer.

## Repository content: 

Here is a list of things NOT to put into a GitHub repository:
 
* Credentials/secrets/tokens
* IP addresses (I think this would depend on the repo, if a GIT repo for an internal service and not for public consumption).?????
* Hostnames (similar to IP addresses, typically stored in configuration files rather than the main repository).
* Controlled Unclassified Information (CUI) or Personally Identifiable Information (PII).
* Proprietary or licensed code.????????

Cybersecurity contact: (?) 