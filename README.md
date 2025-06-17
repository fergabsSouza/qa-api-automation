# QA API Automation 🚀
👉 Este repositório é um exemplo prático de automação de testes de API backend utilizando TypeScript, Jest e Supertest, com foco na API pública [ReqRes](https://reqres.in/).

## ✅ Tecnologias Utilizadas

- **Node.js**
- **TypeScript**
- **Jest**
- **Supertest**
- **Ajv** (para validação de contrato - JSON Schema)
- **GitHub Actions** (Pipeline CI/CD)
- **GitHub Copilot** (assistente de código)

---

## 🚀 Estrutura de Pastas

    qa-api-automation/
    ├── .github/
    │   └── workflows/
    │       └── ci.yml
    ├── src/
    │   └── tests/
    │       ├── get/
    │       │   └── listUsers.test.ts
    │       ├── post/
    │       │   └── createUser.test.ts
    │       ├── put/
    │       │   └── updateUser.test.ts
    │       ├── delete/
    │       │   └── deleteUser.test.ts
    │       ├── auth/
    │       │   └── login.test.ts
    │       └── contract/
    │           └── userContract.test.ts
    ├── schemas/
    │   └── userSchema.json
    ├── utils/
    │   └── api-client.ts
    ├── .gitignore
    ├── jest.config.ts
    ├── package.json
    ├── tsconfig.json
    ├── CopilotConfig.md
    └── README.md


---

## 📌 Estrutura de Branches

| Tipo de Branch | Regra |
|---|---|
| `main` | Branch base, apenas para PRs |
| `feature/*`, `bugfix/*`, etc | Branchs livres para todos os colaboradores |
| `prod` | Apenas o owner pode fazer merge |

**👉 Proteção de branch ativa para a branch `prod`.**

---

## 📋 Como Rodar os Testes Localmente

### Pré-requisitos:

- Node.js >= 18.x
- npm

### Passos:

```bash
git clone https://github.com/seu-usuario/qa-api-automation.git
cd qa-api-automation
npm install
npm run test

