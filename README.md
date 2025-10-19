# Student Records Dashboard

A simple and professional single-table CRUD (Create, Read, Update, Delete) application built using Spring Data JPA and the modern Java UI framework, Vaadin. The project is built with Spring Boot for easy setup and development.

This application serves as an excellent example of a fully Java-based front-end with deep full-stack integration, ideal for learning how to connect a component-based UI to a JPA-backed backend.

> **Note:** For larger, more complex applications, consider applying common design patterns for your UI code, such as Model-View-Presenter (MVP).

---

## ✨ Features & Technology

### Key Features

- **Full-Stack Java:** The entire application, from the database connection to the client-side UI, is written in Java (no separate HTML/CSS/JS required).  
- **CRUD Operations:** Implements core Create, Read, Update, and Delete functions on the Student Records data model.  
- **Professional UI:** Component-based UI with modern aesthetics, using the recommended Lumo theme (`@Theme("lumo")`).  
- **Secure Builds:** Uses HTTPS for all Maven dependencies to ensure secure and reliable builds.  
- **Extensible:** Easy to adapt and customize for other business domains or data models.  

### Tech Stack

| Component    | Technology       | Details                                               |
|-------------|-----------------|-------------------------------------------------------|
| Frontend    | Vaadin           | Java-based component UI framework                     |
| Backend     | Spring Boot      | Provides configuration and application setup         |
| Persistence | Spring Data JPA  | Handles database access and repositories             |
| Database    | H2 (in-memory)   | Default for easy development/testing; supports MySQL/PostgreSQL |
| Build Tool  | Maven            | Manages project lifecycle and dependencies           |
| Java Version| 17+              | Recommended for modern Spring/Vaadin features       |

---

## 🚀 How to Run Locally

You can run the application using your IDE, Maven, or as an executable JAR.

### 1. Clone the Project

```bash
git clone https://github.com/ravi-kumar-chinta/Student-Records-Dashboard.git
cd Student-Records-Dashboard
```
## 2. Run Options

### A. Run in an IDE
Open the project in your favorite IDE (IntelliJ IDEA, Eclipse, VS Code).  
Run the main `Application` class.

### B. Run using Maven (Development Mode)
```bash
mvn spring-boot:run
```
This is the fastest way to run and usually provides hot-reload during development.

## C. Build a JAR and Run Anywhere

The project can be packaged as a single, runnable JAR file that can execute on any computer with Java installed.

**Package the application:**
```bash
mvn package
```
## Run the JAR:
```bash
java -jar target/Student-Records-Dashboard-0.0.1-SNAPSHOT.jar
```
## 3. Open in Browser

After the application starts (using any of the methods above), open your web browser at:
```bash
http://localhost:8080
```
☁️ Deployment to Cloud / PaaS

The built JAR file is cloud-ready and can be deployed easily on modern platforms. The following example uses Cloud Foundry (cf):

Ensure the project is packaged:
```bash
mvn install
```

Deploy using the Cloud Foundry CLI:

`cf push choose-name-for-your-server -p target/*.jar -b https://github.com/cloudfoundry/java-buildpack.git`

Note: Replace choose-name-for-your-server with a unique, memorable name for your application.
If using Java 7 or older compatibility (see the java7 branch), you may be able to omit the -b flag.

# 📝 Repository Notes

This project is an ideal showcase for resumes and portfolios demonstrating proficiency in Java full-stack development, modern component-based UI, and Spring Boot integration.

### Remote Configuration
```bash
git remote add origin https://github.com/ravi-kumar-chinta/Student-Records-Dashboard.git
```
## Thank You
Thank you for checking out this project! Contributions, feedback, and suggestions are always welcome. Happy coding!