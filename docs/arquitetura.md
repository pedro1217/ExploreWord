# Arquitetura do Sistema — ExploreWorld

## 1. Arquitetura em Camadas

O ExploreWorld utilizará uma arquitetura web dividida em três camadas: apresentação, aplicação e dados.

| Camada | Tecnologias | Responsabilidade |
|---|---|---|
| Apresentação | HTML, CSS, Bootstrap e JavaScript | Telas, formulários, filtros e experiência responsiva. |
| Aplicação | PHP, controllers, models e endpoints JSON | Autenticação, regras de negócio, reservas e recomendações. |
| Dados | MySQL via PDO | Persistência de informações e consultas relacionais. |

## 2. Fluxo de Funcionamento

O sistema seguirá o seguinte fluxo:

**Navegador → Formulário/Requisição → Controller PHP → Validação e regras de negócio → Model/PDO → MySQL → Resposta HTML ou JSON.**

## 3. Organização Inicial das Pastas

```text
ExploreWorld/
├── app/
│   ├── controllers/
│   ├── models/
│   └── services/
├── config/
├── public/
│   ├── assets/
│   └── api/
├── database/
├── docs/
├── README.md
└── .gitignore
```

### Função de cada pasta

- **app/** — Controllers, models e serviços do sistema.
- **config/** — Conexão com o banco de dados e configurações.
- **public/** — Ponto de entrada e páginas públicas.
- **public/assets/** — Arquivos CSS, JavaScript e imagens.
- **public/api/** — Endpoints JSON, conforme a integração definida.
- **database/** — DER e scripts SQL do banco de dados.
- **docs/** — Protótipos e documentação do projeto.
- **README.md** — Apresentação e instruções do projeto.
- **.gitignore** — Arquivos e pastas que não devem ser enviados ao GitHub.

## 4. Ambiente de Desenvolvimento

O ExploreWorld será executado localmente utilizando **XAMPP e Apache**, com **PHP** no backend e **MySQL** para o armazenamento dos dados.

A estrutura apresentada é uma proposta inicial e poderá ser ajustada durante o desenvolvimento do sistema.
