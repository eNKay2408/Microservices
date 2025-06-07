<div align="center">

  # ☁️ Microservices

  *A Simple Demo of Microservices Architecture Using Some Popular Technologies* 🐳

  ![Spring](https://img.shields.io/badge/Spring-white?style=for-the-badge)
  ![Data JPA](https://img.shields.io/badge/Data_JPA-white?style=for-the-badge)
  ![Data MongoDB](https://img.shields.io/badge/Data_MongoDB-white?style=for-the-badge)
  ![Test Containers](https://img.shields.io/badge/TestContainers-white?style=for-the-badge)

  ![Netflix Eureka](https://img.shields.io/badge/Netflix_Eureka-white?style=for-the-badge)
  ![API Gateway](https://img.shields.io/badge/API_Gateway-white?style=for-the-badge)
  ![Keycloak](https://img.shields.io/badge/Keycloak-white?style=for-the-badge)
  ![Resilience4J](https://img.shields.io/badge/Resilience4J-white?style=for-the-badge)

  ![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-white?style=for-the-badge)
  ![Docker](https://img.shields.io/badge/Docker-white?style=for-the-badge)
  ![Prometheus & Grafana](https://img.shields.io/badge/Prometheus_&_Grafana-white?style=for-the-badge)
  ![Postman](https://img.shields.io/badge/Postman-white?style=for-the-badge)

  
  <img width="600px" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967434/Microservices/0-AllServices.png">

</div>

## 📘 Table of Contents
1. [Introduction](#introduction) 🧟
2. [Technologies](#technologies) 💻
3. [Features](#features) 🔎
4. [Development](#development) ✈️
5. [Acknowledgements](#acknowledgements) 💙
6. [Contact](#contact) 🌐

## 🧟 <a name="introduction">Introduction</a>

This has truly been one of the most diverse and challenging projects I’ve ever worked on. From the start, I was excited knowing I’d get to learn and implement many cutting-edge technologies in this project. However, this also meant the process would be incredibly difficult, as every part of the project introduced something entirely new. Unlike my previous projects, where adapting in the early stages was enough, here I found myself constantly facing errors and struggling to fix them. The learning curve was steep because many of these technologies are commonly used in professional environments, making the experience both overwhelming and rewarding.

Through this project, I am immensely grateful for the knowledge I’ve gained. I now have a deeper understanding of what it means to be a Java developer - it’s not just about writing code, like in past projects, but also about integrating new technologies and configuring systems to meet demands for optimization and usability. This experience made me realize that the more I learn, the more I see how much I still have to improve, constantly adapting to meet the challenges of a professional environment. Although this project is just a demo, it has given me a clearer picture of the complications that occur behind the scenes in large-scale enterprises. I’m grateful for this journey and ready to keep pushing forward!

## 💻 <a name="technologies">Technologies</a>

- **Spring Boot**: Simplifies development by providing pre-configured templates and embedded servers.
- **Spring Data JPA & MongoDB**: Provides a layer of abstraction to work with databases, simplifying the process of writing queries.
- **Test Containers**: Simplifies integration testing by providing a way to run containers in JUnit tests.
- **Netflix Eureka**: A service registry that allows microservices to find and communicate with each other.
- **API Gateway**: Routes requests to the appropriate service and provides a single point of entry for clients.
- **Keycloak**: An open-source identity and access management solution that provides authentication and authorization services.
- **Resilience4J**: Provides fault tolerance and resilience to microservices by implementing patterns like circuit breakers.
- **Apache Kafka**: A distributed event streaming platform that allows microservices to communicate asynchronously.
- **Docker**: A platform that allows developers to build, ship, and run all services in containers.
- **Prometheus & Grafana**: A monitoring and alerting toolkit that provides metrics and visualization for services.
- **Postman**: A collaboration platform for API development that simplifies the process of testing APIs.

## 🔎 <a name="features">Features</a>

**🔷 Get Product:** Retrieves a product from the database.

**🔷 Post Product:** Adds a new product to the database.

**🔷 Post Order:** Adds a new order to the database.

**🔷 JUnit Test:** Tests the product service for creating and retrieving products.

**🔷 Discovery Server:** Registers services such as Product, Order, Inventory, and Notification.

**🔷 API Gateway:** Routes requests to the appropriate service with endpoints such as /api/product.

**🔷 Authentication & Authorization:** Uses Keycloak to authenticate and authorize requests with JWT.

**🔷 Circuit Breakers:** Uses Resilience4J to implement circuit breakers, enhancing fault tolerance.

**🔷 Event Streaming:** Kafka to send and receive messages asynchronously between the Order and Notification services.

**🔷 Containers:** Docker to run all services in containers for easy deployment.

**🔷 Monitoring:** Prometheus and Grafana to monitor and visualize metrics for services. 

<img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967434/Microservices/0-AllServices.png" alt="All Services"> <img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967434/Microservices/1-GetProduct.png" alt="Get Product">

<img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967434/Microservices/2-PostProduct.png" alt="Post Product"> <img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967433/Microservices/3-PostOrder.png" alt="Post Order">

<img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967433/Microservices/4-Eureka.png" alt="Eureka"> <img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967433/Microservices/5-Keycloak.png" alt="Keycloak">

<img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967433/Microservices/6-Prometheus.png" alt="Prometheus"> <img width="49%" src="https://res.cloudinary.com/dvzhmi7a9/image/upload/v1728967434/Microservices/7-Grafana.png" alt="Grafana">

## ✈️ <a name="development">Development</a>

### 📋 Prerequisites
- [Java](https://www.oracle.com/java/)
- [Docker](https://www.docker.com/)
- [Postman](https://www.postman.com/)
- [Maven](https://maven.apache.org/)

### 🐾 Steps

#### 1. Clone the repository
```bash
git clone https://github.com/eNKay2408/Microservices.git
cd Microservices
```

#### 2. Change Docker Hub username
- Open `pom.xml` in the root directory.
- Replace `enkay2408` with your Docker Hub username.

#### 3. Build images and upload to Docker Hub
```bash
mvn clean compile jib:build
```

#### 4. Run Docker Compose to start services
```bash
docker compose up
```

#### 5. Access services
- Product Service: `http://localhost:8181/api/product`
- Order Service: `http://localhost:8181/api/order`
- Inventory and Notification Services: logs in container.

### ❔ Questions

####  How do I get credentials for Keycloak?
- Open `http://localhost:8080` and log in with `admin/admin`.
- Go to `Clients` and click on `spring-cloud-client`.
- Go to `Credentials` and `Regenerate Secret`.

#### How do I add credentials to Postman?
- Open Postman and create a new request.
- Go to `Authorization` and select `OAuth 2.0`.
- Enter the following details:
  - `Token Name`: Keycloak
  - `Grant Type`: Client Credentials
  - `Access Token URL`: `http://keycloak:8080/realms/spring-boot-microservices-realm/protocol/openid-connect/token`
  - `Client ID`: spring-cloud-client
  - `Client Secret`: [Client Secret from Keycloak]
  - `Scope`: openid offline_access
  - `Client Authentication`: Send as Basic Auth header
  - Finally, Click on `Get New Access Token` and `Use Token`.

#### How do I create a dashboard in Grafana?
- Open `http://localhost:3000` and log in with `admin/admin`.
- Go to `Connections` and `Data sources`.
- Click on `Add data source` and select `Prometheus`.
- Enter the following details:
  - `Name`: Prometheus
  - `URL`: `http://prometheus:9090`
  - Click on `Save & Test`.
- Go to `Dashboard` and click on `New Dashboard`.
- Click on `Import dashboard` and paste the JSON from `Grafana_Dashboard.json` in the root directory.
- Then, click on `Load` and the dashboard will be created.


### 🌟 I hope it saves you time debugging, as I’ve already gone through the tough parts for you, `XD`. And if you found it useful, a star on this GitHub repository would mean the world to me!

## 💙 <a name="acknowledgements">Acknowledgements</a>

- **[Programming Techie](https://www.youtube.com/@ProgrammingTechie):** For the amazing [tutorial](https://www.youtube.com/watch?v=mPPhcU7oWDU) on microservices and Spring Boot. He has been a great mentor throughout this project.
- **[Spring Boot](https://spring.io/projects/spring-boot):** For providing a simple and efficient way to build microservices.
- **[Spring Data](https://spring.io/projects/spring-data):** For simplifying the process of working with databases.
- **[Spring Cloud](https://spring.io/projects/spring-cloud):** For providing tools to build microservices.
- **[Test Containers](https://www.testcontainers.org/):** For providing a way to run containers in JUnit tests.
- **[Keycloak](https://www.keycloak.org/):** For providing authentication and authorization services.
- **[Apache Kafka](https://kafka.apache.org/):** For providing a distributed event streaming platform.
- **[Docker](https://www.docker.com/):** For providing a platform to run services in containers.
- **[Postman](https://www.postman.com/):** For providing a platform to test APIs.

## 🌐 <a name="contact">Contact</a>

- **Name:** Nguyen Phan Duc Khai - **eNKay**
- **Portfolio:** [enkay.tech](https://enkay.tech)
- **LinkedIn:** [en-kay](https://www.linkedin.com/in/en-kay/)
- **Email:** [enkay.work@outlook.com](mailto:enkay.work@outlook.com)
