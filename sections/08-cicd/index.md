---
title: CI/CD
has_children: false
nav_order: 9
---

# CI/CD

## Overview

In my *GraphProject*, I have set up a simple automated process to maintain the quality of the codebase. While my project doesn’t rely on an advanced CI/CD pipeline, I use **manual testing** and **version control** to ensure that new changes are stable and functional.

Whenever I push new changes to the repository, I manually run a set of tests to verify that the core functionalities, such as tutor recommendations and graph plotting, are working as expected. I focus on making sure that:

- The user interface responds correctly to user inputs.
- Filtering and recommendations in the tutor system are accurate.
- Graph plotting behaves as expected, even with different equations.

## Version Control

I use **Git** for version control, ensuring that all updates are properly tracked. I regularly commit changes and use **branches** to test new features before merging them into the main branch.

- Commits are written with clear messages that describe the changes.
- I use **GitHub** to store and collaborate on the project, keeping the repository updated with every change.

## Manual Testing Process

To ensure the project is working as expected, I manually:

1. Run tests for core functionality, such as the graph plotting and tutor recommendation system.
2. Check that the static files (HTML, CSS, JavaScript) are correctly served using **Node.js** and **Express**.
3. Verify that all interactions on the user interface (such as filtering tutors by age, location, and mode) are working as intended.

## Deployment

Since this project is mainly focused on **client-side functionality**, deployment is straightforward. I serve the project using a **Node.js server** that hosts the static files. I also use GitHub Pages for hosting the web version of the project, allowing users to access it directly through a web browser.
