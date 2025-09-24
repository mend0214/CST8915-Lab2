# CST8915-Lab2

## Demo Video Link

## Reflection Questions

1. **What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?**

I added a .env file and used environment variables such as: 
* RABBITMQ_CONNECTION_STRING=amqp://newuser:newpassword@20.116.219.116:5672/
* PORT=3000
* PORT=3030

To configure the ports used by order service and product service, and to access RabbitMQ server.

2. **Why is it important to use environment variables instead of hard-coding configurations in your application?**

It is important to use environment variables instead of hard-coding configuration because it allows multiple deployments of the codebase in different environments without altering the codebase.

3. **Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?**

It is important to have separate repositories for each microservice because it helps maintain indpendence by allowing microservices use different technologies and dependencies and not limiting the whole codebase. It also helps in scalability by allowing developers to update and deploy each microservice individually without have to scale the entire codebase.

## Services GitHub Repo

1. order service : https://github.com/mend0214/order-service-lab2/tree/main/order-service
2. product service : https://github.com/mend0214/product-service-lab2/tree/main/product-service
3. store front : https://github.com/mend0214/store-front-lab2/tree/main/store-front