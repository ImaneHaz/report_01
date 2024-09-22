---
title: Developer guide
has_children: false
nav_order: 11
---

# Developer Guide

The *GraphProject* is a simple web-based tool for graph plotting and tutor recommendations, built with **HTML, CSS, and JavaScript** and served using **Node.js** and **Express**. The codes that are writtent to build the website are in the repository 'artifact' that is in the same organization where 'report' repository can be found. Developers are welcome to contribute or make improvements to the project. Here’s how you can get started:

## Branching Strategy and Differences

To manage the development process effectively, the project uses a branching model with the following branches:

- **Master**: This branch contains the stable, production-ready code. All major features and bug fixes are tested and validated before being merged into the master branch. The master branch represents the final version that is ready for deployment.
  
- **Develop**: This is the primary branch for active development. The develop branch includes features and updates that are still being tested. Before merging into master, new code is added and tested here to ensure everything works properly. **Purpose**: To integrate new features and perform testing before pushing to the master branch.

- **Feature/some-feature**: Each feature branch focuses on developing a specific new feature or enhancement. For example, `feature/some-feature` might contain work on improving the user interface or adding a new filtering option for tutor recommendations. **Purpose**: To allow isolated development of a new feature without affecting other parts of the codebase.

### Current Branch Details:

1. **Master**:
   - Contains the latest stable version of the project.
   - The finalized version of tutor recommendations and graph plotting tools are merged into master after successful testing.
   
2. **Develop**:
   - Includes ongoing updates and features that are not yet in the final state.
   - Active testing is performed here before merging into master.
   - Purpose: To ensure code quality and stability before final deployment.

3. **Feature/some-feature**:
   - Specific features such as improvements to the graph plotting interface or additional tutor recommendation filters are developed here.
   - Once completed, the feature is merged into the develop branch for testing.
   - Purpose: To isolate specific tasks and features from the rest of the codebase, ensuring that new changes do not disrupt existing functionality.

## Getting Started

To contribute to the project, follow these steps:

1. **Clone the Repository**:  
   Clone the project from GitHub to your local machine:

   ```bash
   git clone https://github.com/your-repo-url.git
   ```

2. **Set Up the Environment**:  
   Ensure you have **Node.js** installed. Navigate to the project directory and install the necessary dependencies:

   ```bash
   npm install
   ```

3. **Run the Project Locally**:  
   Start the local server using Node.js:

   ```bash
   npm start
   ```

   This will serve the project on `http://localhost:3000`, where you can view the tutor recommendation system and graph plotting tool.

## Adding or Modifying Code

- **Code Structure**:  
   Ensure any code you add follows the current structure. Most of the logic is in the **JavaScript** files (`script.js`, `tutors.js`), and the styling is in the **CSS** file (`style.css`).
   
- **Tests**:  
   If you're adding new functionality, ensure that you test the changes manually, as there are no automated tests currently integrated.

- **Commit Messages**:  
   Write clear commit messages that describe your changes. Use conventional commit messages like `feat:`, `fix:`, or `refactor:` for better clarity.

## Submitting Changes

Once your changes are complete:

1. **Commit Your Changes**:  
   Add and commit your changes using `git`:

   ```bash
   git add .
   git commit -m "Description of the change"
   ```

2. **Push to GitHub**:  
   Push your changes to the relevant branch on GitHub (e.g., develop or feature):

   ```bash
   git push origin your-branch
   ```

3. **Create a Pull Request**:  
   Submit a pull request, describing the changes you've made. The pull request will be reviewed, and if everything aligns with the project, the changes will be merged into the develop or master branch.
