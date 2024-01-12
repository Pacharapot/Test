#Test
โจทย์ทำ Backend (tool .NET 8, PostgreSQL)
 โครงสร้างโปรเจค
/backend
|-- src
|   |-- YourApiProject
|       |-- Controllers
|       |-- Models
|       |-- Data
|           |-- ApplicationDbContext.cs
|           |-- Migrations
|       |-- Services
|       |-- appsettings.json
|-- YourApiProject.sln
#### Endpoints API:
1. GET `/api/departments`
2. GET `/api/departments/{id}`
3. POST `/api/departments`
4. PUT `/api/departments/{id}`
5. DELETE `/api/departments/{id}`

#### โครงสร้าง SQL (PostgreSQL):
CREATE TABLE Departments (
    Id SERIAL PRIMARY KEY,
    Name VARCHAR(255) NOT NULL
);

CREATE TABLE Users (
    Id SERIAL PRIMARY KEY,
    Name VARCHAR(255) NOT NULL,
    DepartmentId INT,
    FOREIGN KEY (DepartmentId) REFERENCES Departments(Id)
);
#### Backend README:
- คำสั่งสำหรับการตั้งค่าโปรเจค .NET และฐานข้อมูล PostgreSQL.
- ขั้นตอนสำหรับการรันเซิร์ฟเวอร์ Backend.

