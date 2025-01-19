Aqui está o README.md atualizado com a informação sobre o uso de token de segurança:

```markdown
# 🛒 CarrinhoComprasAPI  

Uma API minimalista desenvolvida em **C#** com **.NET**, criada com o objetivo de **aprender e praticar** conceitos básicos e boas práticas de desenvolvimento backend.  

Este projeto foi realizado **para fins de estudo**, sendo um exemplo simples e funcional para explorar as capacidades do .NET e APIs minimalistas.  

---

## 🌟 Funcionalidades  

✔️ Adicionar produtos ao carrinho.  
✔️ Listar os produtos no carrinho.  
✔️ Atualizar a quantidade de produtos.  
✔️ Remover produtos do carrinho.  
✔️ **Segurança**: Token de segurança para proteger as requisições da API.

---

## 🚀 Tecnologias Utilizadas  

- 🖥️ **C#**  
- 🌐 **.NET Minimal API**  
- 📦 **Entity Framework Core** (se necessário)  
- 🐳 **Docker** (para o banco de dados)  
- 🔑 **Token de Segurança** (JWT) para autenticação e proteção das rotas da API.

---

## 📦 Como Instalar e Usar  

### 🔧 Pré-requisitos  
Antes de começar, certifique-se de ter instalado:  
- 🛠️ **.NET SDK (6.0 ou superior)**  
- 🖋️ Um editor como **Visual Studio** ou **Visual Studio Code**  

### 🏗️ Passo a Passo  

1️⃣ Clone o repositório:  
```bash
git clone https://github.com/Morettys2/CarrinhoComprasAPI.git
cd CarrinhoComprasAPI
```  

2️⃣ Restaure as dependências:  
```bash
dotnet restore
```  

3️⃣ Compile o projeto:  
```bash
dotnet build
```  

4️⃣ Execute a aplicação:  
```bash
dotnet run
```  

5️⃣ Acesse a API em **`http://localhost:5000`** ou conforme a URL exibida no terminal.  

---

## 🔗 Endpoints  

### 🛍️ Produtos  

- **GET** `/produtos`  
  Lista todos os produtos no carrinho.  

- **POST** `/produtos`  
  Adiciona um produto ao carrinho.  
  **Exemplo de Body**:  
  ```json
  {
    "nome": "Produto Exemplo",
    "preco": 10.50,
    "quantidade": 2
  }
  ```  

- **PUT** `/produtos/{id}`  
  Atualiza a quantidade de um produto no carrinho.  
  **Exemplo de Body**:  
  ```json
  {
    "quantidade": 3
  }
  ```  

- **DELETE** `/produtos/{id}`  
  Remove um produto do carrinho.  

### 💰 Total  

- **GET** `/total`  
  Calcula o total do carrinho.  

### 🔑 Autenticação  

- **POST** `/auth/login`  
  Autentica o usuário e gera um **Token JWT** para autenticação nas rotas protegidas.  
  **Exemplo de Body**:  
  ```json
  {
    "usuario": "exemplo@dominio.com",
    "senha": "senhaSegura123"
  }
  ```  

---

## 🎯 Objetivo  

Este projeto foi desenvolvido com os seguintes objetivos:  
- Praticar **C#** e o desenvolvimento de APIs utilizando o **.NET Minimal API**.  
- Aprender conceitos como **CRUD**, manipulação de dados e endpoints REST.  
- Explorar a estrutura e organização de um backend básico.  
- Implementar **autenticação JWT** para proteger rotas da API.

---

## ✨ Melhorias Futuras  

- 🌟 Adicionar autenticação e autorização com perfis de usuário (admin, cliente, etc.).  
- 🌟 Suporte a diferentes moedas.  
- 🌟 Integração com gateway de pagamento.  
- 🌟 Criar uma interface front-end para consumir a API.  

---
