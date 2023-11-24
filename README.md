# Angular-Spring Boot Ecommerce

**Note:** This project focuses on Spring Security implementation and Stripe integration and does not include a focus on the UI.

## Getting Started

### Prerequisites

- Java 17
- Maven
- Angular
- MS SQL Server Database
- Stripe Secret Key

**1. Clone the repository:**
```shell
git clone https://github.com/the0ss/angular-springboot-ecommerce.git
```

### Angular Frontend
**1. Navigate to the `frontend` directory:**
```shell
cd frontend
```

2. Install dependencies
```shell
npm install
```

### Spring Boot Backend

**1. Navigate to the `backend` directory:**
```shell
cd backend
```

**2. Build the app:**
```shell
mvn clean install
```

## MS SQL Server Database / Stripe
**1. Modify `application.yml`:**
```shell
spring:
  datasource:
    driver-class-name: com.mysql.cj.jdbc.Driver
    url: jdbc:mysql://localhost:3306/ecom-app
    username: springstudent
    password: springstudent
  jpa:
    hibernate:
      ddl-auto: update
stripe:
  secret-key: sk_test_51NiZKsLtTFoBOb8wTg4V2C3bJqrQ53qMHLusPXct6hp0O3yNtHXfEITKl7bLHNPRG7Egk28A5d1X7H4yoCvUl5kF00OP3VpgCr
```

### Important

For to use this app
  - First create USER and ADMIN role in database then, You can do the REST calls other wise Error.
  - We can use any database H2 or MySQL . Your choice. But MySQL is preferred as we can see the logs.
  - *Main component is backend, UI is just implemented to be used on frontend.*
