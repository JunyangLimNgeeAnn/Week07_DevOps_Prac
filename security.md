
 # Security Scanning

## Overview
This repository uses three types of security scanning:

### SAST (Static Analysis with CodeQL)
- Scans source code for vulnerabilities
- Runs on push to main branch
- Checks for: 
- Logic errors
- Data flow issues
- Debugging or unsafe configurations
- Artifacts: See GitHub Security tab

### SCA (Dependency Check)
- Scans Python packages for known CVEs
- Runs on push to main branch
- Checks for: 
- Outdated packages
- Known vulnerabilities in dependencies
- Artifacts: sca-reports

### DAST (Live Application with ZAP)
- Tests running application for vulnerabilities
- Runs on push to main branch
- Checks for: 
- Missing or insecure HTTP headers
- Runtime configuration issues
- Endpoint vulnerabilities
- Artifacts: zap-baseline-reports, zap-fullscan-reports

## Understanding Results
[Link to Part 10 in README]

## Reporting Vulnerabilities
Please email security@example.com