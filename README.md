# Projeto Livros (Book Manager)

Este projeto é uma aplicação web desenvolvida com **Node.js**, **Express.js** e **Handlebars**, que permite o gerenciamento de livros. A aplicação permite cadastrar, visualizar, editar e excluir livros, armazenando os dados em um banco de dados.

## 📚 Funcionalidades

- ✅ Cadastro de livros
- 📄 Listagem de livros cadastrados
- ✏️ Edição de informações de livros
- ❌ Remoção de livros do sistema

## 🛠 Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [Express-Handlebars](https://www.npmjs.com/package/express-handlebars)
- [MySQL](https://www.mysql.com/) (via `mysql2`)
- [Body-Parser](https://www.npmjs.com/package/body-parser)
- [dotenv](https://www.npmjs.com/package/dotenv)

## 📁 Estrutura de Diretórios

```
projeto1/
├── db/
│   └── conn.js             # Configuração da conexão com banco de dados
├── public/
│   └── css/style.css       # Estilo da aplicação
├── views/
│   ├── layouts/
│   │   └── main.handlebars # Layout base
│   ├── home.handlebars     # Página inicial
│   ├── books.handlebars    # Lista de livros
│   ├── book.handlebars     # Detalhes de um livro
│   └── editbook.handlebars # Formulário de edição
├── index.js                # Arquivo principal da aplicação
├── package.json            # Dependências e scripts
└── package-lock.json
```

## 🔌 Conexão com Banco de Dados

A conexão com o banco de dados está definida no arquivo:

```
db/conn.js
```

Certifique-se de configurar corretamente seu banco MySQL e definir as variáveis de ambiente no arquivo `.env`:

```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=sua_senha
DB_NAME=nome_do_banco
```

## ▶️ Como Rodar o Projeto

1. **Clone o repositório:**

```bash
git clone <url-do-repo>
cd projeto1
```

2. **Instale as dependências:**

```bash
npm install
```

3. **Configure o banco de dados:**

Crie um banco de dados MySQL com o nome especificado no `.env`.

4. **Rode o projeto:**

```bash
npm start
```

5. **Acesse no navegador:**

```
http://localhost:3000
```

## 📌 Observações

- O projeto utiliza `express-handlebars` como motor de visualização.
- Todas as páginas HTML são renderizadas a partir das views `.handlebars`.
- O CSS está localizado em `public/css/style.css`.

---

Desenvolvido com 💻 por Vinicius Cordeiro Ribeiro.