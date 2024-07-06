# Aplicação Gerenciador de Cursos

Esta aplicação teve como objetivo exercitar alguns conceitos de microsserviços com Java e Spring Cloud. 

Para isto criamos um microsserviço de gerenciamento de usuários e outro de gerenciamento de cursos que se comunicam utilizando o RabbitMQ. Além disso criamos um servidor de registros para descoberta de serviços e uma API Gateway para mapear as requisições para seus respectivos microsserviços.

## Variáveis de ambiente

Para executar a aplicação primeiramente é necessário declarar as variáveis de ambiente.

Na pasta raiz crie um arquivo .env com as seguintes variáveis de ambiente:

- POSTGRES_USER: Usuário do banco de dados PostgreSQL.
- POSTGRES_PASSWORD: Senha do banco de dados PostgreSQL.
- RABBITMQ_USER: Usuário do RabbitMQ.
- RABBITMQ_PASSWORD: Senha do RabbitMQ.

Na raiz do módulo gerenciador-cursos-eureka-server crie um arquivo .env com as seguintes variáveis:

- EUREKA_SERVER_USER: Usuário padrão do servidor de registros.
- EUREKA_SERVER_PASSWORD: Senha para acessar o servidor de registros.
- EUREKA_SERVER_URL: O endpoint do servidor de registros.

Na raiz do módulo gerenciador-cursos-usuarios-ms crie um arquivo .env com as seguintes variáveis:

- DEV_DB_URL: URL do banco de dados de desenvolvimento.
- TEST_DB_URL: URL do banco de dados de testes.
- POSTGRES_USER: Usuário do banco de dados PostgreSQL.
- POSTGRES_PASSWORD: Senha do banco de dados PostgreSQL.
- EUREKA_SERVER_USER: Usuário padrão do servidor de registros.
- EUREKA_SERVER_PASSWORD: Senha para acessar o servidor de registros.
- EUREKA_SERVER_URL: O endpoint do servidor de registros.
- RABBITMQ_USER: Usuário do RabbitMQ.
- RABBITMQ_PWD: Senha do RabbitMQ.
- RABBITMQ_URL: URL do RabbitMQ.

Na raiz do módulo gerenciador-cursos-cursos-ms crie um arquivo .env com as seguintes variáveis:

- DEV_DB_URL: URL do banco de dados de desenvolvimento.
- TEST_DB_URL: URL do banco de dados de testes.
- POSTGRES_USER: Usuário do banco de dados PostgreSQL.
- POSTGRES_PASSWORD: Senha do banco de dados PostgreSQL.
- EUREKA_SERVER_USER: Usuário padrão do servidor de registros.
- EUREKA_SERVER_PASSWORD: Senha para acessar o servidor de registros.
- EUREKA_SERVER_URL: O endpoint do servidor de registros.
- RABBITMQ_USER: Usuário do RabbitMQ.
- RABBITMQ_PWD: Senha do RabbitMQ.
- RABBITMQ_URL: URL do RabbitMQ.

Na raiz do módulo gerenciador-cursos-api-gateway crie um arquivo .env com as seguintes variáveis:

- EUREKA_SERVER_USER: Usuário padrão do servidor de registros.
- EUREKA_SERVER_PASSWORD: Senha para acessar o servidor de registros.
- EUREKA_SERVER_URL: O endpoint do servidor de registros.

## Tecnologias Utilizadas

- [Java 17](https://www.oracle.com/br/java/technologies/downloads/)
- [Spring Boot 3.2.5](https://spring.io/projects/spring-boot)
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [Spring Web MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)
- [Spring HATEOAS](https://spring.io/projects/spring-hateoas)
- [Spring Security](https://docs.spring.io/spring-security/reference/index.html)
- [Spring Cloud Netflix](https://cloud.spring.io/spring-cloud-netflix/reference/html/)
- [Spring Cloud Gateway](https://spring.io/projects/spring-cloud-gateway)
- [RabbitMQ](https://www.rabbitmq.com/)
- [Lombok](https://projectlombok.org/)
- [MapStruct](https://mapstruct.org/)
- [Validation](https://docs.spring.io/spring-framework/reference/core/validation/beanvalidation.html)
- [Passay](https://www.passay.org/)
- [PostgreSQL](https://www.postgresql.org/)
- [Flyway](https://flywaydb.org/)
- [Springdoc](https://springdoc.org/#google_vignette)
- [Docker](https://www.docker.com/)

