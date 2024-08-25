# Simple Student CRUD Application with Spring Boot

## Description

This project is a straightforward Student CRUD (Create, Read, Update, Delete) application developed using Spring Boot. It provides a basic example of managing student records with a focus on using Spring Data JPA for data persistence and handling.

## Features

- **Create**: Add new student records to the database.
- **Read**: Retrieve and list student records.
- **Update**: Modify existing student information.
- **Delete**: Remove student records from the database.

## Project Structure

- `Application.java`: The main entry point for the Spring Boot application and a data seeding example using `CommandLineRunner`.
- `Student.java`: Represents the student entity mapped to the `student` table in the database.
- `StudentRepository.java`: Provides CRUD operations for the `Student` entity through Spring Data JPA.

## Technologies

- **Spring Boot**: Framework used to build and run the application.
- **Spring Data JPA**: Provides JPA-based data access.
- **H2 Database**: In-memory database used for development and testing.
- **Maven**: Dependency management and build tool.

## Setup and Running

### Prerequisites

- Java Development Kit (JDK) 17 or later
- Maven 3.6.0 or higher

### Instructions

1. Clone the repository:
    ```bash
    git clone <repository-url>
    ```
2. Change to the project directory:
    ```bash
    cd <project-directory>
    ```
3. Build the project using Maven:
    ```bash
    mvn clean install
    ```
4. Start the application:
    ```bash
    mvn spring-boot:run
    ```

The application will start, and you can access the REST endpoints to interact with the student records.

### Sample Data

Upon starting, the application initializes with a sample student record:

- ``First Name``: Ellie
- ``Last Name``: Joel
- ``Email``: ellie@gmail.com
- ``Age``: 21

## Endpoints

- ``GET /students``: List all students.
- ``POST /students``: Create a new student record.
- ``PUT /students/{id}``: Update a student record by ID.
- ``DELETE /students/{id}``: Delete a student record by ID.


