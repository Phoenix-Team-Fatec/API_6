# Manual do Usuário - RuleAI (DomRock)

## 📋 Índice

1. [📱 Sobre o Sistema](#-sobre-o-sistema)
2. [💻 Requisitos](#-requisitos)
3. [🚀 Instalação](#-instalação)
4. [🎯 Primeiros Passos](#-primeiros-passos)
5. [👥 Funcionalidades por Perfil](#-funcionalidades-por-perfil)
6. [📖 Guia de Uso](#-guia-de-uso)
7. [❓ Perguntas Frequentes](#-perguntas-frequentes)
8. [🆘 Suporte Técnico](#-suporte-técnico)
9. [📝 Notas da Versão](#-notas-da-versão)
10. [🏆 Créditos](#-créditos)

---

## 📱 Sobre o Sistema

O **RuleAI** é uma plataforma inteligente para **criação, gestão e avaliação de regras de negócio utilizando linguagem natural**, permitindo que usuários descrevam regras sem necessidade de conhecimento técnico em programação.

### Principais Objetivos

* Criar regras de negócio a partir de **linguagem natural**
* Traduzir regras para lógica estruturada automaticamente
* Permitir **simulação e validação de regras**
* Avaliar qualidade e assertividade das regras geradas
* Manter histórico e versionamento
* Fornecer **observabilidade e métricas**

### Tecnologias Utilizadas

* **Frontend**: React + TypeScript
* **Backend**: Node.js / Express
* **Banco de Dados**: PostgreSQL
* **IA/LLM**: Integração com modelos de linguagem
* **Autenticação**: JWT

---

## 💻 Requisitos

### Requisitos Mínimos

* Navegador atualizado (Chrome, Edge, Firefox)
* Conexão com internet
* Resolução mínima recomendada: 1366x768

### Requisitos Técnicos (Desenvolvimento)

* Node.js 18+
* Docker (opcional)
* PostgreSQL

---

## 🚀 Instalação

### Clone do Projeto

```bash
git clone https://github.com/Phoenix-Team-Fatec/API_6
cd API_6
```

### Backend

```bash
cd backend
npm install
npm run dev
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 🎯 Primeiros Passos

### 1. Acesso ao Sistema

#### Cadastro

1. Acesse a tela inicial
2. Clique em **"Cadastrar"**
3. Preencha:

   * Nome
   * Email
   * Senha
4. Confirme o cadastro

#### Login

1. Clique em **"Entrar"**
2. Informe email e senha
3. Acesse o sistema

---

### 2. Primeiro Uso

Após login:

* Acesse o painel principal
* Crie sua primeira regra
* Teste a simulação
* Avalie o resultado

---

## 👥 Funcionalidades por Perfil

### 👤 Usuário

* Criar regras em linguagem natural
* Visualizar regras criadas
* Simular execução de regras
* Avaliar qualidade das regras
* Visualizar histórico
* Editar regras

---

### 👨‍💼 Administrador

* Gerenciar usuários
* Monitorar uso do sistema
* Visualizar métricas e logs
* Controlar regras globais

---

## 📖 Guia de Uso

### 🧠 Criação de Regras

#### Criar Regra em Linguagem Natural

1. Acesse **"Nova Regra"**
2. Digite a regra, por exemplo:

   * "Se o cliente tiver mais de 5 compras, aplicar 10% de desconto"
3. Clique em **"Gerar Regra"**

O sistema irá:

* Interpretar a regra
* Converter para lógica estruturada
* Exibir o resultado

---

### 🔍 Visualização de Regras

1. Acesse **"Minhas Regras"**
2. Veja:

   * Nome
   * Descrição
   * Status
   * Data de criação

---

### ▶️ Simulação de Regras

1. Selecione uma regra
2. Clique em **"Simular"**
3. Insira dados de teste
4. Visualize o resultado

---

### ⭐ Avaliação de Qualidade

Após gerar uma regra:

* Avalie:

  * Clareza
  * Precisão
  * Utilidade
* Atribua uma nota
* Salve feedback

---

### 🕓 Histórico e Versionamento

Cada regra possui:

* Histórico de alterações
* Versões anteriores
* Data e autor da modificação

---

### 📊 Observabilidade

O sistema fornece:

* Logs de execução
* Métricas de uso
* Taxa de acerto das regras
* Avaliações dos usuários

---

## ❓ Perguntas Frequentes

### Sobre o Sistema

**P: Preciso saber programar?**
R: Não. O sistema aceita linguagem natural.

**P: Posso editar uma regra depois?**
R: Sim, e o histórico será mantido.

---

### Sobre Regras

**P: A IA pode errar?**
R: Sim. Por isso existe avaliação e simulação.

**P: Posso testar antes de usar?**
R: Sim, através da simulação.

---

### Segurança

**P: Meus dados estão seguros?**
R: Sim. O sistema utiliza autenticação JWT e boas práticas de segurança.

---

## 🆘 Suporte Técnico

* Repositório:
  https://github.com/Phoenix-Team-Fatec/API_6

* Equipe de desenvolvimento: Phoenix Team

---

## 📝 Notas da Versão

### Versão Atual: 1.0.0

**Funcionalidades Implementadas:**

* ✅ Criação de regras com linguagem natural
* ✅ Interpretação com IA
* ✅ Simulação de regras
* ✅ Avaliação de qualidade
* ✅ Histórico e versionamento
* ✅ Autenticação de usuários
* ✅ Observabilidade básica

---

## 🏆 Créditos

**Desenvolvido por**: Phoenix Team - FATEC São José dos Campos
**Projeto Acadêmico**: API 6º Semestre
**Empresa Parceira**: DomRock

---

**Última atualização**: 2026
**Versão do manual**: 1.0

---

*Este documento pode evoluir conforme novas funcionalidades forem implementadas.*
