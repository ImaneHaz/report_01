---
title: Development
has_children: false
nav_order: 5
---

# Development

## DVCS
To track the development of our project, I used a Github repository and created a dedicated organization called `unibo-dtm-se-2324-graphproject Owner`. The main repository is `GraphProject`, which was divided into several branches: the `master` branch contains project releases. 


Commits were written following the [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/) approach. A commit is therefore written in the following format:

```bash
<type>[optional scope]: <description>
```

The types of commits that have been adopted in our case are as follows:

- build: for changes related to the build system or external dependencies;
- chore: for changes that do not affect the production code;
- ci: for changes related to continuous integration;
- docs: for changes that only affect the documentation;
- feat: for the addition of a new feature;
- fix: when a bug is fixed;
- perf: for changes made to the code to improve performance;
- refactor: for changes to the code that do not relate to either bug fixes or the addition of a new feature (e.g., moving a method from one class to another);
- style: for changes that do not affect the meaning of the code (e.g., removing white spaces, formatting, etc.);
- test: for the addition of new tests or correction of existing tests.

## Implementation details

- One important aspect of the project that I'm particularly proud of is the TutorRecommendation class, which efficiently filters tutors based on user preferences like age, mode of tutoring (remote or in-person), and location. This class helped improve the response time of the recommendation engine significantly.

- Another feature worth mentioning is the GraphPlotter module, which handles user input for mathematical equations and dynamically generates the corresponding graph. It provides users with an intuitive interface for visualizing equations, and it’s designed to support different types of graphs with minimal input.
