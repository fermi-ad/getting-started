# Initial Setup

This document provides a step-by-step guide to start using GitHub at the AD organization.

- Get added to Fermi-Controls organization (TBD).
- Configure your  GitHub account with [two-factor authetication (2FA)](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication)
- Verify GitHub credentials and configurations.
  - Ensure that you have valid GitHub credentials (username and 2FA).
  - Set your Git identity in your development environment :

    ```sh
    git config --global user.name "Your Name"
    git config --global user.email "your-email@fnal.gov"
    ```
- Optional. Working from Controls network? Set up the proxy configuration in your development environment to securely connect to and interact with GitHub.
- Review our [content guidelines](./content-guidelines.md) to determine the appropriate settings and structure for your repository. The recommendations will help you make informed decisions regarding repository visibility, collaboration settings, data sensitivity, security features, licensing, compliance, and external contributions.