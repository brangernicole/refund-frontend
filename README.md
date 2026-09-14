# 💰 Refund

Interface web para solicitação e análise de **reembolsos corporativos**, desenvolvida com React, TypeScript, Vite e Tailwind CSS.

O projeto possui dois fluxos principais:

* 👤 **Colaborador:** realiza uma solicitação de reembolso informando a despesa e anexando o comprovante.
* 👨‍💼 **Gestor:** visualiza as solicitações, pesquisa por nome e acessa os detalhes de cada reembolso.

> 🚧 **Status:** Front-end concluído. O Back-end será desenvolvido posteriormente para adicionar autenticação, persistência de dados e integração com API.

## ✨ Funcionalidades

### 👤 Colaborador

* Cadastro de usuário
* Login
* Solicitação de reembolso
* Seleção da categoria da despesa
* Inserção do valor
* Upload de comprovante
* Tela de confirmação após o envio

### 👨‍💼 Gestor

* Dashboard com solicitações de reembolso
* Pesquisa por nome
* Paginação
* Visualização dos detalhes de uma solicitação
* Acesso ao comprovante demonstrativo

### 🧩 Interface

* Design responsivo
* Componentes reutilizáveis
* Formulários controlados
* Navegação entre diferentes fluxos da aplicação
* Organização de rotas por perfil de usuário

## 🛠️ Tecnologias

* **React 19**
* **TypeScript**
* **Vite**
* **React Router**
* **Tailwind CSS 4**
* **clsx**
* **tailwind-merge**

## 📂 Estrutura do projeto

```text
src/
├── assets/       # Imagens e ícones
├── components/   # Componentes reutilizáveis
├── pages/        # Telas da aplicação
├── routes/       # Configuração das rotas
└── utils/        # Utilitários e funções auxiliares
```

### Principais arquivos

* `src/routes/index.tsx` — configuração dos fluxos da aplicação
* `src/pages/SignIn.tsx` — tela de login
* `src/pages/SignUp.tsx` — tela de cadastro
* `src/pages/Refund.tsx` — solicitação e visualização de reembolso
* `src/pages/Dashboard.tsx` — dashboard do gestor
* `src/pages/Confirm.tsx` — confirmação da solicitação
* `src/components/` — componentes reutilizáveis da interface

## 🚀 Como executar

### Pré-requisitos

* [Node.js](https://nodejs.org/) instalado
* npm instalado

### Instalação

```bash
npm install
```

### Desenvolvimento

```bash
npm run dev
```

Depois, acesse a URL exibida no terminal, normalmente:

```text
http://localhost:5173
```

### Build

```bash
npm run build
```

### Preview do build

```bash
npm run preview
```

## 🗺️ Rotas

### Acesso público

| Rota      | Tela     |
| --------- | -------- |
| `/`       | Login    |
| `/signup` | Cadastro |

### Colaborador

| Rota       | Tela                     |
| ---------- | ------------------------ |
| `/`        | Solicitação de reembolso |
| `/confirm` | Confirmação              |

### Gestor

| Rota          | Tela                  |
| ------------- | --------------------- |
| `/`           | Dashboard             |
| `/refund/:id` | Detalhes do reembolso |

## 🔄 Fluxo da aplicação

```text
                    ┌──────────────┐
                    │    Login     │
                    └──────┬───────┘
                           │
                ┌──────────┴──────────┐
                │                     │
                ▼                     ▼
        👤 Colaborador          👨‍💼 Gestor
                │                     │
                ▼                     ▼
        Solicitar reembolso      Dashboard
                │                     │
                ▼                     ▼
           Confirmação          Detalhes
                                      │
                                      ▼
                                Comprovante
```

## 📌 Estado atual

Atualmente, o projeto está com o **Front-end desenvolvido e funcional em modo de demonstração**.

Os dados utilizados na aplicação ainda são demonstrativos e não estão conectados a uma API ou banco de dados.

### Próximos passos

* [ ] Desenvolver API do Back-end
* [ ] Implementar autenticação
* [ ] Criar persistência de usuários
* [ ] Persistir solicitações de reembolso
* [ ] Conectar o dashboard à API
* [ ] Implementar busca e paginação com dados reais
* [ ] Implementar armazenamento de comprovantes
* [ ] Adicionar tratamento de erros e estados de carregamento
* [ ] Integrar Front-end e Back-end

## 🌐 Deploy

**Front-end:** [Vercel](#)

> O link será adicionado após o deploy.

## 🎓 Projeto

Projeto desenvolvido durante os estudos de **Desenvolvimento Web na Rocketseat**, com foco na construção de uma aplicação Front-end utilizando React, TypeScript e Tailwind CSS.

---