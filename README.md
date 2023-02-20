# Email Microservice
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
- The project has an endpoint for sending email messages from POST requests. This is a synchronous endpoint.
- For sending asynchrnous messages, it is connected to a AMPQ messaging service, that queues messages for sending when the service is available.
### How to run this project
```bash
# clone repository
git clone https://github.com/pauloerico/ms-email
```
Add the credentials for the [Google SMTP server](https://support.google.com/accounts/answer/185833), [RabbitMQ](https://www.cloudamqp.com/) service and [ElephantSQL](https://www.elephantsql.com/) databaseon the application.properties file and you are ready to go!
#### Endpoint
- Send email
```http request
POST http://localhost:8080/sending-email
```
#### DTO
```json
{
    "ownerRef": "referência",
    "emailFrom": "sender@email.com",
    "emailTo": "recipient@email.com",
    "subject": "Email subject",
    "text": "Email message here."
}
```
## References
Based on [Michelli Brito's project](https://github.com/MichelliBrito/ms-email) and video tutorials:
- [CRIANDO UM MICROSERVICE DE ENVIO DE EMAIL](https://www.youtube.com/watch?v=ZBleZzJf6ro&t=1671s)
- [MENSAGERIA COM RABBITMQ NO MICROSERVICE DE EMAIL](https://www.youtube.com/watch?v=V-PqR0BxA8c&t=267s)

Other references:
- https://mailtrap.io/blog/sending-email-using-java/
- https://www.javatpoint.com/example-of-sending-email-using-java-mail-api-through-gmail-server


Alternative SMTP servers:
- [mailtrap](https://mailtrap.io/)
- [mailjet](https://www.mailjet.com/)
