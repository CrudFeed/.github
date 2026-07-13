<table align="center">
  <tr>
    <td align="center">
      <img width="100" height="100" alt="CrudFeed" src="https://github.com/user-attachments/assets/8b7a41f5-24de-47a4-b90d-b9d9f1a2182d"><br>
      <sub><b>CrudFeed</b></sub>
    </td>
    <td align="center">
      <img width="100" height="100" alt="CLI" src="https://github.com/user-attachments/assets/bfd3482e-64d4-4a1c-98b4-cdfa91d20fcb"><br>
      <sub><b>CrudFeed CLI</b></sub>
    </td>
    <td align="center">
      <img width="100" height="100" alt="Web" src="https://github.com/user-attachments/assets/1c781f4c-82d8-4498-b9d5-593336468823"><br>
      <sub><b>CrudFeed Web</b></sub>
    </td>
  </tr>
</table>

<br>

<p align="center">
  Lightweight messaging and social content ecosystem. Java-based, clean multi-layered architecture.<br>
</p>

<p align="center">
  This repository acts as a landing page. The actual source code lives in separate repos under the organization.
</p>

<br>

<p align="center">
  <a href="https://github.com/CrudFeed/CrudFeed-CLI"><img src="https://img.shields.io/badge/CLI_Version-2.0_In_Dev-blue?style=for-the-badge&logo=git&logoColor=white" alt="CLI Version"></a>
  <a href="https://github.com/CrudFeed/CrudFeed-WEB"><img src="https://img.shields.io/badge/WEB_Version-Pre_Alpha_In_Dev-orange?style=for-the-badge&logo=git&logoColor=white" alt="Web Version"></a>
  <img src="https://img.shields.io/badge/More_Versions-In_the_Future-lightgrey?style=for-the-badge&logo=git&logoColor=white" alt="More Versions In the future">
</p>

<p align="center">
  <sub>🗄 Do you want to see how we started? <a href="https://github.com/M1reXx/CrudFeed">Check the archive</a>.</sub>
</p>

<br>

<p align="center">
  <font size="7"><b>Powered by</b></font>
</p>

<p align="center">
  <img width="40" src="https://img.shields.io/badge/%20-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
  <img width="40" src="https://img.shields.io/badge/%20-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img width="40" src="https://img.shields.io/badge/%20-59666C?style=flat-square&logo=hibernate&logoColor=white" alt="Hibernate">
  <img width="40" src="https://img.shields.io/badge/%20-C71A36?style=flat-square&logo=apachemaven&logoColor=white" alt="Maven">
  <img width="40" src="https://img.shields.io/badge/%20-000000?style=flat-square&logo=intellijidea&logoColor=white" alt="IDEA">
  <img width="40" src="https://img.shields.io/badge/%20-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux">
</p>

---

## 🧱 Architecture

Both versions share the same layered structure — clean separation, no shortcuts:

```
┌─────────────────┐
│     Servlet     │  ← handles HTTP requests / CLI commands
├─────────────────┤
│     Service     │  ← business logic, validation
├─────────────────┤
│    Repository   │  ← Hibernate-backed data access
├─────────────────┤
│      Entity     │  ← JPA entities (Lombok-powered)
└─────────────────┘
         │
         ▼
     PostgreSQL
```

Each layer only talks to the one directly below it. No entity is ever exposed straight to a servlet, no repository ever contains business logic.

---

## 🚀 Getting Started

```bash
git clone https://github.com/CrudFeed/CrudFeed-CLI.git
# or
git clone https://github.com/CrudFeed/CrudFeed-WEB.git
```

Set up PostgreSQL, configure your Hibernate connection settings, and build with Maven:

```bash
mvn clean install
```

---

## 🚧 Status

At this time, the project is being developed in secret

---
