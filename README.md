# Lab 2: CST8915 Full-stack Cloud-native Development

## Youtube video:
[https://youtu.be/BMyPxqBRqto](https://youtu.be/BMyPxqBRqto)

## Microservices repos:
- [Store front](https://github.com/bout0167/lab2-store-front.git)
- [Product service](https://github.com/bout0167/lab2-product-service.git)
- [Order service](https://github.com/bout0167/lab2-order-service.git)

## 1. What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?
I changed both services to use environment variables for their configuration. The order-service uses environment variables for the RabbitMQ connection and port. The product-service uses an environment variable for its port. RabbitMQ is used as a backing service for the order-service.

## 2. Why is it important to use environment variables instead of hard-coding configurations in your application?
Environment variables make it easier to use the application in different environments. We can change the settings without changing the code. They also help keep sensitive information, such as passwords, out of the code.

## 3. Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?
Each service has its own repository, so it can be developed, tested, and updated separately. This makes the project easier to manage and allows each service to be scaled independently.