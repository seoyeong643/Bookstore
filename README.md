# Bookstore
A simple Spring Boot REST API for managing books. This project includes endpoints to create, read, update, and delete books.

## Project Structure
```css
bookstore
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com
│   │   │       └── example
│   │   │           └── bookstore
│   │   │               ├── BookstoreApplication.java
│   │   │               ├── controller
│   │   │               │   └── BookController.java
│   │   │               ├── model
│   │   │               │   └── Book.java
│   │   │               └── repository
│   │   │                   └── BookRepository.java
│   │   └── resources
│   │       └── application.properties
│   └── test
│       └── java
│           └── com
│               └── example
│                   └── bookstore
│                       └── BookstoreApplicationTests.java
└── pom.xml
```

## Getting Started

### Prerequisites

- Java 11 or later
- Maven
- Spring Boot 2.7.x or later

### Dependencies

- Spring Web
- Spring Data JPA
- H2 Database

## Running the Application
You can run the application by executing the `main` method in `BookstoreApplication.java` or using the following Maven command:
```sh
mvn spring-boot:run
```

## API Endpoints
 
- **Get all books:** `GET http://localhost:8080/api/books`
- **Get book by ID:** `GET http://localhost:8080/api/books/{id}`
- **Create a new book:** `POST http://localhost:8080/api/books`
  - Request Body (JSON):
    ```json
    {
      "title": "Sample Book",
      "author": "Author Name"
    }
    ```
- **Update a book:** `PUT http://localhost:8080/api/books/{id}`
  - Request Body (JSON):
    ```json
    {
      "title": "Updated Book Title",
      "author": "Updated Author Name"
    }
    ```
- **Delete a book:** `DELETE http://localhost:8080/api/books/{id}`



