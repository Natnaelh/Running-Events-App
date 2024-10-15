# 🎉 Running Events - Spring Boot Project

This is a Spring Boot application for managing running events. The project is set up with Liquibase for database version control.

## Features

- 📦 Initial Spring Boot project setup
- 🔄 Liquibase integration for database migrations
- 🌱 REST API for managing running events and participants
- ⚙️ Pre-configured Maven build system

## Getting Started

### Prerequisites

To run this project, you need:

- Java 17+
- Maven 3.6+
- PostgreSQL (or your preferred database)

### Setting Up

1. Clone the repository:

   ```
   git clone <repository-url>
   cd RunningEvents
   ```
   
2. Update the database configuration in src/main/resources/application.properties:

    ```
    spring.datasource.url=jdbc:postgresql://localhost:5432/running_events_db
    spring.datasource.username=your_username
    spring.datasource.password=your_password
    ```

3, Run the application:
   ```mvn spring-boot:run```


4, Running Liquibase Migrations
To apply database migrations with Liquibase, simply start the application and Liquibase will run automatically based on the changelog file ```(db.changelog-master.xml)```.


