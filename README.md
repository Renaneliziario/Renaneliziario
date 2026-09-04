# Renan Queiroz Eliziario

**Desenvolvedor Back-End Java** | Spring Boot · Microsserviços · REST API · Docker

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/renaneliziario/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white)](mailto:renanqueiroz92@gmail.com)
![Aberto a oportunidades](https://img.shields.io/badge/Aberto%20a%20oportunidades-✔-brightgreen?style=flat)

---

Graduado em **Análise e Desenvolvimento de Sistemas** (Impacta, 2024) com curso profissionalizante em **Back-End Java** concluído (EBAC, 08/2026).

Portfólio construído com progressão técnica deliberada: dos fundamentos de OOP e persistência com JDBC até ecossistemas de microsserviços com Spring Cloud, Docker Compose e bancos de dados isolados por serviço, incluindo um front-end em React consumindo essas APIs. Foco em código testável, APIs documentadas e ambientes reproduzíveis.

---

## 🛠️ Tech Stack

![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat&logo=springboot&logoColor=white)
![Spring Cloud](https://img.shields.io/badge/Spring_Cloud-6DB33F?style=flat&logo=spring&logoColor=white)
![React](https://img.shields.io/badge/React_19-61DAFB?style=flat&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white)
![JUnit5](https://img.shields.io/badge/JUnit_5-25A162?style=flat&logo=junit5&logoColor=white)
![Mockito](https://img.shields.io/badge/Mockito-25A162?style=flat&logoColor=white)
![Swagger](https://img.shields.io/badge/Swagger-85EA2D?style=flat&logo=swagger&logoColor=black)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat&logo=apachemaven&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)

**Linguagens:** Java 8/11/17, SQL, Python, TypeScript
**Frameworks:** Spring Boot 3, Spring Cloud Config, OpenFeign, Flyway, React, Node.js, JPA/Hibernate, Spring Data JPA, JUnit 4/5, Mockito, Lombok
**Arquitetura:** Estruturas de Dados, Microsserviços, REST API, MVC, Generic DAO, SOLID, Clean Code, Design Patterns, Injeção de Dependência
**Bancos:** PostgreSQL, MySQL, MongoDB, H2
**DevOps:** Docker, Docker Compose, Maven, Git, GitHub, Swagger/OpenAPI, Actuator/Prometheus, Linux
**Noções (ainda sem prática consolidada):** Terraform, AWS, RabbitMQ, Angular

---

## 🚀 Projetos em Destaque

### 🦺 [epi-warehouse-microservices](https://github.com/Renaneliziario/epi-warehouse-microservices)
**Almoxarifado Industrial de EPI — Spring Boot 3.3 · Spring Cloud · PostgreSQL + H2 · Docker Compose**

O projeto mais completo do portfólio. 5 microsserviços de domínio (identidade, categoria, catálogo/retirada de estoque, gestão de segurança industrial) com [frontend próprio em React](https://github.com/Renaneliziario/epi-warehouse-frontend) consumindo as APIs reais.

- Validação cross-service síncrona via `RestClient` (padrão `/exists`, 204/404), sem duplicar dado entre serviços
- `servico-operacao` com PostgreSQL + Flyway, schema versionado e seed real de domínio; os demais em H2
- Frontend React + TypeScript integrado end-to-end nos 4 domínios, com testes (Vitest + React Testing Library)
- Métricas expostas via Actuator/Prometheus; Docker Compose orquestrando os 5 serviços + Postgres
- **CI (GitHub Actions) nos dois repositórios**: backend roda `mvn clean install` a cada push/PR; frontend roda typecheck, lint, testes e build

---

### ☁️ [Sales-Microservices](https://github.com/Renaneliziario/Sales-Microservices)
**Ecossistema de Microsserviços de E-Commerce — Spring Boot 3.4 · Spring Cloud · Docker Compose**

Arquitetura distribuída com 4 serviços independentes (Config Server, Cliente, Produto, Vendas), cada um com banco de dados PostgreSQL isolado.

- Spring Cloud Config Server centralizando configurações dos 3 serviços dependentes
- Integração entre serviços via Feign Client, com saga manual de compensação no fluxo de venda
- Fluxo completo de venda com baixa automática de estoque e validação de disponibilidade
- APIs REST documentadas via Swagger/OpenAPI; ambiente orquestrado com Docker Compose

---

### 🏆 [desafio-programador-duxus](https://github.com/Renaneliziario/desafio-programador-duxus)
**Desafio Técnico Real — Spring Boot 3.2 · Thymeleaf · JUnit 5 · Docker**

Aplicação web full-stack desenvolvida como desafio técnico. Demonstra capacidade de entrega em contexto real com cobertura de testes completa.

- Interface web com Thymeleaf + REST API documentada via Swagger no mesmo projeto
- 3 entidades relacionais (Integrante, Time, Composição) com mapeamento JPA e controle transacional
- Java Records como DTOs para imutabilidade na camada de API
- Suíte de testes com JUnit 5 parametrizado e MockMvc; perfil H2 permite execução sem Docker

---

### 🏛️ [SalesPersistence-JPA](https://github.com/Renaneliziario/SalesPersistence-JPA)
**Arquitetura em Camadas · Generic DAO · JPA/Hibernate · H2**

- Padrão Generic DAO com Java Generics centralizando operações de persistência
- Criteria API com JOIN FETCH evitando N+1, mapeamentos ORM avançados (`@OneToMany`, `@ManyToOne`)
- Persistence Units separados (PostgreSQL em produção, H2 em teste)

---

### 🛡️ [QualityGuard-UnitTests](https://github.com/Renaneliziario/QualityGuard-UnitTests)
**Engenharia de Qualidade · JUnit 4/5 · Mockito · Reflection API**

- Suíte completa com testes unitários e de integração
- Mockito para isolamento de camadas e anotações personalizadas via Reflection API

---

### 🛢️ [SalesSystem-JDBC](https://github.com/Renaneliziario/SalesSystem-JDBC)
**Persistência Nativa · JDBC · PostgreSQL · Controle Transacional**

- Integração direta com PostgreSQL via JDBC puro e gerenciamento manual de transações
- Proteção contra SQL Injection com PreparedStatement em todas as operações

---

## 📫 Contato

- **LinkedIn:** [linkedin.com/in/renaneliziario](https://www.linkedin.com/in/renaneliziario/)
- **Email:** renanqueiroz92@gmail.com
- **Localização:** São Paulo, SP — Brasil

> *"Cada projeto é uma decisão técnica consciente — não apenas código que funciona, mas código que comunica."*
