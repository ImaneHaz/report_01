---
title: Design
has_children: false
nav_order: 4
---

# Design

This chapter outlines the strategies used to meet the requirements identified in the analysis.

## Architecture

At a high level, **GraphProject** consists of three fundamental components:

- **Backend**: Provides a REST static file serving using Node.js and Express that handles core functionalities, such as tutor recommendations and graph plotting, and interfaces with the local data in JavaScript arrays for data persistence.
- **Frontend Web Application**: Communicates with the backend through the REST static file serving using Node.js and Express, allowing users to input preferences for tutor recommendations and graph equations.
- **client-side data management Database**: Stores user preferences, tutor information, and graph data in a flexible format that supports scalability and fast querying.

The architecture follows a **layered approach**:

- **Presentation Layer**: Responsible for handling user interactions, displaying tutor recommendations and rendering graphs on the frontend.
- **Business Logic Layer**: Implements the core logic, including matching user preferences with tutors and processing graph plotting requests.
- **Persistence Layer**: Interfaces with the client-side data management local data in JavaScript arrays for storing and retrieving tutor data, user preferences, and graph configurations.
- **Database Layer**: Manages data storage in a client-side data management structure, ensuring flexible and scalable storage of user, tutor, and graph data.

## Modelling

- The system's domain is modeled around key entities such as **User**, **Tutor**, **Recommendation**, and **Graph**.
- These entities are structured to handle seamless user preference matching, tutor data retrieval, and graph generation.
- **Class Diagrams** highlight the relationships between these entities, focusing on:
    - How user preferences are stored and processed.
    - How tutors are filtered based on criteria such as location, mode of tutoring, and expertise.
    - How graphs are generated based on user inputs.
- **Domain-Driven Design (DDD)** principles are used to manage the complexity of tutor recommendation and graph plotting behaviors.

## Interaction

- **Sequence Diagrams** illustrate how the system processes key workflows, such as:
    - **Tutor Recommendation Flow**: From user input (age, preferences) to retrieving matching tutors from the local data in JavaScript arrays and sending them to the frontend for display.
    - **Graph Plotting Flow**: From user input of a mathematical equation to graph rendering based on the specified X and Y axis ranges.
- Activity diagrams are used to visualize complex processes and interactions between the backend, frontend, and local data in JavaScript arrays.

## Behaviour

- **State Diagrams** describe the different states the system can be in, including:
    - **User Authenticated**: The user has successfully logged in.
    - **Recommendation Generated**: The system has provided tutor recommendations based on user inputs.
    - **Graph Rendered**: A graph has been successfully generated from the user’s input equation.
- Transitions between these states are triggered by user actions, such as submitting filters, requesting recommendations, or plotting graphs.

## Data-related Aspects

- **Data Schema**: The local data in JavaScript arrays uses a client-side data management schema with the following key documents:
    - **User Document**: Stores user details, including their preferences, past recommendations, and graph history.
    - **Tutor Document**: Contains tutor-specific information such as subjects, ratings, and availability.
    - **Recommendation Document**: Logs the results of tutor queries based on user preferences.
    - **Graph Configuration Document**: Stores the user's input equations and graph settings.
- **Data Persistence Technologies**: The system utilizes a client-side data management local data in JavaScript arrays like MongoDB or Firebase to provide flexible, scalable, and fast access to stored data.
- **Backup and Recovery**: Regular data backups will be scheduled to ensure integrity and enable quick recovery in case of system failure.
