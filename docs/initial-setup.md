# Initial Setup

This document provides a step-by-step guide to start using GitHub in the Fermi-AD organization.

###  1. Joining Fermi-AD
- Get added to Fermi-AD organization (TBD).

### 2. Secure your account 
- Configure your  GitHub account with [two-factor authetication (2FA)](https://docs.github.com/en/authentication/securing-your-account-with-two-factor-authentication-2fa/configuring-two-factor-authentication)
- Configure Single Sing-On (SSO):
   - Make sure your GitHub account is associated with your @fnal.gov email address.
   - Set Up your [git cli with SAML SSO](https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/about-authentication-with-saml-single-sign-on#authorizing-personal-access-tokens-and-ssh-keys-with-saml-sso)

### 3. Verify GitHub credentials and configurations.
  1. Check credentials: Verify that  that you have valid GitHub credentials including your username, SSO and 2FA.
  2. Set your Git identity in your development environment :

```
git config --global user.name "Your Name"
git config --global user.email "your-email@fnal.gov"
```

### 4. Network configuration - optional:
-  _Applies when working from Controls network_ - Set up your `~/.ssh/config` to securely connect through a bastion _using SSH_ to interact with GitHub.

```~/.ssh/config
Host github.com
    ProxyJump <bastion-host>
```
To request access to the bastion systems, please consult your line manager and have them complete a access request form on your behalf.

### 5. Repository Setup
- Review our [content guidelines](./content-guidelines.md) to determine the appropriate settings and structure for your repository. The recommendations will help you make informed decisions regarding repository visibility, collaboration settings, data sensitivity, security features, licensing, compliance, and external contributions.


## Troubleshooting

 Here's a common problem and solution for VSCode users on Windows when enabling SSO:

 **Issue:**
```sh
remote: The `fermi-ad' organization has enabled or enforced SAML SSO. To access
remote: this repository, you must re-authorize the OAuth Application `Git Credential Manager`.
fatal: unable to access '<repo URL>': The requested URL returned error: 403
```
**Solution:** Follow the instructions provided in [this Stack Overflow thread](https://stackoverflow.com/questions/66475833/how-to-re-authorize-the-oauth-application-git-credential-manager) instructions.
