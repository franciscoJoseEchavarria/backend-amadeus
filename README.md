# Reto Amadeus Backend
Este proyecto es una aplicación backend desarrollada con Spring Boot que proporciona varios endpoints para gestionar usuarios y consultas de usuarios.

## Requisitos

- Java 17
- Gradle
- PostgreSQL

## Configuración de la Base de Datos

Para configurar la conexión a la base de datos, sigue estos pasos:

1. Crea una base de datos en PostgreSQL.
2. Configura las credenciales de la base de datos en el archivo `application.properties`.

### application.properties

```
properties
spring.application.name=reto3-back-amadeus

# Configuración de la base de datos
# URL de la base de datos PostgreSQL
spring.datasource.url=jdbc:postgresql://127.0.0.1:5432/reto-back-3
# Nombre de usuario para la base de datos
spring.datasource.username=postgres
# Contraseña para la base de datos
spring.datasource.password=nueva123

# Configuración de Hibernate
# Dialecto de Hibernate para PostgreSQL
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect
# Muestra las consultas SQL en la consola
spring.jpa.show-sql=true
# Configuración de Hibernate para crear y eliminar las tablas en cada inicio
spring.jpa.hibernate.ddl-auto=create-drop

# Configuración del servidor
# Puerto en el que la aplicación se ejecutará
server.port=8081
```