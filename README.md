# Order Service
## Project structure
- [API Gateway](https://github.com/mibrgmv/order-service-gateway/)
- [Order Creation Service](https://github.com/mibrgmv/order-creation-service/)
- [Order Processing Service](https://github.com/mibrgmv/order-processing-service/)
### gRPC Gateway
A gateway that exposes an API and handles user requests to services via gRPC.
### Order Creation Service
A service that is responsible for order creation and completion. It communicates implicitly with the gateway via gRPC and asynchronous with **Order Processing Service** via 2 Kafka topics.
## Order Processing Service
Handles order processing logic. Communicates alike **Order Creation Service**.
## Docker support
Here is a docker compose to get up Kafka, Order processing service and its Postgres database. 
```yml

```
