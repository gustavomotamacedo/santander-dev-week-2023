# santander-dev-week-2023
Java RESTful API para a santanter-dev-week-2023

## Diagrama de classes

```mermaid
classDiagram
  class User {
    -name: String
    -account: Account
    -features: Feature[]
    -card: Card
    -news: News[]
  }
  class Account {
    -number: String
    -agency: String
    -balance: Float
    -limit: Float
  }
  class Feature {
    -icon: String
    -description: String
  }
  class Card {
    -number: String
    -limit: Int
  }
  class News {
    -icon: String
    -description: String
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
```
