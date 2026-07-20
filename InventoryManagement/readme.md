# Inventory Management System

Sistema web de gerenciamento de estoque desenvolvido com **ASP.NET Core MVC** e **Entity Framework Core**, permitindo o cadastro, edição, consulta e remoção de produtos por meio de uma interface simples e organizada.

---

# Sobre o Projeto

O **Inventory Management System** foi desenvolvido para facilitar o gerenciamento de produtos em estoque utilizando o padrão arquitetural **MVC (Model-View-Controller)**.

A aplicação realiza operações de CRUD (Create, Read, Update e Delete), armazenando os dados em um banco SQL Server através do Entity Framework Core.

---

# Funcionalidades

- Cadastro de produtos
- Listagem de produtos
- Edição de produtos
- Exclusão de produtos
- Validação de formulários
- Controle de estoque
- Interface baseada em ASP.NET MVC

---

# Tecnologias Utilizadas

- ASP.NET Core MVC
- C#
- Entity Framework Core
- SQL Server
- HTML5
- CSS3
- Bootstrap
- Razor Pages

---

# Arquitetura

O projeto segue o padrão **MVC**, separando as responsabilidades da aplicação:

### Model
Responsável pela representação dos dados e pelas validações.

Exemplo:

- Product

### View

Responsável pela interface com o usuário.

Exemplos:

- Index
- Create
- Edit
- Delete

### Controller

Responsável por receber as requisições e realizar a comunicação entre View e Model.

Exemplo:

- ProductsController

---

# Banco de Dados

O projeto utiliza:

- SQL Server
- Entity Framework Core
- DbContext para gerenciamento das entidades

A conexão é realizada através da string de conexão configurada no arquivo:

```
appsettings.json
```

---

# Estrutura do Projeto

```
InventoryManagement
│
├── Controllers
│   └── ProductsController.cs
│
├── Data
│   └── AppDbContext.cs
│
├── Models
│   └── Product.cs
│
├── Views
│   └── Products
│       ├── Index
│       ├── Create
│       ├── Edit
│       └── Delete
│
├── wwwroot
│
├── Program.cs
│
└── appsettings.json
```

---

# Como Executar

## 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/inventory-management-system.git
```

## 2. Entre na pasta

```bash
cd inventory-management-system
```

## 3. Configure o banco

Edite o arquivo:

```
appsettings.json
```

Adicione sua Connection String do SQL Server.

---

## 4. Execute as migrations (caso existam)

```bash
dotnet ef database update
```

---

## 5. Execute o projeto

```bash
dotnet run
```

ou abra a solução:

```
InventoryManagement.sln
```

no Visual Studio e pressione **F5**.

---

# Autor

**Gabriel Afonso dos Santos**

- GitHub: https://github.com/gabrielafonsods
- LinkedIn: https://www.linkedin.com/in/gabriel-afonso-0a273b271/
