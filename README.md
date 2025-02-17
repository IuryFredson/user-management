# User Management System

Este é um sistema de gerenciamento de usuários desenvolvido com Spring Boot (backend) e React (frontend). O sistema permite a criação, leitura, atualização e exclusão (CRUD) de usuários em um banco de dados PostgreSQL.

## Tecnologias Utilizadas

- **Backend**: Spring Boot, Java, PostgreSQL
- **Frontend**: React, Tailwind CSS
- **Ferramentas**: Maven, Git, PostgreSQL

## Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- [Java JDK 17 ou superior](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Maven](https://maven.apache.org/download.cgi)
- [Node.js](https://nodejs.org/) (para o frontend)
- [PostgreSQL](https://www.postgresql.org/download/)

## Configuração do Banco de Dados

1. Crie um banco de dados no PostgreSQL com o nome `usermanagement` (ou outro nome de sua preferência).
2. Execute o script SQL localizado em `src/main/java/com/usermanagement/database/schema.sql` para criar a tabela `users`.

## Configuração do Projeto

1. Clone o repositório:

   ```bash
   git clone https://github.com/IuryFredson/user-management.git
   ```

2. Navegue até o diretório do projeto:

```bash
cd user-management/backend
```
3. Configure o arquivo application.properties com as credenciais do seu banco de dados:

```bash
spring.datasource.url=jdbc:postgresql://localhost:5432/your_database_name
spring.datasource.username=your_username
spring.datasource.password=your_password
```

4. Compile e execute o projeto Spring Boot:

```bash
mvn clean install
mvn spring-boot:run
```
O backend estará disponível em http://localhost:8080

5. Para o frontend, navegue até o diretório frontend e instale as dependências:

```bash
cd ../frontend
npm install
```
6. Execute o frontend:

```bash
npm run dev
```
O frontend estará disponível em http://localhost:5173.


## **Endpoints da API**
- **GET**/api/v1/users/{id} - Retorna um usuário específico pelo ID.

- **POST** /api/v1/users - Cria um novo usuário.

- **PUT** /api/v1/users/{id} - Atualiza um usuário existente.

- **DELETE** /api/v1/users/{id} - Exclui um usuário.


## **Estrutura do Projeto**
**Backend**: Spring Boot com controllers, services e repositórios.

**Frontend**: React com componentes para listar, criar, editar e excluir usuários.


## **Contribuição**
Se você deseja contribuir para este projeto, siga os passos abaixo:

Faça um **fork** do repositório.

Crie uma branch para sua feature (git checkout -b feature/nova-feature).

Commit suas mudanças (git commit -m 'Adicionando nova feature').

Push para a branch (git push origin feature/nova-feature).

Abra um **Pull Request**.



