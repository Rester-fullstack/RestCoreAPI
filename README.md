RestCoreAPI

API RESTful desenvolvida em C# com ASP.NET Core, utilizando Entity Framework Core e SQL Server, para gerenciamento de Produtos e Usuários.
Inclui endpoints completos de CRUD e documentação automática via Swagger.

🚀 Funcionalidades da API

A API permite realizar operações de CRUD:

📦 Produtos

GET – Listar produtos

GET /{id} – Buscar produto por ID

POST – Cadastrar produto

PUT /{id} – Atualizar produto

DELETE /{id} – Remover produto

👤 Usuários

GET – Listar usuários

GET /{id} – Buscar usuário por ID

POST – Criar usuário

PUT /{id} – Atualizar usuário

DELETE /{id} – Remover usuário

🛠️ Tecnologias Utilizadas

ASP.NET Core 8

Entity Framework Core

SQL Server (LocalDB ou instância própria)

Swagger / Swashbuckle (documentação da API)

LINQ

.NET 8

📁 Estrutura do Projeto
RestCoreAPI/
│
├── Controllers/
├── Data/
├── Migrations/
├── Models/
├── Properties/
├── RestCoreAPI.http
│
├── Program.cs
├── appsettings.json
├── RestCoreAPI.csproj
└── README.md

⚙️ Como Rodar o Projeto
1. Clone o repositório
git clone https://github.com/Rester-fullstack/RestCoreAPI.git

2. Configure a string de conexão

No arquivo appsettings.json:

"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=RestCoreAPIDB;Trusted_Connection=True;"
}


Ajuste para sua instância do SQL Server se necessário.

3. Execute as migrations para criar o banco
dotnet ef database update

4. Execute a API
dotnet run

5. Abra o Swagger

Acesse no navegador:

https://localhost:<porta>/swagger


Aqui você pode testar todos os endpoints.

📡 Endpoints Principais
/produtos
Método	Descrição
GET	Lista todos os produtos
GET /{id}	Consulta produto por ID
POST	Cadastra novo produto
PUT /{id}	Atualiza produto
DELETE /{id}	Remove produto
/usuarios
Método	Descrição
GET	Lista usuários
GET /{id}	Consulta usuário por ID
POST	Cadastra novo usuário
PUT /{id}	Atualiza usuário
DELETE /{id}	Remove usuário

👩‍💻 Autora

Ester da Costa Batista
📧 ester.retse30@gmail.com
