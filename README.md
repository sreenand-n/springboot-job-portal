# Job Portal Web Application

A simple Job Portal Web Application built using Spring Boot, Spring MVC, JSP, JSTL, and Bootstrap. This project was developed to understand the complete MVC workflow, form handling, dependency injection, and dynamic data rendering in Spring applications.

## Features

* View all available job postings
* Add a new job posting
* Display submitted job details
* Dynamic data rendering using JSP and JSTL
* Layered architecture (Controller → Service → Repository)
* Form data binding with Spring MVC

## Tech Stack

### Backend

* Java
* Spring Boot
* Spring MVC

### Frontend

* JSP
* JSTL
* Bootstrap 5

### Build Tool

* Maven

### Utilities

* Lombok

## Project Structure

src/main/java
├── com/example/JobApp
│   ├── model
│   │   └── JobPost.java
│   ├── repo
│   │   └── JobRepo.java
│   ├── service
│   │   └── JobService.java
│   ├── JobController.java
│   └── JobAppApplication.java

src/main/resources
├── META-INF/resources
│   ├── home.jsp
│   ├── addjob.jsp
│   ├── success.jsp
│   └── viewalljobs.jsp
├── static/css
│   ├── style.css
│   └── style1.css
└── application.properties

pom.xml

## Application Flow

1. User opens the Home Page.
2. User can view existing jobs or add a new job.
3. Form data is submitted to the controller.
4. Spring MVC automatically binds form data to a JobPost object.
5. The Service layer processes the request.
6. The Repository layer manages the job data.
7. Data is rendered dynamically in JSP pages using JSTL and Expression Language (EL).

## Learning Outcomes

Through this project, I practiced:

* Spring MVC Architecture
* Dependency Injection using @Autowired
* Form Handling in Spring MVC
* Model and View Communication
* JSP Expression Language (EL)
* JSTL Tags
* Layered Application Design
* Bootstrap Integration

## Current Limitation

This project currently uses an in-memory ArrayList to store job data. Data will be lost when the application restarts.


## How to Run

1. Clone the repository

git clone https://github.com/sreenand-n/springboot-job-portal.git

2. Navigate to the project directory

cd springboot-job-portal

3. Run the application

mvn spring-boot:run

4. Open in browser

http://localhost:8080

