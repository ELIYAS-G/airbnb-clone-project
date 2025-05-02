# Airbnb Clone Project

## Overview
This project is a clone of the Airbnb web application, aiming to replicate core features and improve full-stack development skills.

## Project Goals
- Build a functional clone of Airbnb.
- Practice using Python, Flask, and front-end technologies.
- Implement user authentication, property listings, and booking flow.

## Tech Stack
- Python
- Flask
- HTML / CSS / JavaScript
- MySQL (or SQLite, depending on phase)
- Bootstrap (optional for styling)
## Team Roles

### 1. Backend Developer
Responsible for building the server-side logic, APIs, and integrating the database. Ensures smooth data flow between the front end and the server.

### 2. Frontend Developer
Handles the user interface and user experience (UI/UX). Builds responsive, interactive pages using HTML, CSS, JavaScript, and frameworks.

### 3. Database Administrator (DBA)
Manages the database structure, ensures data integrity, handles migrations, and optimizes performance.

### 4. DevOps Engineer
Sets up the development, staging, and production environments. Automates deployment pipelines and ensures system reliability.

### 5. Product Owner
Defines the project vision, gathers requirements, prioritizes tasks, and ensures the project meets business goals.

### 6. Quality Assurance (QA) Engineer
Tests the application to catch bugs, ensure usability, and maintain overall software quality.

### 7. UX/UI Designer
Designs wireframes, mockups, and user flows to ensure an intuitive and engaging user experience.

### 8. Scrum Master / Project Manager
Keeps the team on track, manages timelines, removes blockers, and facilitates communication among team members.
## Technology Stack

### Python
A versatile programming language used to build the backend logic and core functionalities.

### Flask
A lightweight web framework for building RESTful APIs and handling routing, requests, and responses.

### HTML / CSS / JavaScript
Core front-end technologies for structuring, styling, and adding interactivity to the web application.

### MySQL (or SQLite)
A relational database system to store user data, bookings, property listings, and other critical information.

### Bootstrap
A front-end framework for quickly designing responsive and mobile-first user interfaces.

### Git
A version control system to track code changes and collaborate with the team.

### GitHub
A cloud-based hosting service for managing the repository, collaborating on code, and version control.

### Docker (optional, if you plan to use it)
A platform to containerize the application and ensure consistency across development and production environments.
## Database Design

### Entities and Fields

#### 1. Users
- id (unique identifier)
- name
- email
- password_hash
- date_joined

#### 2. Properties
- id
- owner_id (foreign key → Users)
- title
- description
- location

#### 3. Bookings
- id
- user_id (foreign key → Users)
- property_id (foreign key → Properties)
- start_date
- end_date

#### 4. Reviews
- id
- user_id (foreign key → Users)
- property_id (foreign key → Properties)
- rating
- comment

#### 5. Payments
- id
- booking_id (foreign key → Bookings)
- amount
- payment_date
- status

### Entity Relationships

- A **User** can have multiple **Properties**.
- A **User** can make multiple **Bookings**.
- A **Property** can have multiple **Bookings**.
- A **Booking** belongs to one **Property** and one **User**.
- A **Review** is written by a **User** for a **Property**.
- A **Payment** is linked to one **Booking**.
## Feature Breakdown

### User Management
Allows users to register, log in, update their profiles, and manage their accounts. This ensures secure access and personalized user experiences.

### Property Management
Hosts can list, update, and delete their properties, including adding photos, descriptions, and pricing. This feature forms the backbone of the platform, providing users with options to browse.

### Booking System
Enables guests to search for available properties, make reservations, and manage their bookings. This is the core transactional flow of the application.

### Reviews and Ratings
Lets users leave reviews and ratings for properties after their stay. This builds trust in the platform and helps future guests make informed decisions.

### Payment Integration
Handles secure payments, including deposits and refunds, for bookings. This ensures smooth and reliable financial transactions between guests and hosts.

### Search and Filters
Provides search functionality with filters like location, price, dates, and property type. This helps users quickly find listings that match their needs.

### Admin Dashboard (optional if you plan to build it)
Gives administrators tools to monitor users, properties, bookings, and handle reports. This keeps the platform running smoothly and safely.
