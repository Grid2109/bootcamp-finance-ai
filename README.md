<div align="center">
  <img src="public/logo.svg" alt="Finance AI Logo" width="220" />

  <p align="center">
    <strong>Plataforma inteligente de gestão e planejamento financeiro pessoal potencializada por Inteligência Artificial.</strong>
  </p>

  <p align="center">
    <a href="#-sobre-o-projeto">Sobre</a> •
    <a href="#-funcionalidades">Funcionalidades</a> •
    <a href="#-demonstração--telas">Telas</a> •
    <a href="#-tecnologias">Tecnologias</a> •
    <a href="#-como-executar">Como Executar</a> •
    <a href="#-estrutura-do-projeto">Estrutura</a> •
    <a href="#-autora">Autora</a>
  </p>

  <p align="center">
    <img src="https://img.shields.io/badge/Next.js_14-black?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js 14" />
    <img src="https://img.shields.io/badge/React_18-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React 18" />
    <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
    <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" />
    <img src="https://img.shields.io/badge/Prisma_ORM-2D3748?style=for-the-badge&logo=prisma&logoColor=white" alt="Prisma" />
    <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
    <img src="https://img.shields.io/badge/Clerk_Auth-6C47FF?style=for-the-badge&logo=clerk&logoColor=white" alt="Clerk" />
  </p>
</div>

---

## 📌 Sobre o Projeto

O **Finance AI** é uma aplicação web moderna voltada para o controle financeiro pessoal completo, desenvolvida durante o bootcamp da **Full Stack Club (FSC)**.

A plataforma combina o poder do **Next.js 14 (App Router)** com componentes reutilizáveis do **shadcn/ui**, autenticação segura de nível de produção com **Clerk**, modelagem de dados relacional com **Prisma ORM** e banco **PostgreSQL**, e integração com **Inteligência Artificial** para geração de relatórios e insights de gastos automatizados.

> 🚧 **Status do Projeto:** Em desenvolvimento contínuo. A camada de autenticação, design system base e estrutura de banco de dados já estão implementadas e funcionais.

---

## ✨ Funcionalidades

### ✅ Já Implementadas
- **Autenticação Segura com Clerk**:
  - Fluxo completo de login, cadastro e logout.
  - Suporte a login social (Google) e credenciais (e-mail/senha).
  - Rotas protegidas via middleware e Server Components.
- **Interface Moderna e Responsiva**:
  - Construída com Tailwind CSS e shadcn/ui.
  - Tipografia personalizada com a fonte **Mulish**.
  - Experiência visual imersiva na tela de boas-vindas/login.
- **Banco de Dados e Modelagem com Prisma**:
  - Schema de transações financeiras (`Transaction`) estruturado com tipagem estrita para tipos (`DEPOSIT`, `EXPENSE`, `INVESTMENT`), categorias (`FOOD`, `TRANSPORTATION`, `HOUSING`, etc.) e métodos de pagamento (`PIX`, `CREDIT_CARD`, `BANK_SLIP`, etc.).
- **Boas Práticas de Código e Padronização**:
  - Husky, Git Commit Msg Linter, Lint-Staged, Prettier e ESLint configurados para garantir integridade e commits semânticos.

### 🚀 Roadmap / Próximos Passos
- [ ] **Módulo de Transações**:
  - Listagem completa de receitas, despesas e investimentos em tabela interativa.
  - Modal de criação, edição e exclusão de transações com validação via Zod + React Hook Form.
  - Vínculo direto de cada transação ao usuário logado (`userId`).
- [ ] **Dashboard Financeiro Interativo**:
  - Cards de saldo total, receitas do mês, despesas e taxa de economia.
  - Gráficos visuais por categoria e método de pagamento.
  - Filtro dinâmico por mês/ano.
- [ ] **Consultor Financeiro com IA**:
  - Geração de diagnósticos de gastos e recomendações inteligentes de economia utilizando modelos de IA.
- [ ] **Planos e Assinaturas (Stripe)**:
  - Integração de pagamentos para liberação de recursos avançados de IA.

---

## 📸 Demonstração & Telas

<div align="center">
  <h3>1. Tela de Boas-Vindas e Login</h3>
  <img src=".github/assets/01-tela-login.png" alt="Tela de Login do Finance AI" width="100%" />
  <p><em>Interface inicial com branding, apresentação da plataforma e botão de acesso direto.</em></p>
</div>

<br />

<div align="center">
  <h3>2. Autenticação e Login (Clerk)</h3>
  <img src=".github/assets/02-clerk-sign-in.png" alt="Tela de Sign In com Clerk" width="100%" />
  <p><em>Fluxo de login com autenticação Google em um clique ou e-mail.</em></p>
</div>

