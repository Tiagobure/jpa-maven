# Java jpa
## Java Persistence API (JPA) é a especificação padrão da plataforma Java EE (pacote javax.persistence) para mapeamento objeto-relacional e persistência de dados.
JPA é apenas uma especificação (JSR 338):

- http://download.oracle.com/otn-pub/jcp/persistence-2_1-fr-eval-spec/JavaPersistence.pdf

Para trabalhar com JPA é preciso incluir no projeto uma implementação da API (ex: Hibernate).
Arquitetura de uma aplicação que utiliza JPA:
---
![Screenshot 2025-02-21 at 17-38-20 Microsoft Word - nivelamento-JPA-Hibernate docx - nivelamento-JPA-Hibernate pdf](https://github.com/user-attachments/assets/e8944f64-ad13-43a3-97b1-a27292038eef)

## Principais classes:
### EntityManager
https://docs.oracle.com/javaee/7/api/javax/persistence/EntityManager.html

Um objeto EntityManager encapsula uma conexão com a base de dados e serve para efetuar operações de
acesso a dados (inserção, remoção, deleção, atualização) em entidades (clientes, produtos, pedidos, etc.)
por ele monitoradas em um mesmo contexto de persistência.
Escopo: tipicamente mantem-se uma instância única de EntityManager para cada thread do sistema (no caso
de aplicações web, para cada requisição ao sistema).
EntityManagerFactory

https://docs.oracle.com/javaee/7/api/javax/persistence/EntityManagerFactory.html

Um objeto EntityManagerFactory é utilizado para instanciar objetos EntityManager.
Escopo: tipicamente mantem-se uma instância única de EntityManagerFactory para toda aplicação.

# Classe desse projeto de estudo

![Screenshot 2025-02-21 at 17-40-10 Microsoft Word - nivelamento-JPA-Hibernate docx - nivelamento-JPA-Hibernate pdf](https://github.com/user-attachments/assets/5a9ebf6a-d054-493d-a8ae-e5f5b32c3e27)
