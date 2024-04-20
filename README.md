
# ATDev Assignment :

This Assignment is a Student Management System built using Spring Boot framework. It provides basic CRUD (Create, Read, Update, Delete) functionalities for managing student records.

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- MySQL (for demonstration purposes)
- Maven

## API Endpoints

- GET      /api/students: Fetch all students
- POST     /api/students: Create a new student
- PUT      /api/students/{id}: Update an existing student
- DELETE   /api/students/{id}: Delete a student by ID

## Sample Request/Response

- GET  /api/students
Response :
```json
        [
            {
                "id": 1,
                "name": "sangmesh birajdar",
                "age": 24
            },
            {
                "id": 2,
                "name": "ramesh patil",
                "age": 25
            }
        ]
```

- POST  /api/students
Request : 
```json
        {
            "name": "sangmesh birajdar",
            "age": 24
        }
```
Response :
```json
        {
            "id": 3,
            "name": "ramesh patil",
            "age": 24
        }
```

- PUT  /api/students/{id}
Request :
```json
        {
            "name": "sangmesh birajdar"
        }
```
Response:
```json
        {
            "id": 3,
            "name": "rahul mane ",
            "age": 25
        }
```

- DELETE  /api/students/{id}

Response: 204 No Content

## Database
This project uses MySQL database for demonstration purposes.  Using "application.properties" file, you can configure any other database.
