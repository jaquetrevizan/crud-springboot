<h1 align="center" style="font-weight: bold;">API de Produtos - CRUD com Spring Boot</h1>

Este é um projeto de exemplo de uma API RESTful para gerenciar produtos, desenvolvida com Spring Boot 3, Spring Framework 6 e Java 22. A API permite operações de criação, leitura, atualização e exclusão (CRUD) de produtos, utilizando o banco de dados PostgreSQL.

<h2>⚡️Tecnologias e Dependências</h2>

- **Java 22**: Linguagem de programação utilizada no desenvolvimento do projeto.
- **Spring Boot 3**: Framework que facilita a criação de aplicações Java baseadas em Spring.
- **Spring Framework 6**: Oferece suporte adicional ao desenvolvimento com Spring Boot.
- **Spring Web MVC**: Framework utilizado para a construção da API RESTful.
- **Spring Data JPA**: Abstração para facilitar a interação com bancos de dados relacionais usando JPA.
- **Spring Validation**: Utilizado para validação dos dados de entrada.
- **Spring HATEOAS**: Facilita a implementação de princípios RESTful, incluindo hipermídia.
- **PostgreSQL Driver**: Driver JDBC necessário para a conexão com o banco de dados PostgreSQL.
- **PostgreSQL**: Banco de dados relacional utilizado para armazenar os dados da aplicação.

<h2>⚡️ Endpoints da API</h2>

A API fornece os seguintes endpoints para operações CRUD:

- **POST /products**: Cria um novo produto.
- **GET /products**: Retorna uma lista de todos os produtos.
- **GET /products/{id}**: Retorna um produto específico pelo ID.
- **PUT /products/{id}**: Atualiza um produto existente pelo ID.
- **DELETE /products/{id}**: Exclui um produto pelo ID.

<h2>⚡️ Estrutura de Dados </h2>

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
```

<h2>⚡️ Validações e HATEOAS</h2>

O projeto utiliza o Spring Validation para garantir que os dados de entrada estejam corretos antes de serem processados. Também faz uso do Spring HATEOAS para adicionar links aos recursos retornados, seguindo as melhores práticas de design de APIs RESTful.

<h2>✉️ Dúvidas</h2>

Se você tiver alguma dúvida sobre este repositório, envie-a para trevizan.jaqueline@gmail.com.
