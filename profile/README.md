<p align="center">
  <img width="120" height="120" alt="CrudFeed" src="https://github.com/user-attachments/assets/8b7a41f5-24de-47a4-b90d-b9d9f1a2182d">
</p>

<h1 align="center">CrudFeed</h1>

<p align="center">
  A lightweight social network built with a Java backend architecture and IT design.
</p>

<br>

<p align="center">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white" alt="Hibernate">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/JavaFX-007396?style=flat-square&logo=openjdk&logoColor=white" alt="JavaFX">
  <img src="https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white" alt="Maven">
  <img src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=flat-square&logo=intellijidea&logoColor=white" alt="IntelliJ IDEA">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
</p>

<br>

<p align="center">
  <sub>🗄 Do you want to see how we started? <a href="https://github.com/M1reXx/CrudFeed">Check the archive</a>.</sub>
</p>

---

<br>

> This repository is a landing page. The actual source code lives in separate repositories under the organization.

<br>

## 📦 Modules

| Module | Stack | Status | Access |
| :--- | :--- | :--- | :--- |
| **GUI** | Java, JavaFX | [![GUI](https://img.shields.io/badge/IN_DEV-brightgreen?style=for-the-badge&logo=git&logoColor=white)](https://github.com/CrudFeed/CrudFeed-GUI) | 🔒 Private |
| **CLI** | Java | [![CLI](https://img.shields.io/badge/REVISION-blue?style=for-the-badge&logo=git&logoColor=white)](https://github.com/CrudFeed/CrudFeed-CLI) | 🔒 Private |
| **Android** | Kotlin, Gradle | [![Android](https://img.shields.io/badge/PLANNED-lightgrey?style=for-the-badge&logo=git&logoColor=white)](https://github.com/CrudFeed/CrudFeed-ANDROID) | 🔒 Private |
| **Web** | HTML5, CSS, JavaScript | [![Web](https://img.shields.io/badge/ON_HOLD-orange?style=for-the-badge&logo=git&logoColor=white)](https://github.com/CrudFeed/CrudFeed-WEB) | 🔒 Private |
| **CORE** | Java, Spring Framework, Hibernate, ProGuard | ![CORE](https://img.shields.io/badge/CLOSED_SOURCE-red?style=for-the-badge&logo=git&logoColor=white) | 🔒 Closed |
| **Server** | Java, Spring Boot | [![Server](https://img.shields.io/badge/REVISION-blue?style=for-the-badge&logo=git&logoColor=white)](https://github.com/CrudFeed/CrudFeed-SERVER) | 🔒 Private |

<br>

## 🧱 Architecture

All modules share the same layered structure:

```
┌─────────────────┐
│    Controller   │  ← REST endpoints, receives DTOs
├─────────────────┤
│     Service     │  ← business logic, validation
├─────────────────┤
│    Repository   │  ← Hibernate-backed data access
├─────────────────┤
│      Entity     │  ← JPA entities (Lombok-powered)
└────────┬────────┘
         ▼
     PostgreSQL
```

Each layer only talks to the one directly below it. No entity is ever exposed straight to a servlet, and no repository ever contains business logic.

<br>

## 🚀 Getting Started

```bash
git clone https://github.com/CrudFeed/<repository_name>.git
cd <repository_name>
```

Set up PostgreSQL, configure your Hibernate connection settings, then build with Maven:

```bash
mvn clean install
```
<br>

## 🚧 Status

The project is currently being developed in private.
