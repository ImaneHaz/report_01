---
title: Design
has_children: false
nav_order: 4
---

# Design

This chapter explains the strategies used to meet the requirements identified in the analysis.

## Architecture

At a high level, GraphProject consists of three fundamental components:

- The backend, which provides a REST API for all application functionalities.
- The frontend web application, which interfaces with the backend through the REST API.
- The NoSQL database, which handles data persistence for user preferences, tutor information, and saved graph data.

The chosen architecture follows a layered approach:

- Presentation layer: Handles user interactions and displays tutor recommendations and graphs.
- Business layer: Implements the core application logic, including matching user preferences with tutor data and managing graph plotting requests.
- Persistence layer: Interfaces with the NoSQL database for storing and retrieving user and tutor data.
- Database layer: Manages the storage of tutor information, user preferences, and other relevant data in a NoSQL format.

## Modelling

- This section explains how the system’s domain has been modeled, such as defining key entities like User, Tutor, Graph, and Recommendation.
- The domain model is structured to handle user preferences, tutor data, and graph generation seamlessly.
- Class diagrams will highlight the relationships between these core entities and showcase how these designs address the requirements.
    - For instance, how Tutor objects are filtered and matched based on user criteria.
    - Tactical patterns and Domain-Driven Design (DDD) principles are applied to model complex behaviors like tutor recommendation and graph plotting.

## Interaction

- This section will describe the behavior of the system using sequence or activity diagrams.
    - For instance, a sequence diagram that shows how the system processes a tutor recommendation request: from user input to retrieving matching tutors from the NoSQL database and delivering them to the frontend.
    - Another sequence diagram could illustrate the graph plotting flow, from user equation input to graph rendering.

## Behaviour

- This section will explain the possible states of the system, using UML state diagrams to show:
    - States like User Authenticated, Recommendation Generated, and Graph Rendered.
    - Transitions between states, triggered by user actions (e.g., inputting filters, requesting recommendations, submitting graph equations).

## Data-related aspects

- Data schema: The database schema uses a NoSQL structure, storing data in documents for Users, Tutors, Recommendations, and Graph Configurations.
    - User document stores user details, including preferences and history.
    - Tutor document stores tutor-specific details such as subject expertise, rating, and availability.
    - Recommendation document logs the matching results for user queries.
    - Graph Configuration document saves user-defined equations and graph settings.
- Data persistence technologies: The system uses a NoSQL database like MongoDB or Firebase, ensuring flexible, scalable data storage and fast querying for tutor recommendations and graph plotting.
- Backup and recovery: Regular backups will be configured to ensure data integrity and quick recovery in case of failure.
