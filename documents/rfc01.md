# RFC #1: Estrutura de Pastas para o Projeto CustomerAPI

## Tema:

Definição da estrutura de pastas da CustomerAPI baseada nas práticas mais utilizadas pela comunidade Golang, seguindo conceitos de Arquitetura Hexagonal.

## Motivação:

A organização do código-fonte é fundamental para garantir a manutenibilidade e escalabilidade de um projeto, especialmente ao seguir boas práticas como Arquitetura Hexagonal e Domain-Driven Design (DDD). Em Golang, embora a linguagem ofereça liberdade na definição de estrutura de pastas, algumas abordagens têm se consolidado na comunidade como práticas recomendadas.

O objetivo desta RFC é justificar a escolha de uma estrutura de pastas que facilita o crescimento do projeto, a separação de responsabilidades e o desacoplamento entre as camadas de domínio e infraestrutura.

### Proposta

Após uma análise das práticas mais comuns na comunidade Golang, decidimos adotar a seguinte estrutura de pastas para o projeto CustomerAPI:

#### Estrutura

```
/customer-api
  /cmd
    /api
      main.go         # Ponto de entrada da aplicação
  /internal
    /domain
      /customer
        customer.go   # Entidade Customer
    /app
      /usecases
        customer_service.go  # Casos de uso (CRUD de clientes)
    /interfaces
      /http
        customer_handler.go  # Adaptador HTTP
  /pkg
    - common utilities
```