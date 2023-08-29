# Santander Dev Week 2023

Java RESTful API criada para a Santander Dev Week.

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