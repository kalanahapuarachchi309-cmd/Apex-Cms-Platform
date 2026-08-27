# APEX-CMS: Platform Services Foundation

> **GitHub Repository About Description:**
> *Spring Cloud Platform Infrastructure for APEX-CMS containing API Gateway, Config Server, and Eureka Service Registry.*

---

## 👨‍🎓 Student & Submission Information

| Field | Details |
| :--- | :--- |
| **Student Name** | Kalana Maduranaga |
| **Student Number** | 241711018 |
| **GCP Project ID** | `apex-cms-506311` |
| **GCP Region** | `asia-south1` (Mumbai) |

---

## 📖 Overview

The **Platform Services** layer provides the essential distributed infrastructure foundation for the APEX-CMS microservices ecosystem. It orchestrates service registration, centralized dynamic configuration, and intelligent routing.

### Platform Modules
1. **Config Server (`port: 9000`)**: Spring Cloud Config Server providing externalized, centralized configuration management.
2. **Service Registry (`port: 9001`)**: Netflix Eureka Server managing dynamic registration and heartbeat health checks.
3. **API Gateway (`port: 7000`)**: Spring Cloud Gateway providing reactive non-blocking reverse proxy routing, load balancing, and CORS handling.

---

## 🧰 Technology Stack

- **Java Version:** Java 25 / OpenJDK 21
- **Framework:** Spring Boot 4.1.0, Spring Cloud 2025.1.2
- **Build Tool:** Apache Maven
- **Core Components:** Spring Cloud Gateway, Spring Cloud Config Server, Netflix Eureka Server

---

## 🚀 Startup Instructions

Start the platform services in the following order:

```bash
# 1. Start Config Server
cd platform/config-server
mvn spring-boot:run

# 2. Start Service Registry
cd platform/service-registry
mvn spring-boot:run

# 3. Start API Gateway
cd platform/api-gateway
mvn spring-boot:run
```\n