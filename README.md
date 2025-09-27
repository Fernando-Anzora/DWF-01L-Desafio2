# DWF-01L-Desafio2
## Project Description
DWF practical Challenge 2 of the laboratory group 01L, in pairs
This project is a REST API developed with **Spring Boot** for book management. It allows you to register, consult, update and delete books.

## 🛠 Technologies Used
Used Spring Boot Dependencies:

**Spring Web,**
**Spring Data JPA,**
**H2 Database,**
**Lombok,**
**Spring Boot DevTools,**
**Swagger**

Front-End frameworks:

**HTML5 + JavaScript,**
**Tailwind CSS,**
**Font Awesome,**
**SweetAlert2**

Structure of the project
bookapi/
├── src/
├── pom.xml
├── README.md
├── frontend/

## 📋 How to execute correctly

👾 Step 1:
Open the project in Intellij IDEA

🎆 Method 1:

From the Terminal we execute: .\mvnw spring-boot: run or mvn spring-boot: run

From the H2 console 
http://localhost:8080/h2-console
The parameters 
JDBC URL: jdbc: h2:mem: booksdb
User: sa
Password:(empty)

🎆 Method 2:

Run the BookapiApplication file.java from Intellij IDEA visual environment

👾 Step 2:

🎆 Method 1:
From the browser go to the url: http://localhost:8080/index.html

🎆 Method 2:

From the CMD terminal
curl http://localhost:8080/api/books

## Available Endpoints

### Get all books
```
GET http://localhost:8080/api/v1/books
```

### Search books by title
```
GET http://localhost:8080/api/v1/books/search?title=<title>
```

### Create a new book
```
POST http://localhost:8080/api/v1/books
```
**Body example:**
```json
{
  "title": "Cien años de soledad",
  "author": "Gabriel García Márquez",
  "publicationYear": 1968
}
```

### Update a book
```
PUT http://localhost:8080/api/v1/books/1
```
**Body example:**
```json
{
  "title": "Cien años enamorado",
  "author": "Gabriel García Márquez",
  "publicationYear": 1969
}
```

### Delete a book
```
DELETE http://localhost:8080/api/v1/books/1
```

### Pagination example
```
GET http://localhost:8080/api/v1/books?page=0&size=1
```

