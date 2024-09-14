---
title: Concept
has_children: false
nav_order: 2
---

# Concept

Graph Project

The project focuses on developing a tutor recommendation system with an integrated graph plotting tool. More specifically, the application will be composed of:

Backend that provides access to various functionalities, such as tutor recommendations and graph plotting, and handles data persistence.
Frontend, which will be provided both as a web application and, optionally, as a mobile application.

# Use case 1: Tutor Recommendations

Actors: User, Tutor
Description: The user can input their age and filter preferences (mode of tutoring and location) to receive tutor recommendations.

Main Flow:
The user opens the recommendation system.
Specifies their age and preferences (remote or in-person mode, location).
The system retrieves a list of matching tutors.
The user views detailed information for each tutor, such as expertise, rating, and availability.
The user can select a tutor for further communication.

# Use case 2: Graph Plotting

Actors: User
Description: The user can input equations and specify X and Y range values to generate and visualize graphs.

Main Flow:
The user opens the graph plotting tool.
Inputs an equation (e.g., y = x^2).
Specifies the X and Y axis range for the graph.
The system generates and displays the graph.