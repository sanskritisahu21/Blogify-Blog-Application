# 📝 Blogify – A Java-Based Blog Application

## 📚 Overview

**Blogify** is a full-stack blog application developed using Java and the Spring Boot framework. It enables users to create, read, update, and delete blog posts, providing a seamless blogging experience. The application is designed with scalability and maintainability in mind, leveraging modern Java development practices.

## 🛠️ Tech Stack

* **Backend:**

  * **Java 17:** Core programming language.
  * **Spring Boot:** Framework for building the application.
  * **Spring MVC:** For handling web requests and responses.
  * **Spring Data JPA:** For database interactions.
  * **Hibernate:** ORM tool for mapping Java objects to database tables.
  * **MySQL/PostgreSQL:** Relational database management system.
  * **Maven:** Build automation tool.

* **Frontend:**

  * **Thymeleaf:** Server-side Java template engine for rendering HTML.
  * **Bootstrap:** CSS framework for responsive design.

* **Security:**

  * **Spring Security:** For authentication and authorization.
  * **JWT (JSON Web Tokens):** For stateless authentication.

## 🚀 Features

* **User Authentication:**

  * Secure registration and login functionality.
  * Password encryption using BCrypt.

* **Blog Management:**

  * Create, read, update, and delete blog posts.
  * Rich text editor for composing blog content.

* **User Roles:**

  * Role-based access control (e.g., Admin, Author, Reader).

* **Responsive Design:**

  * Mobile-friendly interface using Bootstrap.

* **Search Functionality:**

  * Search blog posts by title or content.

* **Pagination:**

  * Paginated list of blog posts for better user experience.

## 📂 Project Structure

```
Blogify-Blog-Application/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── blogify/
│   │   │           ├── controller/
│   │   │           ├── model/
│   │   │           ├── repository/
│   │   │           ├── service/
│   │   │           └── BlogifyApplication.java
│   │   └── resources/
│   │       ├── static/
│   │       ├── templates/
│   │       └── application.properties
├── pom.xml
└── README.md
```

## 🧰 Installation and Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/sanskritisahu21/Blogify-Blog-Application.git
   cd Blogify-Blog-Application
   ```

2. **Configure the database:**

   * Create a MySQL/PostgreSQL database named `blogify`.
   * Update the `application.properties` file with your database credentials:

     ```properties
     spring.datasource.url=jdbc:mysql://localhost:3306/blogify
     spring.datasource.username=your_username
     spring.datasource.password=your_password
     spring.jpa.hibernate.ddl-auto=update
     ```

3. **Build and run the application:**

   ```bash
   mvn spring-boot:run
   ```

4. **Access the application:**

   Open your browser and navigate to `http://localhost:8080`.

## 🧪 Testing

* The application includes unit and integration tests using JUnit and Spring Boot Test.
* To run the tests:

  ```bash
  mvn test
  ```

## 📈 Future Enhancements

* **Commenting System:** Allow users to comment on blog posts.
* **Image Uploads:** Enable image uploads for blog posts.
* **Rich Text Editor:** Integrate a WYSIWYG editor for better content creation.
* **API Integration:** Expose RESTful APIs for external integrations.
* **Dockerization:** Containerize the application using Docker for easier deployment.
