# Email Microservice
## About the project
This project consists of a backend asynchronous microservice for sending emails for multiple purposes, from email notifications, user account confirmation, etc.
## Application
### Stack
- Java 17
### Technologies
- Spring Boot
- JavaMail
- JPA / Hibernate
- Maven
- RabbitMQ
### Database
- PostgreSQL ([ElephantSQL](https://www.elephantsql.com/))
### Features
- 
## How to run this project

```bash
# clone repository
git clone https://github.com/pauloerico/ms-email
```
Add the credentials for the [Google SMTP server](https://support.google.com/accounts/answer/185833), [RabbitMQ](https://www.cloudamqp.com/) service and [ElephantSQL](https://www.elephantsql.com/) databaseon the application.properties file and you are ready to go!

## Reference
- Based on [Michelli Brito's project](https://github.com/MichelliBrito/ms-email) and video tutorials:
  - [CRIANDO UM MICROSERVICE DE ENVIO DE EMAIL](https://www.youtube.com/watch?v=ZBleZzJf6ro&t=1671s)
  - [MENSAGERIA COM RABBITMQ NO MICROSERVICE DE EMAIL](https://www.youtube.com/watch?v=V-PqR0BxA8c&t=267s)
