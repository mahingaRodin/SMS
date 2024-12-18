**Digital TVET School Management System**

**Project Overview**  
The Digital TVET School Management System is a Spring Boot application designed to manage various aspects of TVET schools, including user authentication, course management, and reporting. The system aims to simplify administrative tasks while providing an intuitive interface for students, teachers, and administrators.

**Features**
- **User Management**: Handle user roles such as Admin, Teacher, and Student.
- **Course Management**: Add, update, and delete courses.
- **Reports**: Generate detailed reports for school activities.
- **Authentication**: Secure login and role-based access control.

**Tech Stack**
- **Backend**: Spring Boot (Java)
- **Database**: MySQL
- **Build Tool**: Maven
- **ORM**: Hibernate (JPA)
- **API Documentation**: Swagger

**Prerequisites**
- Java 17+
- MySQL Workbench installed
- Maven installed

**Getting Started**

**Step 1: Clone the Repository**
```bash
git clone https://github.com/your-username/digital-tvet-school-management.git  
cd digital-tvet-school-management  
```  

**Step 2: Set Up the Database**
1. Open MySQL Workbench.
2. Create a new database named `tvet_management`.
3. Update the `application.properties` file with your database credentials:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/tvet_management  
   spring.datasource.username=your_username  
   spring.datasource.password=your_password  
   spring.jpa.hibernate.ddl-auto=update  
   ```  

**Step 3: Install Dependencies**  
Run the following command to install Maven dependencies:
```bash
./mvnw clean install  
```  

**Step 4: Run the Application**  
Start the application using:
```bash
./mvnw spring-boot:run  
```  

The application will run on `http://localhost:8080`.

**Project Structure**
```
src  
└── main  
    └── java  
        └── com.tvet.management  
            ├── controller    # REST controllers  
            ├── model         # Entity classes  
            ├── repository    # Data access layer  
            └── service       # Business logic  
    └── resources  
        ├── application.properties # Configuration  
```

**Endpoints**

**User Endpoints**
- `POST /users` - Create a new user
- `GET /users` - Get all users
- `GET /users/{id}` - Get user by ID

**Course Endpoints**
- `POST /courses` - Create a new course
- `GET /courses` - Get all courses
- `DELETE /courses/{id}` - Delete a course by ID

**Authentication Endpoints**
- `POST /auth/login` - User login

**Contributing**
1. Fork the repository.
2. Create a new branch (`feature/your-feature-name`).
3. Commit your changes.
4. Push to the branch.
5. Open a Pull Request.

**License**  
This project is licensed under the MIT License. See the LICENSE file for details.

**Contact**  
For questions or support, please contact:
- **Name**: mahinga rodin
- **Email**: mahingarodin@gmail.com
