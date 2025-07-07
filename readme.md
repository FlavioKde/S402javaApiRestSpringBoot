markdown
# 🌐 REST API Practice Project — Spring Boot with H2, MySQL & MongoDB

This repository serves as the main entry point for a multi-database REST API practice project built with Spring Boot and Java 19. It includes **three independent submodules**, each showcasing CRUD operations with a different persistence layer: H2 (in-memory), MySQL (relational), and MongoDB (NoSQL).

## 🧾 Project Overview

- Demonstrates RESTful CRUD operations with Spring Boot 🎯  
- Includes three focused subprojects, each with its own database technology 🛢️  
- Designed with clean architecture: controllers, services, repositories, and exception handling 💡  
- Uses Swagger UI in all modules for live documentation and testing 📚  

## 🧩 Submodule Repositories

```
| Module              | Database | Description                           | Path            |
|---------------------|----------|---------------------------------------|-----------------|
| `rest-api-h2`       | H2       | CRUD API using an in-memory DB 🍥      | `repos/h2`      |
| `rest-api-mysql`    | MySQL    | CRUD API using MySQL relational DB 🐬  | `repos/mysql`   |
| `rest-api-mongodb`  | MongoDB  | CRUD API using MongoDB NoSQL DB 🍃     | `repos/mongodb` |

> Each submodule is a standalone Gradle project with its own package structure, database configuration, Swagger documentation and global exception handler.
```


## 🚀 Technologies Shared Across Modules

- Java 19 ☕  
- Spring Boot  
- Spring Web  
- Spring Data JPA / MongoDB  
- Swagger (Springdoc OpenAPI)  
- Gradle  
- Exception handling with `@RestControllerAdvice`  



## 📚 Reference Materials

These resources supported the development of the modules or could be useful when building similar systems:

```
- [Spring ResponseEntity Tutorial](https://www.baeldung.com/spring-response-entity)  
- [Spring Boot CRUD with MySQL](https://dev.to/abhi9720/a-beginners-guide-to-crud-operations-of-rest-api-in-spring-boot-mysql-5hcl)  
- [Spring Boot CRUD with MongoDB](https://www.geeksforgeeks.org/spring-boot-crud-operations-using-mongodb/)  
- [Spring H2 Database Setup](https://www.baeldung.com/spring-boot-h2-database)  

```


## 🧪 How to Clone & Initialize Submodules

```bash
git clone https://github.com/your-username/rest-api-main.git
cd rest-api-main
git submodule update --init --recursive
Each module can be run independently:

bash
cd repos/h2
./gradlew bootRun
Or switch to repos/mysql or repos/mongodb for other implementations.

```
📖 Swagger UI Access
Once a submodule is running locally, access Swagger documentation at:

http://localhost:8080/swagger-ui/index.html
🛠️ Project Goals

### This exercise aims to:

Solidify understanding of RESTful conventions

Practice Spring Boot MVC structure

Explore different data persistence options

Apply consistent error handling and documentation standards

Prepare for real-world backend development across data layers