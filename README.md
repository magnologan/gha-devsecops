# DevSecOps Pipeline - GitHub Actions
DevSecOps Pipeline using free SAST, DAST and SCA tools

## How it works?

This GitHub Action runs Snyk, SonarCloud and ZAP on your repository to check for security issues and vulnerabilities in your code and your third-party dependencies.

### SCA - Software Composition Analysis 

This is provided by Snyk, all you need is a Snyk account and add the Snyk token as a secret.

### SAST - Static Application Security Testing

This is provided by SonarCloud, the SaaS version of SonarQube, all you need is a SonarCloud account and add the Sonar token as a secret. Also need to create the sonar-project.properties to your repository root.

### DAST - Dynamic Application Security Testing

This is provided by  ZAP, an open-source web proxy tool. We are only leveraging the Automated Scanning features of ZAP. You only need to point ZAP to scan the application once it is built. 

## References:
SonarCloud GHA - https://github.com/marketplace/actions/sonarcloud-scan

Snyk GHA - https://github.com/marketplace/actions/snyk

ZAP GHA - https://github.com/marketplace/actions/zap-baseline-scan
