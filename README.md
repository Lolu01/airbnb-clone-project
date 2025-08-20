# airbnb-clone-project

## Overview
The Airbnb Clone Project is a collaborative software engineering project aimed at replicating the core functionalities of Airbnb’s platform. The goal is to design and build a scalable application that allows users to list, search, and book properties.  

## Project Goals
- Build a functional web application with user-friendly interfaces.
- Learn and apply software engineering principles.
- Practice collaboration, version control, and team workflows.
- Implement robust backend APIs for managing users, properties, and bookings.

## Tech Stack
- Django (backend framework)
- PostgreSQL (database)
- GraphQL (API query language)
- React (frontend framework)
- Docker (containerization)
- GitHub Actions (CI/CD)

- ## Team Roles

- **Backend Developer**: Implements core logic, APIs, and integrates services.
- **Frontend Developer**: Builds user interfaces and ensures responsiveness.
- **Database Administrator (DBA)**: Designs and maintains the database schema.
- **DevOps Engineer**: Handles deployment, CI/CD pipelines, and server management.
- **QA Engineer**: Tests features, ensures functionality and reliability.
- **Project Manager**: Organizes tasks, timelines, and team collaboration.

- ## Database Design

### Entities & Fields
- **Users*
  - id, name, email, password, role
- **Properties*
  - id, owner_id, title, location, price, availability
- **Bookings*
  - id, user_id, property_id, start_date, end_date, status
- **Reviews*
  - id, booking_id, user_id, rating, comment
- **Payments*
  - id, booking_id, amount, payment_status, payment_date

### Relationships
- A user can own multiple properties.
- A booking belongs to a property and a user.
- A review belongs to a booking.
- A payment belongs to a booking.

- ## Feature Breakdown

- **User Management**: Handles user registration, login, profiles, and authentication.
- **Property Management**: Allows property owners to list, update, and remove their properties.
- **Booking System**: Users can book available properties for specific dates.
- **Review System**: Users can leave reviews and ratings after their stay.
- **Payment Integration**: Handles secure payments for bookings.

- ## API Security

- **Authentication**: Ensures only registered users can access resources.
- **Authorization**: Restricts actions based on user roles (e.g., host vs. guest).
- **Rate Limiting**: Prevents abuse by limiting requests per user/IP.
- **Data Encryption**: Protects sensitive data like passwords and payments.

🔑 Security is crucial to protect user data, prevent fraud, and ensure trust in the platform.

## CI/CD Pipeline

CI/CD (Continuous Integration and Continuous Deployment) automates the testing and deployment of new code. This ensures rapid delivery of updates without breaking the system.

- **Tools**:
  - GitHub Actions: Automates tests and deployments.
  - Docker: Packages app into containers for consistent environments.
  - Heroku/AWS: Hosting and deployment of the app.
