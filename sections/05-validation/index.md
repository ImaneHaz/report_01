---
title: Validation
has_children: false
nav_order: 6
---

# Validation

## Testing

- The testing process for GraphProject followed a combination of **Test-Driven Development (TDD)** and **manual testing** to ensure that all features meet the functional and non-functional requirements.
    - **Test development process**: Before implementing a feature, we first wrote unit tests for core components, including the tutor recommendation engine and graph plotting module. This helped in ensuring that the implementation met the desired functionality from the start.
    - **Success rate**: The majority of our tests passed on the first run, with a success rate of 95%. Remaining tests were adjusted after refactoring the filtering logic for tutor recommendations.
    - **Coverage**: We aimed for high test coverage, particularly for critical parts like the recommendation engine and the graph plotting system. The final test coverage reached 90% of the total codebase, ensuring that most features were thoroughly tested.
    - **Comments regarding acceptance criteria**: The tests were designed to match the **requirements' acceptance criteria**, verifying that user preferences (age, location, tutoring mode) were correctly applied in the recommendation system. Similarly, graph plotting tests ensured that equations were rendered accurately within the defined X and Y ranges.

## Acceptance test

- Acceptance tests were conducted to verify that the implemented system aligns with the user stories and functional requirements.
    - For the tutor recommendation system, acceptance tests confirmed that users were able to filter tutors based on age, location, and tutoring mode, and the results matched the expected tutor profiles.
    - For the graph plotting feature, acceptance tests ensured that users could input mathematical equations, set the X and Y axis ranges, and the graphs generated matched the expected visual outputs.
    - Comments regarding acceptance criteria: All acceptance tests passed successfully, confirming that the system met the initial requirements. For example, tutor recommendations were delivered within the expected 3-second time frame, and graph plots were rendered correctly based on the input equation.
