# Santander Dev Week 2023

Java RESTful API criada para a Santander Dev Week.

## Tecnologias Utilizadas
- **Java 17**;
- **Spring Boot 3**
- **Spring Data JPA**
- **OpenAPI (Swagger)**
- **Railway**

### Diagrama de Classes

```mermaid
classDiagram
  class User {
    - name: String
    - account: Account
    - features: Feature[]
    - card: Card
    - news: News[]
  }

  class Account {
    - number: String
    - agency: String
    - balance: String
    - limit: String
  }

  class Feature {
    - icon: String
    - description: String
  }

  class Card {
    - number: String
    - limit: String
  }

  class News {
    - icon: String
    - description: String
  }

  User -- Account : has
  User -- Feature : has multiple
  User -- Card : has
  User -- News : has multiple
```
### Deploy

O deploy desta API foi realizado com [Railway](railway.app/) e pode ser encontrado no seguinte domínio: (https://sdw-2023-jessicakisner-production.up.railway.app/)

### A API no Swagger

A documentação da API pode ser vista e editada no Swagger no seguinte domínio: (https://sdw-2023-jessicakisner-production.up.railway.app/swagger-ui/index.html)

### Referência

Esta API foi criada como parte do projeto do Santander Bootcamp 2023 - Backend Java, disponibilizado pela [Dio](https://web.dio.me)