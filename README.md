<h1 align="center"> API de Produtos - CRUD com Spring Boot</h1>
<p align="center">Projeto de exemplo de uma API RESTful para gerenciar produtos, desenvolvida com Spring Boot 3 e Java 22.</p>

---

<p align="center">
  <img src="https://img.shields.io/badge/Java-22-orange?logo=openjdk" alt="Java">
  <img src="https://img.shields.io/badge/Spring_Boot-3-brightgreen?logo=springboot" alt="Spring Boot">
</p>

---

## Objetivo

Este projeto foi desenvolvido com o foco em:

- Demonstrar a criação de uma API RESTful utilizando Spring Boot.
- Implementar operações de **CRUD** (Create, Read, Update, Delete) para gerenciamento de produtos.
- Aplicar boas práticas de validação de dados e uso de **HATEOAS** em APIs REST.

---

## Funcionalidades

- **Criar produtos** (`POST /products`)
- **Listar produtos** (`GET /products`)
- **Buscar produto por ID** (`GET /products/{id}`)
- **Atualizar produto** (`PUT /products/{id}`)
- **Excluir produto** (`DELETE /products/{id}`)

---

## Tecnologias Utilizadas

- [Java 22](https://www.oracle.com/br/java/technologies/downloads/): linguagem utilizada no desenvolvimento do projeto.
- [Spring Boot 3](https://spring.io/projects/spring-boot): framework para construção rápida de aplicações Java.
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa): abstração para persistência de dados.
- [Spring Validation](https://docs.spring.io/spring-framework/reference/core/validation/): validação de dados de entrada.
- [Spring HATEOAS](https://spring.io/projects/spring-hateoas): implementação de hipermídia em APIs REST.
- [PostgreSQL](https://www.postgresql.org/): banco de dados relacional utilizado.
- [Maven](https://maven.apache.org/): gerenciamento de dependências e build.

---

## Estrutura de Dados

```json
{
  "idProduct": "e5e3d4f5-4a25-4d2d-9bef-6d85225c2828",
  "name": "Nome do produto",
  "value": 000.00,
  "_links": {
    "self": {
      "href": "http://localhost:8080/products/e5e3d4f5-4a25-4d2d-9bef-6d85225c2828"
    }
  }
}
````

---

## Instalação e Execução

**Pré-requisitos:**

* [JDK 22](https://www.oracle.com/br/java/technologies/downloads/)
* [Maven](https://maven.apache.org/)
* [PostgreSQL](https://www.postgresql.org/)

**Passos:**

```bash
# Clone o repositório
git clone https://github.com/jaquetrevizan/crud-springboot.git

# Acesse o diretório do projeto
cd crud-springboot

# Configure o banco de dados PostgreSQL no arquivo application.properties
spring.datasource.url= jdbc:postgresql://localhost:5432/products-api
spring.datasource.username= seu-usuario
spring.datasource.password= sua-senha
spring.jpa.hibernate.ddl-auto=update

# Construa o projeto
mvn clean install

# Execute a aplicação
mvn spring-boot:run
```

---

## Dúvidas & Sugestões

* Se tiver alguma ideia para melhorar este projeto ou encontrar algum problema, fique à vontade para abrir uma issue aqui no repositório.
* Para dúvidas mais diretas, você também pode me escrever em: **[trevizan.jaqueline@gmail.com](mailto:trevizan.jaqueline@gmail.com)**.