<br />

<div align="center">
  <h3>3. Criação de Conta (Sign Up)</h3>
  <img src=".github/assets/03-clerk-sign-up.png" alt="Tela de Sign Up com Clerk" width="100%" />
  <p><em>Formulário de cadastro ágil, seguro e integrado ao provedor de identidade.</em></p>
</div>

---

## 🛠️ Tecnologias

As seguintes ferramentas e bibliotecas formam a base desta aplicação:

- **Frontend & Framework**: [Next.js 14](https://nextjs.org/) (App Router & Server Actions)
- **Linguagem**: [TypeScript](https://www.typescriptlang.org/)
- **Estilização**: [Tailwind CSS](https://tailwindcss.com/) & [shadcn/ui](https://ui.shadcn.com/)
- **Ícones**: [Lucide React](https://lucide.dev/)
- **Autenticação**: [Clerk](https://clerk.com/)
- **ORM & Banco de Dados**: [Prisma](https://www.prisma.io/) com [PostgreSQL](https://www.postgresql.org/) (hospedado no [Neon](https://neon.tech/))
- **Qualidade de Código**: [ESLint](https://eslint.org/), [Prettier](https://prettier.io/), [Husky](https://typicode.github.io/husky/) e [lint-staged](https://github.com/lint-staged/lint-staged)

---

## 🚀 Como Executar o Projeto Localmente

### Pré-requisitos
Certifique-se de ter instalado em sua máquina:
- [Node.js](https://nodejs.org/) (versão 18.x ou superior)
- Gerenciador de pacotes `npm`, `yarn` ou `pnpm`
- Uma conta no [Clerk](https://clerk.com/) para obter as chaves de autenticação
- Uma instância de banco PostgreSQL (recomendado: [Neon Database](https://neon.tech/))

### 1. Clonar o repositório
```bash
git clone https://github.com/Grid2109/bootcamp-finance-ai.git
cd bootcamp-finance-ai
```

### 2. Instalar as dependências
```bash
npm install
```

### 3. Configurar as variáveis de ambiente
Crie um arquivo `.env` na raiz do projeto baseado no `.env.example`:

```bash
cp .env.example .env
```

Preencha com as suas credenciais:
```env
# Banco de Dados (PostgreSQL / Neon)
DATABASE_URL="postgresql://usuario:senha@host:5432/financeai?sslmode=require"

# Autenticação Clerk
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_...
CLERK_SECRET_KEY=sk_test_...
```

### 4. Executar as migrações do banco de dados
Sincronize o banco de dados com o schema do Prisma:
```bash
npx prisma migrate dev
```

### 5. Iniciar o servidor de desenvolvimento
```bash
npm run dev
```

Abra [http://localhost:3000](http://localhost:3000) no seu navegador para ver a aplicação em execução.

---

## 📂 Estrutura do Projeto

```plaintext
bootcamp-finance-ai/
├── app/
│   ├── (auth)/login/       # Página de Login e autenticação
│   ├── _components/        # Componentes compartilhados e shadcn/ui
│   ├── _lib/               # Funções utilitárias (ex: cn helper)
│   ├── layout.tsx          # Root Layout com Mulish font e ClerkProvider
│   └── page.tsx            # Página inicial protegida por autenticação
├── prisma/
│   ├── schema.prisma       # Definição do banco e enums (Transaction, Types, Categories)
│   └── migrations/         # Histórico de migrações do banco
├── public/                 # Assets públicos estáticos (logo.svg, login.png)
├── .github/
│   └── assets/             # Imagens e prints sequenciais para o README
├── middleware.ts           # Middleware de proteção de rotas do Clerk
├── components.json         # Configuração do shadcn/ui
└── package.json            # Dependências e scripts do projeto
```

---

## 🤝 Créditos & Agradecimentos

Este projeto está sendo desenvolvido como parte dos estudos práticos do bootcamp promovido pela **[Full Stack Club (FSC)](https://fullstackclub.com.br/)**, ministrado por **Felipe Rocha**, focado nas tecnologias mais modernas do ecossistema Full Stack JavaScript/TypeScript e Inteligência Artificial aplicada a produtos reais.

---

## 👩‍💻 Autora

<div align="left">
  <p>Desenvolvido com dedicação por <strong>Ingrid Lira</strong>.</p>
  
  <a href="https://github.com/Grid2109" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-Grid2109-181717?style=for-the-badge&logo=github" alt="GitHub" />
  </a>
  &nbsp;
  <a href="https://www.linkedin.com/in/grid-lira" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-grid--lira-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn" />
  </a>
</div>

---

<div align="center">
  <sub>⭐️ Se você achou este projeto interessante, deixe uma estrela no repositório!</sub>
</div>
