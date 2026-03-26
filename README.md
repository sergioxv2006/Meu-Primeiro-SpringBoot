# 🌱 Meu Primeiro Spring Boot
Projeto desenvolvido durante o estudo do framework Spring Boot com Java, baseado na vídeo aula de 2 horas do canal Matheus Leandro Ferreira no YouTube.

## 📋 Sobre o Projeto
Uma API REST completa com autenticação JWT, gerenciamento de usuários e produtos, integrada ao banco de dados PostgreSQL.

## 🚀 Tecnologias Utilizadas

- Java — linguagem principal do projeto
- Spring Boot — framework principal, iniciado via Spring Initializer
- Spring Security — autenticação e autorização
- JWT (JSON Web Token) — controle de acesso via token
- PostgreSQL — banco de dados relacional
- JPA / Hibernate — mapeamento objeto-relacional
- Maven (pom.xml) — gerenciamento de dependências
- Postman — testes de requisições HTTP

## 🗂️ Estrutura do Projeto
```
src/main/java/com/example/meu_primeiro_springboot/
├── controller/       # Controladores REST (AuthController, ProdutoController, HelloController)
├── exceptions/       # Tratamento global de exceções
├── model/            # Entidades (Usuario, Produto)
├── repository/       # Interfaces de acesso ao banco de dados
├── security/         # Configurações de segurança, JWT e filtros
└── service/          # Regras de negócio
```

## ⚙️ Funcionalidades

- ✅ Cadastro de usuários com senha criptografada (BCrypt)
- ✅ Login com geração de token JWT
- ✅ Autenticação via Bearer Token
- ✅ CRUD de produtos protegido por autenticação
- ✅ Tratamento de exceções personalizado
- ✅ Integração com PostgreSQL

## 🔧 Como Executar

1. Clone o repositório
2. Configure o **application.properties** com suas credenciais do PostgreSQL
3. Execute o projeto via IntelliJ IDEA ou com **./mvnw spring-boot:run**
4. Acesse (http://localhost:8080)

## 📡 Endpoints Principais
| Método | Rota                 | Descrição                     |
|--------|----------------------|-------------------------------|
| POST   | `/auth/register`     | Cadastrar novo usuário        | 
| POST   | `/auth/login`        | Autenticar e obter token      | 
| GET    | `/api/produtos/{id}` | Buscar produto (autenticado)  |

## 📚 Referência
Vídeo aula: **Matheus Leandro Ferreira** — YouTube
