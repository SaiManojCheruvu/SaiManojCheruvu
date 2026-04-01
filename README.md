<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&pause=1000&color=58A6FF&center=true&vCenter=true&width=650&lines=Hey+there%2C+I'm+Sai+Manoj+%F0%9F%91%8B;Full-Stack+Engineer+%7C+Boston%2C+MA;Go+%7C+React+%7C+TypeScript+%7C+Java;System+Design+%7C+Concurrency+%7C+Real-time" alt="Typing SVG" />
</h1>

<p align="center">
  <a href="https://www.linkedin.com/in/saimanojcheruvu/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://leetcode.com/u/Manoj-Cheruvu-02070979/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" /></a>
  <a href="https://medium.com/@saimanojcheruvu"><img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" /></a>
  <a href="mailto:saimanojcheruvu@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

---

## 🧑‍💻 About Me

Software Engineer with **5+ years** of experience building scalable full-stack applications — currently based in Boston, MA.

I care about building systems that are correct under pressure: concurrent writes, real-time updates, race conditions. I use this GitHub to study and implement those patterns hands-on.

- 🔨 **Primary stack**: Go, React/TypeScript, Java, PostgreSQL, Redis
- 📐 **Design focus**: Concurrency safety, system design patterns, OOP principles
- 📡 **Real-time systems**: WebSocket pub/sub, collaborative tooling, event-driven architecture
- ☁️ **AWS Certified Cloud Practitioner** (CLF-002)

---

## 🗂️ Public Repos

### 🔒 [Pet-Store](https://github.com/SaiManojCheruvu/Pet-store) — Concurrent Purchase Safety
> Full-stack pet marketplace (Go + React/TypeScript + GraphQL + PostgreSQL) demonstrating safe handling of concurrent data updates

**The core challenge:** Multiple buyers trying to purchase the same pet simultaneously. Solved at two levels:

- **Code-level locking** — `sync.Mutex` on the service layer (`PetService`, `SinglePurchaseStrategy`, `BatchPurchaseStrategy`) and `sync.RWMutex` on the repository layer, preventing goroutine races on purchase state
- **DB-level locking** — PostgreSQL `SELECT FOR UPDATE` reservation pattern: atomically checks availability and marks purchased in a single transaction, so no two requests can double-sell the same record
- **Strategy pattern** — `PurchaseStrategy` interface with separate `SinglePurchaseStrategy` and `BatchPurchaseStrategy` implementations; `PurchaseService` hot-swaps strategies safely using `sync.RWMutex`
- **Stack**: Go (net/http, sync), PostgreSQL, GraphQL, React/TypeScript, Docker Compose

---

### 📡 [High-Level-Design](https://github.com/SaiManojCheruvu/High-Level-Design) — System Design Implementations
> Practical implementations of system design concepts from [Hello Interview](https://www.hellointerview.com/learn/system-design) — theory turned into running code

- **Real-time collaborative notes** — WebSocket pub/sub for live data propagation across distributed clients, with conflict handling
- Each implementation includes trade-off analysis and scaling notes alongside working code
- Dockerized for local experimentation
- 📝 [Medium: Real-time Data Patterns](https://medium.com/@saimanojcheruvu/real-time-data-patterns-c2502ee410ba)
- **Stack**: JavaScript, Java, CSS, Docker

---

### 🍰 [CakeStoreApp](https://github.com/SaiManojCheruvu/CakeStoreApp) — Full-Stack TypeScript App
> End-to-end store application with a clean frontend/backend project structure
- **Stack**: TypeScript (72%), CSS, JavaScript

---

### 📐 [Object-Oriented-Designs](https://github.com/SaiManojCheruvu/Object-Oriented-Designs) — Design Patterns in Java
> OOP coursework covering 17 design patterns with JUnit testing and lambda expression refactoring

Patterns covered include Singleton, State, Multicast, Composite, Proxy, Visitor, Command, and Strategy (with Comparators), plus their lambda-expression equivalents.

- **Stack**: Java (100%)

---

### 📈 [StockPricePredictionUsingTimeSeries](https://github.com/SaiManojCheruvu/StockPricePredictionUsingTimeSeries)
> Time series analysis and stock price forecasting — **Stack**: R

---

## 🛠️ Tech Stack

**Languages**

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Redux](https://img.shields.io/badge/Redux-764ABC?style=flat-square&logo=redux&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Material UI](https://img.shields.io/badge/MUI-007FFF?style=flat-square&logo=mui&logoColor=white)
![Apollo Client](https://img.shields.io/badge/Apollo_Client-311C87?style=flat-square&logo=apollographql&logoColor=white)

**Backend & Architecture**

![Go](https://img.shields.io/badge/Go_Microservices-00ADD8?style=flat-square&logo=go&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![WebSockets](https://img.shields.io/badge/WebSockets-010101?style=flat-square&logo=socketdotio&logoColor=white)

**Databases**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)

**Cloud & DevOps**

![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI%2FCD-FC6D26?style=flat-square&logo=gitlab&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)

---

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=saimanojcheruvu&style=flat-square&color=58A6FF" />
</p>

<p align="center"><i>"Build i
