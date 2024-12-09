# Blog_Application


EchoWrite Blog Application

Welcome to EchoWrite, a simple yet powerful blog application built with Spring Boot. This application allows users to register, log in, create, edit, delete, and view blog posts with ease. It provides a basic structure for a full-fledged blog system and serves as a great foundation for building more advanced features.



Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Technology Stack](#technology-stack)
4. [Installation & Setup](#installation--setup)
5. [Configuration](#configuration)
6. [Usage](#usage)
7. [Contributing](#contributing)
8. [License](#license)



Introduction

EchoWrite is a blog application developed using Java Spring Boot, offering a clean and user-friendly interface for managing blog posts. Whether you are a novice blogger or a seasoned content creator, EchoWrite helps you easily share your thoughts and ideas with the world.



 Features

- User Authentication: Allows users to register, log in, and manage sessions securely.
- Post Management: Users can create, edit, delete, and view posts with rich text formatting.
- Image Upload: Supports uploading images for blog posts, enhancing the content.
- Admin Access: Default admin account for managing users and posts.



Technology Stack

Backend:  
- **Spring Boot**: A powerful Java-based framework for building robust web applications.  
- **Spring Security**: Ensures secure authentication and authorization.  
- **Spring Data JPA**: Provides a streamlined way to interact with the database.  
- **Thymeleaf**: A templating engine for rendering dynamic HTML views.  
- **MySQL**: A relational database to store user and post data.

**Frontend**:  
- **HTML/CSS**: Clean and responsive UI built using HTML5 and CSS3.  
- **Bootstrap**: Ensures the app is mobile-friendly and responsive.

**Additional Tools**:  
- **Maven**: Dependency management and build automation tool.  
- **Git**: Version control for easy collaboration.

---

## **Installation & Setup**

### **Prerequisites**

Before running the application, make sure you have the following installed on your machine:

- **Java 11 or later**  
- **Maven**  
- **MySQL Database**  

### **Steps to Run Locally**

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/EchoWrite.git
   cd EchoWrite
   ```

2. **Configure the Database**

   - Install MySQL and create a new database named `echowrite`.
   - Configure your `application.properties` file with the database credentials.

3. **Build the Project**

   Run the following command to build the application using Maven:

   ```bash
   mvn clean install
   ```

4. **Run the Application**

   Start the Spring Boot application using the command:

   ```bash
   mvn spring-boot:run
   ```

   The application will be accessible at `http://localhost:8080/`.

---

## **Configuration**

This section outlines the main configuration parameters for your application:

### **1. Database Configuration**

Make sure to configure your MySQL database URL, username, and password in the `src/main/resources/application.properties` file.

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/echowrite
spring.datasource.username=root
spring.datasource.password=yourpassword
```

### **2. File Upload Settings**

Set the maximum file upload size for images in `application.properties`:

```properties
spring.servlet.multipart.max-file-size=10MB
spring.servlet.multipart.max-request-size=10MB
```

### **3. Security Settings**

The default admin credentials are:

```properties
spring.security.user.name=admin
spring.security.user.password=adminpassword
```

---

## **Usage**

After starting the application, you can access the following features:

1. **Register**: New users can create an account by providing their name, email, and password.
2. **Login**: Existing users can log in using their credentials.
3. **Dashboard**: Users can view their posts and manage their content.
4. **Create Post**: Users can create a new blog post with optional image uploads.
5. **Edit Post**: Users can update their existing posts.
6. **Delete Post**: Users can delete unwanted posts.

Note: Admin users have full control over managing users and posts.

---

Contributing

We welcome contributions to make **EchoWrite** even better. Here’s how you can help:

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature-name`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push your changes to the branch (`git push origin feature-name`).
5. Create a pull request.




Acknowledgements

- Spring Boot: Thanks to the Spring team for creating a powerful and efficient framework.
- Bootstrap: For making it easier to design responsive and attractive web pages.
- Thymeleaf: For simplifying the rendering of dynamic web content.

