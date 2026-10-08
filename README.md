# 🚩 Switchly

**Switchly** is a real-time Feature Flag Management API built with Java 21 and Spring Boot. It provides a multi-tenant hierarchy (**Organizations → Projects → Feature Flags**) allowing engineering teams to dynamically roll out, test, and toggle feature flags without re-deploying code.

---

## ✨ Features

- **Multi-Tenant Architecture:** Manage flags across organizations and individual projects.
- **Dynamic Flag Operations:** Create, retrieve, update state, and delete feature flags.
- **Centralized Exception Handling:** Standardized RESTful error responses for resource conflicts and missing records.
- **Clean In-Memory Persistence:** Fast, lightweight repository pattern ready for database integration.

---

## 🛠️ Tech Stack

- **Language:** Java 21
- **Framework:** Spring Boot 3
- **Build System:** Maven
- **Validation:** Jakarta Bean Validation

---

## 🚀 API Endpoints Overview

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| **POST** | `/api/v1/orgs` | Create an organization |
| **GET** | `/api/v1/orgs` | List all organizations |
| **GET** | `/api/v1/orgs/{orgId}` | Get organization details |
| **POST** | `/api/v1/orgs/{orgId}/projects` | Create a project under an organization |
| **GET** | `/api/v1/orgs/{orgId}/projects` | List all projects in an organization |
| **GET** | `/api/v1/projects/{projectId}` | Get project details |
| **POST** | `/api/v1/projects/{projectId}/flags` | Create a feature flag in a project |
| **GET** | `/api/v1/projects/{projectId}/flags` | List all flags for a project |
| **GET** | `/api/v1/flags/{flagId}` | Get details of a specific flag |
| **PUT** | `/api/v1/flags/{flagId}/state` | Toggle a flag's enabled state |
| **DELETE** | `/api/v1/flags/{flagId}` | Delete a feature flag |

---

## 💻 Getting Started

### Prerequisites
- **JDK 17** or higher

### Running the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/aaryan1005/com.switchly
   cd switchly
