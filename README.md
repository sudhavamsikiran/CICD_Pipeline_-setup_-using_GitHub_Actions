# CICD_Pipeline_-setup_-using_GitHub_Actions
CI/CD pipeline using GitHub Actions that automates the build, test, and deployment process for the application
## CI/CD Pipeline

### Overview
This repository contains a CI/CD pipeline implemented using GitHub Actions. The pipeline automates the build and deployment processes, ensuring high-quality and secure code delivery.

### Pipeline Workflow
The pipeline is triggered on every push and pull request to the `main` branch. It consists of the following steps:

1. **Checkout code:** Fetches the repository content.
2. **Set up Node.js:** Installs the specified Node.js version.
3. **Install dependencies:** Installs the required project dependencies.
4. **Run tests:** Executes the test suite.
5. **Build project:** Builds the project for production.
6. **Scan for secrets:** Uses Yelp's `detect-secrets` to scan for sensitive information in the codebase.
7. **Security scan:** Uses GitHub's CodeQL to perform a security scan.

### Deployment
After a successful build, the pipeline deploys the application to the production environment.

### Quality and Security Checks
The pipeline ensures quality and security through the following checks:

- **Automated tests:** Runs the test suite to verify code functionality.
- **Secret scanning:** Detects any hardcoded secrets in the codebase.
- **Security scanning:** Identifies potential security vulnerabilities using CodeQL analysis.


