# Contributing to DMP Dashboard

Welcome! Thank you for your interest in contributing to **DMP Dashboard**, an open source tool for monitoring and visualizing Data Management Plans (DMPs) within research projects and organizations. This contribution guide applies to all who wish to assist, whether by fixing bugs, contributing code, or improving documentation.

We aim to foster collaboration while ensuring  integrity, clear process, and adherence to best practices. Please read this document carefully before contributing.

---

## Code of Conduct

All contributors are expected to follow the [Code of Conduct](https://www.contributor-covenant.org/version/3/0/code_of_conduct/). Please ensure that interactions remain respectful and constructive. A welcoming and inclusive environment is essential for the success of this project.

---

## How You Can Help

### Report Issues or Bugs

Identify problems in the dashboard, methodology, software, or documentation. Steps to report bugs:

- **Search the Issues tab** to see if the problem has already been reported.
- **Open a new issue** if no existing issue matches your bug.
- Include the following details:
  - A clear description of the issue.
  - Steps to reproduce the problem (if applicable).
  - Error logs/screenshots (if relevant).
  - Details about your environment (e.g., R version, operating system, setup).

### Propose New Features

Suggest features to improve: usability, performance, reproducibility, or general functionality. Be sure to align requests with the goals of the project.

---

## General Contribution Guidelines

1. **Fork and Clone the Repository**
   - Fork this repository on GitHub.
   - Clone your fork to your local system:
     ```bash
     git clone https://github.com/your-username/dmp-dashboard.git
     cd dmp-dashboard
     ```

2. **Set Up Your Development Environment**
   - This project uses R. See the [README.md](README.md) for prerequisites.
   - Install dependencies via:
     ```r
     install.packages("renv")  # if not already installed
     renv::restore()
     ```

3. **Make Your Changes**
   - Create a new branch for your contribution:
     ```bash
     git checkout -b my-changes-branch
     ```
   - Make your proposed changes, adhering to coding standards and documentation requirements.

4. **Test Your Changes**
   - Run and validate tests as appropriate.
   - Ensure your code passes formatting standards and does not introduce bugs.
   - Include tests for any new functionality where applicable.

5. **Submit a Pull Request**
   - Push changes to your forked repository:
     ```bash
     git push origin my-changes-branch
     ```
   - Open a Pull Request (PR) from your branch to the main repository `main` branch.
   - Describe your changes in detail:
     - What problem does this solve/improve?
     - How does it affect the current code or methodology?
     - Are any areas still in progress?
     - Link to related issues (if any).

---

## Acknowledging Contributions

Depending on the level of contribution, contributions will be recognized in the `CITATION.cff` as authors.

---

Thank you for helping make DMP Dashboard better!
