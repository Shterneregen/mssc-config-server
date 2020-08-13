# SFG Brewery Configuration Service

| Service                                                                                    | Port   |
| ------------------------------------------------------------------------------------------ |--------|
| [MSSC Beer Service](https://github.com/Shterneregen/mssc-beer-service)                     | 8080   |
| [MSSC Beer Order Service](https://github.com/Shterneregen/mssc-beer-order-service)         | 8081   |
| [MSSC Beer Inventory Service](https://github.com/Shterneregen/mssc-beer-inventory-service) | 8082   |
| [SFG Inventory Failover Service](https://github.com/Shterneregen/mssc-inventory-failover)  | 8083   |
| [SFG Brewery Gateway Service](https://github.com/Shterneregen/mssc-brewery-gateway)        | 9090   |
| [SFG Brewery Eureka Service](https://github.com/Shterneregen/mssc-brewery-eureka)          | 8761   |
| [SFG Brewery Configuration Service](https://github.com/Shterneregen/mssc-config-server)    | 8888   |
| [SFG Brewery Configuration Repo](https://github.com/Shterneregen/mssc-brewery-config-repo) | GitHub |

---
To use commands below, property *encrypt.key* should be set in [bootstrap.properties](./src/main/resources/bootstrap.properties).  
This allows to store credentials encrypted in [SFG Brewery Configuration Repo](https://github.com/Shterneregen/mssc-brewery-config-repo).
```
curl -d "password" -X POST http://localhost:8888/encrypt
```
```
curl -d "a490da079322ab133e891f496e8f65b2fea664f029c5962bd8e5bf9f6dbac7b5" -X POST http://localhost:8888/decrypt
```

---
* Original repo:
[SFG Brewery Configuration Service](https://github.com/springframeworkguru/mssc-config-server)
* Course: 
[Spring Boot Microservices with Spring Cloud Beginner to Guru](https://www.udemy.com/course/spring-boot-microservices-with-spring-cloud-beginner-to-guru/)