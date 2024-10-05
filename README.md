# Customer API

**CustomerAPI** é um projeto desenvolvido em **Golang** com o propósito de estudar e aplicar boas práticas de Arquitetura Hexagonal e Domain-Driven Design (DDD). O foco é criar uma API de gerenciamento de clientes, desde operações básicas de **CRUD** até funcionalidades mais avançadas. A API serve como uma plataforma de aprendizado, explorando os princípios e conceitos do Golang, enquanto segue uma abordagem limpa e escalável.

### Objetivo

* **Aprender Golang:** Estudar e aplicar a linguagem em um projeto real.
* **Arquitetura Hexagonal:** Garantir que a lógica de negócios (domínio) seja desacoplada da infraestrutura.
* **DDD (Domain-Driven Design):** Foco na modelagem do domínio e na clareza do código.
* **Boas práticas:** Seguir princípios de Clean Code, SOLID e desenvolvimento orientado a testes (TDD).

### Funcionalidades

#### 1. Geriamento de Clientes

* Criar, listar, atualizar e excluir clientes.
* Foco na modelagem do domínio de clientes.

#### 2. Estudo de Golang

* Implementação das funcionalidades usando recursos idiomáticos do Go, como goroutines, interfaces e tratamento de erros.

#### 3. Documentação e RFCs:

* Cada decisão técnica será documentada por meio de RFCs (Request for Comments) para promover transparência e boas práticas de desenvolvimento.

### Estrutura do Projeto

O projeto segue a Arquitetura Hexagonal, organizando o código em torno de camadas bem definidas:

* **Domínio:** Contém as entidades e regras de negócios.
* **Casos de Uso:** Orquestra as interações entre o domínio e a infraestrutura.
* **Adaptadores:** Ponto de integração com interfaces externas (HTTP, banco de dados, etc.).