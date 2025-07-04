
# 🏋️‍♂️ Fitness Tracking Microservices

A microservices-based fitness tracking application that allows users to manage workouts, track goals, and monitor health metrics in a modular, scalable, and robust system architecture.

---

## 🚀 Overview

This project is a fitness application built using a **Microservices Architecture**. It consists of independently deployable services handling different functionalities such as user management, workout logging, goal tracking, and analytics.

Each service communicates via **REST APIs** and registers with **Eureka Discovery Server**. Built with **Spring Boot**, the system also features **API Gateway**, **PostgreSQL**, and **MongoDB** for hybrid data handling.

---

## 🧱 Microservices Breakdown

| Service              | Description                                  | Tech Stack                          |
|----------------------|----------------------------------------------|-------------------------------------|
| **API Gateway**       | Routes requests to appropriate services       | Spring Cloud Gateway                |
| **Eureka Server**     | Service discovery and registration            | Netflix Eureka                      |
| **User Service**      | Manages user profiles and authentication      | Spring Boot, PostgreSQL             |
| **Workout Service**   | Logs daily workout routines                   | Spring Boot, MongoDB                |
| **Goal Service**      | Handles fitness goal creation and progress    | Spring Boot, PostgreSQL             |
| **Activity Service**  | Tracks daily fitness activities               | Spring Boot, MongoDB                |

---

## 🛠️ Tech Stack

- **Java 17**
- **Spring Boot 3.x**
- **Spring Cloud (Eureka, Gateway)**
- **PostgreSQL & MongoDB**
- **Docker (for containerization)**
- **Maven**
- **Lombok**
- **Spring Security (basic setup)**

---

## 📦 Folder Structure

```

fitness-tracking-microservices/
│
├── api-gateway/
├── eureka-server/
├── user-service/
├── workout-service/
├── goal-service/
├── activity-service/
└── README.md

````

---

## 🔧 How to Run

1. **Start Eureka Server**
   ```bash
   cd eureka-server
   mvn spring-boot:run
````

2. **Start API Gateway**

   ```bash
   cd api-gateway
   mvn spring-boot:run
   ```

3. **Start Other Services (in separate terminals)**

   ```bash
   cd user-service && mvn spring-boot:run
   cd workout-service && mvn spring-boot:run
   cd goal-service && mvn spring-boot:run
   cd activity-service && mvn spring-boot:run
   ```

4. **Access Eureka Dashboard**

   * [http://localhost:8761](http://localhost:8761)

---

## 📊 Features

* 🔐 Secure user sign-up and login (basic auth)
* 📅 Log and track fitness activities daily
* 🎯 Set and monitor fitness goals
* 📈 View analytics of workout history
* 🔄 Service discovery and seamless routing with API Gateway

---

## 🧑‍💻 Author

> 👤 **Agnik Mondal**
> 🎓 Computer Science & Engineering
> 🏆 Hackathon Winner | MERN & Java Enthusiast
> 🔗 [GitHub](https://github.com/agnik2003) | [LinkedIn](https://www.linkedin.com/in/agnik-mondal-11a37828a/)

---

## 📌 Future Improvements

* ✅ Add JWT-based authentication
* ✅ Swagger/OpenAPI documentation for APIs
* 📲 Frontend in React.js
* 📈 Integrate Prometheus + Grafana for metrics
* ☁️ Deploy to AWS/GCP with CI/CD

---

## 📃 License

This project is open-source and available under the [MIT License](LICENSE).

---
