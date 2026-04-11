# API-6 — DomRock

<span id="topo"></span>
<h1 align="center"> FATEC SJC - 6º Semestre ADS — DomRock </h1>
<br>

## 📍 Objetivo

Desenvolvimento de Aplicação Web com aplicação de técnicas de IA Generativa para controle de regras de negócio.

<br><br>

## ➯ Backlog do Produto

| Rank | Prioridade | US | Estimativa | Sprint | Requisitos do parceiro |
|------|------------|----|------------|--------|--------------------------|
| #1 | Alta | Como gerente, quero utilizar linguagem natural em texto para criar novas regras de negócio, facilitando alteração de comissões. | 21 | 1 | RF1 |
| #2 | Alta | Como gerente, quero listar as regras de negócio vigentes, para ter uma visão geral das regras. | 8 | 1 | RF2 |
| #3 | Alta | Como gerente, quero ver o resultado de forma clara, da regra de negócio criada, em texto ou em código. | 8 | 1 | RF3 |
| #4 | Média | Como gerente, quero conseguir avaliar a qualidade da resposta da aplicação, para maior assertividade. | 13 | 2 | RF4 |
| #5 | Média | Como gerente, quero ver o histórico de alterações das regras de negócio, para ter uma visão ampla do fluxo de alterações. | 5 | 2 | RF5 |
| #6 | Média | Como gerente, quero alterar para versões anteriores das regras de negócio, facilitando sazonalidade de comissões. | 13 | 2 | RF6 |
| #7 | Baixa | Como gerente, quero acompanhar e observar o funcionamento do sistema para entender seu desempenho e eficiência. | 8 | 3 | RF7 |
| #8 | Baixa | Como gerente, quero ver graficos com os resultados das regras de negócio, para maior explicabilidade da aplicação. | 13 | 3 | RF8 |

<br><br>

<h2>🎯 Cenários de Teste</h2>

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Gerente acessa a funcionalidade de criação de regras e insere a frase em linguagem natural "Vendedores recebem 10% de comissão em vendas acima de 1000 reais".<br><br>**Resultado esperado:** Sistema interpreta o texto, cria a regra de negócio e exibe o resultado das regras de negócio aplicadas. | **Ação:** Gerente tenta cadastrar uma regra com texto inválido ou incompreensível.<br><br>**Resultado esperado:** Sistema informa que a regra não pôde ser interpretada e solicita revsão. |
| **#02** | **Ação:** Gerente acessa a página de listagem de regras de negócio.<br><br>**Resultado esperado:** Sistema exibe todas as regras vigentes cadastradas e histórico. | **Ação:** Gerente acessa a listagem quando não existem regras cadastradas.<br><br>**Resultado esperado:** Sistema exibe mensagem informando que não há regras vigentes. |
| **#03** | **Ação:** Gerente acessa a lista de regras e seleciona uma regra cadastrada para visualizar.<br><br>**Resultado esperado:** Sistema exibe o resultado da regra de forma clara em formato de texto. | **Ação:** Gerente seleciona a opção de visualizar a regra em formato de código.<br><br>**Resultado esperado:** Sistema apresenta o código gerado para a regra correspondente. |


<br><br>

## 🧭 Requisitos Funcionais

| Código | Descrição (derivada das US) |
|:-----:|:------------------------------|
| RF1 | ----------------------------------------------------------------------------------------- |

<br><br>

## 🔐 Requisitos Não Funcionais (RNF)

- Manual de Instalação (no repositório).
- Manual do Usuário (no repositório).
- Modelos LLM de uso público via API (Hugging Face, Gemini, Grok, Llama, OpenAI)
- Framework Langchain, Langgraph, Llama Index, outros (Python) 
- Vue.JS para Frontend 
- SpringBoot para Backend 
- Um vídeo tutorial para demonstrar como usar para usuários que não tem domínio de tecnologia 
<br><br>

## 🗺️ MVP
![PHOENIX TEAM - 6SEM - DomRock](https://github.com/user-attachments/assets/1fb3ae0a-adf6-4259-b434-437318e261be)

<br>

## 🗂️ Documentos das Sprints

[Sprint 1](./Documentação%20das%20sprints/sprint-1.md)

[Sprint 2](./Documentação%20das%20sprints/sprint2.md)

<br>

## 🛠️ Tecnologias

- Spring/Java
- LangChain
- Vue.js
- Python
- MLFlow
- Ollama
- HuggingFace
- Groq

<br>

## 👥 Equipe

| Função | Nome | LinkedIn | GitHub |
|:-----:|:----:|:--------:|:------:|
| Porduct Owner| 	Matheus Andrade | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/matheus-andrade-santos/) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/MatheusAndrade1999) |
| Scrum Master | 	Gustavo Villela | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/gustavo-villela-a9314b268) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/TaldoGus) |
| Dev Team | Vinicius Peretta | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/vinicius-assis-peretta-5a2436227) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/Peretta) |
| Dev Team | 	Samuel Alkmin | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/samuel-alkmin-machado-52743a292) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/samekmd) |
| Dev Team | Guilherme Sato | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/guilherme-sato-42b609292) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/gsatocode) |
| Dev Team | Larissa Colucci | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/larissa-colucci-996393295) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/LarissaCGomes) |
| Dev Team | João Victor Menezes | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/jvictormo) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/jvictormo) |
| Dev Team | 	Joniel Oliveira | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/jonielrodrigues) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/JonielOliveira) |
| Dev Team | 	Mariana Tebecherani | [<img height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/LinkedIn.svg">](https://www.linkedin.com/in/mariana-tebecherani) | [<img align="center" height="30px" src="https://github.com/tandpfun/skill-icons/blob/main/icons/Github-Dark.svg"/>](https://github.com/Marianatebecherani) |
<br>

→ [Voltar ao topo](#topo)

---
