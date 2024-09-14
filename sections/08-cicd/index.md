---
title: CI/CD
has_children: false
nav_order: 9
---

# CI/CD

## High-level description

In our *GraphProject*, I've implemented a robust CI/CD pipeline to ensure the integrity and quality of the codebase. Each component of the project is equipped with its own set of tests, covering functionality, edge cases, and integration scenarios.

Whenever a developer attempts to push new changes, typically via a pull request to the `master` branch, our CI/CD system is triggered. First, it runs a series of code checks, including linting and formatting validations, to ensure consistency and adherence to coding standards. Next, the system executes the suite of tests associated with the modified code, verifying that new changes do not break existing functionality.

Additionally, we incorporate code coverage analysis into the pipeline, generating comprehensive reports to assess the effectiveness of our test suite. If all checks pass successfully, the pipeline automatically triggers the creation of a new release version. Using semantic release guidelines, this versioning process is seamlessly tied to the commit history, providing clear and meaningful version increments. The newly created release is then published directly to our GitHub repository, making it easily accessible to stakeholders and users.

If any of the checks fail, the CI/CD pipeline acts as a gatekeeper, blocking the merge of faulty code into the `master` branch. This automated process ensures that the codebase remains stable over time, consistently aligned with the established development conventions agreed upon by the team. Moreover, the pipeline helps detect potential errors early, enhancing the overall stability and reliability of the software.
