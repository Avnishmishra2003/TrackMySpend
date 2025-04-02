# TrackMySpend 

## Description
A comprehensive Java-based web application built using Spring Boot, Spring Data JPA, MySQL, and Thymeleaf. This project follows the MVC design pattern and offers a dynamic, database-driven web interface.

## Features
- User authentication and authorization
- CRUD operations using Spring Data JPA
- Thymeleaf templates for dynamic UI rendering
- MySQL database integration
- RESTful API endpoints
- Exception handling and validation

## Technologies Used
- **Java** (JDK 17 or latest)
- **Spring Boot** (Spring Boot Starter, Spring Data JPA, Spring Security)
- **MySQL** (Database)
- **Thymeleaf** (Template Engine)
- **Maven** (Build Tool)
- **Hibernate** (ORM Framework)

## Installation & Setup

### Prerequisites
Ensure you have the following installed:
- JDK 17 or later
- MySQL Server
- Maven
- IDE (IntelliJ IDEA, Eclipse, or VS Code)

### Steps to Setup
1. **Clone the Repository**
   ```sh
   git clone https://github.com/your-repo-name.git
   cd your-repo-name
   ```

2. **Configure Database**
   - Update `application.properties` in `src/main/resources/` with your database credentials:
     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/your_database
     spring.datasource.username=root
     spring.datasource.password=your_password
     spring.jpa.hibernate.ddl-auto=update
     ```

3. **Build & Run the Project**
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```

4. **Access the Application**
   Open your browser and navigate to:
   ```
   http://localhost:8080
   ```

## API Endpoints
| Method | Endpoint       | Description              |
|--------|--------------|--------------------------|
| GET    | /            | Home Page                |
| GET    | /users       | List all users           |
| POST   | /users       | Create a new user        |
| PUT    | /users/{id}  | Update user details      |
| DELETE | /users/{id}  | Delete a user            |

## Folder Structure
```
project-root
│   pom.xml
│   README.md
└───src
    ├───main
    │   ├───java/com/example/project
    │   │   ├───controller
    │   │   ├───service
    │   │   ├───repository
    │   │   ├───model
    │   │   ├───config
    │   ├───resources
    │   │   ├───templates
    │   │   ├───static
```

## Contribution Guidelines
1. Fork the repository
2. Create a feature branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Create a Pull Request
