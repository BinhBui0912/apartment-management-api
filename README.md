#  Apartment Management System

A RESTful API for managing apartment complexes, built with **Spring Boot 3** and **Java 21**.

## 🛠 Technology Stack
- **Java 21** + **Spring Boot 3.5.4**
- **Spring Security** + **JWT Authentication**
- **Spring Data JPA** + **MySQL 8.0**
- **Docker** + **Docker Compose**
- **Spock Framework** for testing

##  Quick Start with Docker

### Prerequisites
- Docker and Docker Compose installed

### Run the Application
1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd apartment-manager
   ```

2. **Start all services**
   ```bash
   docker-compose up -d
   ```

3. **Access the application**
   - API: `http://localhost:8080`
   - Swagger UI: `http://localhost:8080/swagger-ui.html`

### Docker Services
- **MySQL Database**: Port 3306
- **Spring Boot App**: Port 8080

### Useful Docker Commands
```bash
# View logs
docker-compose logs -f app

# Stop all services
docker-compose down

# Rebuild and restart
docker-compose up --build

# Check running containers
docker-compose ps
```


##  Key Features
- **Apartment Management**: CRUD operations with pagination
- **Resident Management**: Demographics and apartment association
- **Monthly Bill Management**: Billing and payment tracking
- **JWT Authentication**: Role-based access control (ADMIN/USER)
- **Email Integration**: Notifications via SMTP
- **API Documentation**: Swagger UI and OpenAPI specs

##  API Endpoints

### Authentication
```http
POST /api/v1/auth/login          # User login
POST /api/v1/auth/register       # User registration
```

### Main Resources
```http
GET    /api/v1/apartments        # Get apartments (paginated)
POST   /api/v1/apartments        # Create apartment
GET    /api/v1/residents         # Get residents (paginated)
POST   /api/v1/residents         # Create resident
GET    /api/v1/monthly-bills     # Get bills (paginated)
POST   /api/v1/monthly-bills     # Create bill
```

##  Project Structure
- **Controllers**: REST API endpoints
- **Services**: Business logic layer
- **Repositories**: Data access layer
- **DTOs**: Request/Response objects
- **Security**: JWT + Role-based auth
- **Testing**: Spock + JUnit integration

---

**Contact**: duybinhh03@gmail.com
