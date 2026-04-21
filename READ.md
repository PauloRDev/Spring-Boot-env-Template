# spring-boot-env-template

Basic configuration template for environment variables in Spring Boot projects.

---

## .env

> ⚠️ **Never upload the `.env` file to GitHub!** Add it to your `.gitignore` file.`.

```env
# DATABASE
DB_URL=jdbc:h2:mem:testdb
DB_USERNAME=your_username
DB_PASSWORD=your_password

# API Keys
API_KEY=your_api_key
API_SECRET=your_secret_here

# Environment
APP_ENV=development
APP_PORT=8080
```

---

## .gitignore

```gitignore
.env
```

---

## application.properties

```properties
spring.application.name=AppName

# Database
spring.datasource.url=${DB_URL}
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}

# API Keys
api.key=${API_KEY}
api.secret=${API_SECRET}

# Environment
server.port=${APP_PORT}
```

---
