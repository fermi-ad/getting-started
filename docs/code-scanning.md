# Code scanning


## Software dependency known vulnerabilities.
Scanning your repository for known vulnerabilities is essential to maintain secure software. We recommend utilizing databases from the [National Vulnerability Database NVD](https://nvd.nist.gov/).

### GitHub Dependabot
By default, all the repositories under Fermi-AD organization have [GitHub Dependabot](https://docs.github.com/en/code-security/getting-started/dependabot-quickstart-guide) enabled.  To view the security alerts:

1. Go to your repository
2. Click "Security"
3. Click "Vulnerability alerts" in the sidebar.

For information on supported repositories and programming languages, refer to the [Dependabot documentation](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/about-dependabot-version-updates#supported-repositories-and-ecosystems)

### CVE Binary Tool

Another option for vulnerability scanning  is the [CVE Binary Tool](https://github.com/intel/cve-bin-tool), a free, open source tool. It uses data from the National Vulnerability Database (NVD),  as well from Redhat, Open Source Vulnerability Database (OSV), Gitlab Advisory Database (GAD), and Curl.
“It is intended to be used as part of your continuous integration system to enable regular vulnerability scanning and give you early warning of known issues in your supply chain. It can also be used to auto-detect components and create SBOMs.”

You can setup a [GitHub Action](https://github.com/intel/cve-bin-tool-action) to run the CVE tool as part of your CI/CD. Below is an example of the github action:


```
#.github/workflows/cve-scanner.yml
name: CVE Binary Tool Scanner

on:
  pull_request:
    branches: [ main ]
  workflow_dispatch:

permissions:
  contents: read
  security-events: write

jobs:
  scan:
    runs-on: ubuntu-latest
    steps:
      - uses: intel/cve-bin-tool-action@main
```