# Schedule Hub Backend (Spring Boot + PostgreSQL)

<p align="center">
  <a href="https://opensource.org/licenses/MIT" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT License" />
  </a>
  <a href="https://spring.io/projects/spring-boot" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/spring%20boot-3.x-green" alt="Spring Boot" />
  </a>
  <a href="https://www.postgresql.org/" target="_blank" rel="noopener noreferrer">
    <img src="https://img.shields.io/badge/postgresql-15-blue" alt="PostgreSQL" />
  </a>
</p>

Backend service for the **Schedule Hub App**, providing secure APIs for managing appointments, events, user accounts, and scheduling conflict detection. Built with **Spring Boot** and **PostgreSQL**, it powers the Angular frontend with REST endpoints and real-time validation.

---

## Features
- **User & Admin Management** – Role-based access to protect sensitive data and features.
- **Appointment & Event Scheduling** – Create, update, and delete with validation.
- **Conflict Detection** – Smart buffer rules for virtual and in-person events.
- **Database Integration** – PostgreSQL persistence with JPA/Hibernate.
- **Testing** – Unit tests for entities, services, and scheduling logic.

---

## Tech Stack
- **Backend:** Spring Boot 3.x, Java 17  
- **Database:** PostgreSQL 15  
- **Build Tool:** Maven  
- **APIs:** RESTful JSON endpoints  
- **Testing:** JUnit 5, Mockito  

---

## Project Structure
```
khepra-backend/
├── src/main/java/com/khepra/...
│   ├── controller   # REST controllers
│   ├── dto          # Data Transfer Objects
│   ├── entity       # JPA entities
│   ├── repository   # Spring Data JPA Repositories
│   ├── service      # Business logic
│   └── utils        # Validation & helpers
├── src/test/java/... # Unit tests
└── pom.xml          # Maven configuration
```

---

## Getting Started
### Prerequisites
- Java 17+
- Maven 3.8+
- PostgreSQL 15

### Setup
1. Clone the repo:
```bash
git clone https://github.com/quinise/ScheduleHub-backend.git
cd khepra-backend
```

2. Configure your database in `application.properties`:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/khepra
spring.datasource.username=your_username
spring.datasource.password=your_password
```

3. Run the application:
```bash
mvn spring-boot:run
```

---

## Testing

Run the unit tests with:
```bash
mvn test
```

---

## Related Repositories

- **Frontend:** [ScheduleHub-frontend](https://github.com/quinise/ScheduleHub-frontend) – Angular 19 client

---

## License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
