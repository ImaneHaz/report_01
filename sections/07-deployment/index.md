---
title: Deployment
has_children: false
nav_order: 8
---

# Deployment

## Overview

The *GraphProject* is primarily a web-based project using **HTML, CSS, and JavaScript** for the tutor recommendation system and graph plotting tool, served using **Node.js** and **Express**. The project also includes a **Jekyll** website hosted on GitHub Pages to display the documentation and project details.

## Branch-specific Deployment (Jekyll Site)

In the `feature/some-feature` branch, you will find two additional files: **Gemfile** and **Gemfile.lock**. These files are essential for managing the dependencies for the Jekyll-based project website hosted at https://imanehaz.github.io/GraphProject/.

- **Gemfile**: Specifies the version of **Jekyll** and any plugins used to build the website. This file ensures that the site is built with the correct tools.
- **Gemfile.lock**: Locks the exact versions of the dependencies listed in the **Gemfile**, ensuring consistency across environments.

These files are crucial for maintaining the Jekyll website. They help manage dependencies and ensure the site builds consistently both locally and on GitHub Pages.

### Jekyll-based Website
To deploy the Jekyll site, GitHub Pages automatically builds the site using the **Gemfile** and **Gemfile.lock**. No additional steps are required once the branch is pushed to GitHub, as GitHub Pages will handle the deployment.

By keeping the Gemfile and Gemfile.lock in the feature/some-feature branch, the Jekyll website remains functional, ensuring that the documentation is properly hosted and up-to-date.
