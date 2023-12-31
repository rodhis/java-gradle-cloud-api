# Java Gradle API

Java API padrão Rest com deploy em serviço de nuvem.

Parte do bootcamp Backend Java feito pela Dio/Santander.

---------------

### Link da API publicada: [Clique Aqui](https://rodhis-java-api.up.railway.app/swagger-ui/index.html)

Obs: Esta API ficará publicada por tempo limitado, enquanto for usada como portfólio pessoal.

-----------------------

### Tecnologias utilizadas:

- Spring boot 3
- Spring initializer
- Gradle
- OpenAPI Documentation (antigo Swagger)
- JPA
- H2 database
- Railway com PostgreSQL

-----------------
### Abstração no Figma: [Link](https://www.figma.com/file/tlqteif6Y4BIpxypnP64qx/DIO%2FSantander-Bank-API-project?type=design&node-id=2%3A92&mode=design&t=PtF9ZvLtrzGFbhNF-1)

---------------------

### Diagrama de Classes (com Mermaid):

```mermaid

classDiagram
class User {
-String name
-Account account
-Feature[] features
-Card card
-News[] news
}

class Account {
-String number
-String agency
-Number balance
-Number limit
}

class Feature {
-String icon
-String description
}

class Card {
-String number
-Number limit
}

class News {
-String icon
-String description
}

User "1" *-- "1" Account
User "1" *-- "N" Feature
User "1" *-- "1" Card
User "1" *-- "N" News
```
