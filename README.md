# 🕵️‍♂️ NLW Agents

Projeto desenvolvido durante o **NLW (Next Level Week)** da **Rocketseat**, utilizando tecnologias modernas para criação de uma **API robusta e eficiente**.

---

## 🚀 Tecnologias

- **Node.js** com **TypeScript nativo** (`--experimental-strip-types`)
- **Fastify** – Framework web rápido e eficiente
- **PostgreSQL** com extensão `pgvector` para vetores
- **Drizzle ORM** – Operações type-safe no banco de dados
- **Zod** – Validação de schemas
- **Docker** – Containerização do banco de dados
- **Biome** – Linting e formatação de código

---

## 🏗️ Arquitetura

O projeto segue uma arquitetura modular com:

- Separação de responsabilidades entre rotas, schemas e conexão com banco
- Validação de schemas com **Zod** para garantir segurança de tipos
- ORM **type-safe** com **Drizzle**
- Validação centralizada de variáveis de ambiente

---

## ⚙️ Setup e Configuração

### ✅ Pré-requisitos

- Node.js (versão com suporte a `--experimental-strip-types`)
- Docker e Docker Compose instalados

### 🔧 Passos

1. **Clone o repositório:**

```bash
git clone <url-do-repositorio>
cd server
```
2. **Clone o repositório:**

```bash
docker-compose up -d
```

3. **Crie o arquivo .env:**

```bash
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
```
4. **Instale as dependências:**

```bash
npm install
```

5. **Execute as migrações do banco:**

```bash
npx drizzle-kit migrate
```

6. **(Opcional) Popule o banco com dados de exemplo:**

```bash
npm run db:seed
```

7. **Execute o projeto:**

```bash
npm run dev
```

8. Produção:

```bash
npm start
```

---

## 📚 Scripts Disponíveis

- `npm run dev` – Executa o servidor em modo de desenvolvimento com hot reload  
- `npm start` – Executa o servidor em modo de produção  
- `npm run db:seed` – Popula o banco de dados com dados de exemplo  

---

## 🌐 Endpoints

A API estará disponível em: **http://localhost:3333**

### Endpoints disponíveis:

- `GET /health` – Health check da aplicação  
- `GET /rooms` – Lista as salas disponíveis  

---

## 🧠 Aprendizados

Durante o desenvolvimento do projeto, foram reforçados diversos conceitos importantes:

- Uso do Fastify para performance otimizada em APIs  
- Utilização de recursos avançados do Node.js com TypeScript nativo  
- Organização de código por responsabilidade  
- Validação forte com Zod  
- Integração com banco de dados PostgreSQL utilizando pgvector  
- Criação e execução de migrações com Drizzle ORM  
- Uso de Docker para ambientes consistentes de desenvolvimento  
- Boas práticas de linting e formatação com Biome  

---

## 👨‍💻 Autor

Desenvolvido com ❤️ por [Guilherme Martins](https://github.com/gmartins99) durante o evento **NLW Agents** da [Rocketseat](https://rocketseat.com.br).  

---

## 📝 Licença

Este projeto está licenciado sob a licença **MIT**. Veja o arquivo [LICENSE](./LICENSE) para mais detalhes.

