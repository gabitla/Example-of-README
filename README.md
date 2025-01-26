# AppSchool

## Description
AppSchool is a system designed to optimize the administration and organization of small schools and academies, offering an integrated solution that centralizes academic and administrative processes. Focused on digitization and modernization, it aims to solve common problems such as information dispersion, manual processes, and inefficient communication.

---

## Project Status
The project is currently under development.

---

## Key Features
1. **User Management**: Registration and management of students and teachers.
2. **Grades and Attendance**: Detailed and real-time tracking.
3. **Schedules and Courses**: Efficient planning to optimize time.
4. **Communication**: Interactive chat, real-time notifications, and email alerts.
5. **Report Generation**: Academic performance analysis with automated reports.

---

## Architecture and Technologies

### Microservices
The system is designed as a microservice-based architecture deployed on AWS. The microservices include:
- User management
- Course management
- Schedule management
- Notification service
- Report generation

### Programming Languages
- JavaScript
- Python
- Go
- Ruby
- PHP
  
* [![React][React.js]][React-url]
* [![Vue][Vue.js]][Vue-url]
* [![Angular][Angular.io]][Angular-url]
* [![Python][Python.com]][Python-url]

  <p align="right">(<a href="#readme-top">back to top</a>)</p>

### Databases
- PostgreSQL for relational data
- DynamoDB for availability management
- SQLite for local tasks
- Redshift for analysis and reporting
- MongoDB for non-relational data storage

### AWS Services
- **Load Balancer** for load balancing
- **API Gateway** for centralized request handling
- **S3** for backup storage
- **Auto Scaling Group** for scalability

---

## Installation

### Prerequisites
- Docker and Docker Compose installed.
- AWS account configured.

### Clone the Repository
Clone the project from GitHub:
```bash
git clone https://github.com/gabriel9818/appSchool.git
```

### Docker Compose Configuration
Run the following command to start the microservices (fill in configurations as needed):
```bash
docker-compose up -d
```

Example `docker-compose.yml` file:
```yaml
version: '3.8'
services:
  appschool-auth:
    image: appschool/auth-service
    ports:
      - "5000:5000"
    environment:
      - DATABASE_URL=postgresql://username:password@host:port/dbname

  appschool-courses:
    image: appschool/course-service
    ports:
      - "5001:5001"
```

---

## Credits
- Gabriel Ruales
- Gabriela Tumbaco

---

## Contact
Official repository: [GitHub](https://github.com/gabriel9818/appSchool)

