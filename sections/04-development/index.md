---
title: Development
has_children: false
nav_order: 5
---

# Development

## Distributed Version Control System
To track the development of the project, I used a GitHub repository and created a dedicated organization called `unibo-dtm-se-2324-graphproject`. The main repository is `GraphProject`, with branches for different development stages. The `master` branch contains project releases, while the `develop` branch is used for ongoing development.

Commits were written following the [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/) approach. A commit is therefore written in the following format:

```bash
<type>[optional scope]: <description>

The types of commits that have been adopted in this project are:

**build: for changes related to the build system or external dependencies;
**chore: for changes that do not affect the production code;
**ci: for changes related to continuous integration;
**docs: for changes that only affect the documentation;
**feat: for the addition of a new feature;
**fix: when a bug is fixed;
**perf: for changes made to improve performance;
**refactor: for changes to the code that are not bug fixes or new features (e.g., moving a method from one class to another);
**style: for changes that do not affect the meaning of the code (e.g., removing white spaces, formatting);
**test: for adding or correcting tests.

**Implementation details

- One important aspect of the project that I'm particularly proud of is the TutorRecommendation class, which efficiently filters tutors based on user preferences like age, mode of tutoring (remote or in-person), and location. This class significantly improved the response time of the recommendation engine.

- Another feature worth mentioning is the GraphPlotter module, which handles user input for mathematical equations and dynamically generates the corresponding graph. It provides users with an intuitive interface for visualizing equations and supports different types of graphs with minimal input.
