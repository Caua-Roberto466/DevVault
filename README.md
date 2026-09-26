# 🗄️ DevVault

### Sua plataforma pessoal de organização, conhecimento e planejamento de projetos

*Aprenda. Planeje. Desenvolva. Tudo em um só lugar.*

![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react&logoColor=black) ![Node.js](https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white) ![Express](https://img.shields.io/badge/API-Express-000000?style=for-the-badge&logo=express&logoColor=white) ![MariaDB](https://img.shields.io/badge/Database-MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white) ![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge)

---

## 📖 Sobre o projeto

O **DevVault** é uma plataforma web criada para estudantes de Desenvolvimento de Sistemas e programadores que querem parar de espalhar suas ideias, anotações e planejamentos entre dezenas de arquivos e apps diferentes.

Em vez de ser só mais um gerenciador de tarefas ou repositório de código, o DevVault integra três etapas essenciais da jornada de quem programa:

> **Aprender → Planejar → Desenvolver**

Tudo conectado, tudo no mesmo lugar.

---

## 🧩 Módulos principais

O sistema é dividido em três módulos que trabalham de forma integrada:

| 📁 DevVault Projects   Gerenciamento dos seus projetos pessoais: status, tecnologias, links, anotações e histórico de evolução. | 📚 DevDictionary   Sua biblioteca pessoal de conceitos técnicos, com explicações, exemplos de código e organização por categoria/tecnologia. | 🧱 ProjectBlueprint   Planejamento estruturado de um projeto antes de codar: objetivos, requisitos, funcionalidades e modelagem inicial do banco. |
| --- | --- | --- |

### 🔗 Integração entre módulos

O grande diferencial do DevVault é que **nada fica isolado**. Um conceito estudado no DevDictionary pode ser associado a um requisito no ProjectBlueprint, que por sua vez está ligado a um projeto real no DevVault Projects — permitindo enxergar a relação direta entre teoria e prática.

---

## ✨ Funcionalidades (MVP)

- [x] CRUD completo de **projetos**
- [x] CRUD completo de **conceitos técnicos**
- [x] Cadastro e gerenciamento de **tecnologias**
- [x] Cadastro e gerenciamento de **requisitos**
- [x] Relacionamento **projeto ↔ conceito**
- [x] Relacionamento **projeto ↔ tecnologia**
- [x] **Dashboard** com resumo geral
- [x] Pesquisa e filtros básicos

### 🔮 Roadmap futuro

- [ ] Editor visual de diagramas de banco de dados
- [ ] Visualização gráfica das relações entre conceitos e projetos
- [ ] Exportação de documentação técnica
- [ ] Histórico detalhado de alterações
- [ ] Sistema de etiquetas e filtros avançados
- [ ] Autenticação e múltiplos usuários
- [ ] Sincronização entre dispositivos
- [ ] Deploy online

---

## 🛠️ Stack tecnológica

| Camada | Tecnologia | Função |
| --- | --- | --- |
| **Frontend** | React | Interface, componentes e consumo da API |
| **Backend** | Node.js + Express | API REST, regras de negócio e validações |
| **Banco de dados** | MariaDB (via XAMPP, local) | Armazenamento relacional dos dados |

> O React nunca acessa o banco diretamente — toda comunicação passa pela API REST em Node.js, garantindo separação clara entre interface e dados.

---

## 🗃️ Estrutura do banco de dados (inicial)

| Tabela | Descrição |
| --- | --- |
| `projects` | Projetos pessoais cadastrados |
| `concepts` | Conceitos técnicos da biblioteca |
| `technologies` | Tecnologias utilizadas |
| `requirements` | Requisitos dos projetos |
| `features` | Funcionalidades planejadas |
| `project_technologies` | Relação N:N entre projetos e tecnologias |
| `project_concepts` | Relação N:N entre projetos e conceitos |


---

## 🚀 Como rodar o projeto localmente

### Pré-requisitos

- Node.js instalado
- XAMPP (ou outro servidor MariaDB/MySQL) rodando localmente

### 1. Clonar o repositório

```bash
git clone https://github.com/seu-usuario/devvault.git
cd devvault
```

### 2. Configurar o banco de dados

- Inicie o MariaDB pelo XAMPP
- Crie o banco `devvault`
- Importe o script SQL (quando disponível em `server/database/`)

### 3. Rodar o backend (API)

```bash
cd server
npm install
npm run dev
```

### 4. Rodar o frontend (React)

```bash
cd client
npm install
npm start
```

A aplicação estará disponível em `http://localhost:3000`, consumindo a API em `http://localhost:5000` (ou porta configurada).

---

## 🎯 Diferenciais

- **Integração real** entre teoria (DevDictionary) e prática (Projects/Blueprint)
- **Organização centralizada** de projetos, requisitos e conhecimentos
- **Planejamento estruturado** antes de sair codando
- **Biblioteca de conhecimento personalizada**, construída pelo próprio usuário
- **100% local** na primeira versão, sem dependência de serviços pagos

---

Feito para quem quer aprender, planejar e desenvolver com organização. 🚀
