# Student Management REST API with Spring Boot

This project is a beginner-friendly **RESTful API** built using **Java** and **Spring Boot**. It demonstrates the core principles of REST architecture by implementing basic **CRUD operations** for managing students. The project is designed to help beginners understand how to structure, build, and test REST APIs using Spring Boot.

---

## 🎓 Project Overview

The **Student Management API** allows users to:

* Add new students
* View all students or a single student
* Update student details
* Remove students from the system

It uses an **H2 in-memory database**, making it lightweight and easy to run without additional setup.

---

## 📦 Features

* ✅ Create new students
* 🔍 Retrieve single or multiple students
* ✏️ Update existing student records
* ❌ Delete students
* 💾 H2 in-memory database integration
* 🧪 Easy testing with Postman or curl

---

## 🛠 Technologies Used

* Java 17+
* Spring Boot
* Spring Web
* Spring Data JPA
* Maven
* H2 Database

---

## 📁 Project Structure

```
src/
└── main/
    └── java/com/springstarter/student_api/
        ├── StudentApiApplication.java
        └── student/
            ├── api/
            │   ├── StudentController.java
            │   ├── request/
            │   │   ├── StudentRequest.java
            │   │   └── UpdateStudentRequest.java
            │   └── response/
            │       └── StudentResponse.java
            ├── domain/
            │   └── Student.java
            └── repository/
                └── StudentRepository.java
```



<img width="1919" height="850" alt="delete" src="https://github.com/user-attachments/assets/730241c9-654e-4773-bb1c-6bb155cec88b" />

<img width="1908" height="1068" alt="database" src="https://github.com/user-attachments/assets/f0717c2e-fb99-4f33-b382-03d35b95cea0" />



<img wi<img width="1883" height="1055" alt="post" src="https://github.com/user-attachments/assets/81c9997d-ab9f-4865-9a38-5f80d5c6ca4c" />
dth=<img width="1894" height="1062" alt="get-all" src="https://github.com/user-attachments/assets/032eefab-85f5-47a8-b114-c3cd7ceb7d8f" />
"1886" height="1069" alt="get" src="https://github.com/user-attachments/assets/19674c67-bcba-4fb8-a683-ee4675a9b005" />



---

## 🚀 Getting Started

### Prerequisites

Ensure the following are installed:

* Java 17 or higher
* Maven

### Run the Application

```bash
git clone <repository-url>
cd student-management-api
./mvnw sprin<img width="1887" height="1063" alt="put" src="https://github.com/user-attachments/assets/b8922500-0634-4d90-a47c-669bf644a1bf" />
g-boot:run
```

The server will start at:

```
http://localhost:8080
```

---

## 🔗 API Endpoints

| Method | Endpoint       | Description                |
| ------ | -------------- | -------------------------- |
| GET    | /students      | Get all students           |
| GET    | /students/{id} | Get student by ID          |
| POST   | /students      | Create a new student       |
| PUT    | /students/{id} | Update an existing student |
| DELETE | /students/{id} | Delete a student           |

---

## 🗃 Database Access (H2 Console)

The application uses an H2 in-memory database.

Access it at:

```
http://localhost:8080/h2-console
```

**JDBC URL:** `jdbc:h2:mem:testdb`
**Username:** `sa`
**Password:** *(leave blank)*

---

## 🧪 Testing Example

**POST /students**

```json
{
  "name": "John Doe",
  "email": "john.doe@example.com",
  "course": "Computer Science"
}
```

---

