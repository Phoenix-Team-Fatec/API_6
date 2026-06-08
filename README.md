# API-6 — DomRock

<span id="topo"></span>
<h1 align="center"> FATEC SJC - 6º Semestre ADS — DomRock </h1>
<br>

## 📍 Objetivo

Desenvolvimento de uma aplicação web (RuleAI) que utiliza técnicas de IA Generativa para criação, gerenciamento e controle de regras de negócio, permitindo que gestores interajam com o sistema por meio de linguagem natural e acompanhem os resultados por meio de indicadores e gráficos, promovendo maior explicabilidade e eficiência nas decisões.

<br><br>

## ➯ Backlog do Produto

| Rank | Prioridade | US | Estimativa | Sprint | Requisitos do parceiro |
|------|------------|----|------------|--------|--------------------------|
| #1  | Alta  | Como gerente, quero utilizar linguagem natural em texto para criar novas regras de negócio, facilitando alteração de comissões. | 21 | 1 | RF1 |
| #2  | Alta  | Como gerente, quero listar as regras de negócio vigentes, para ter uma visão geral das regras. | 8  | 1 | RF2 |
| #3  | Alta  | Como gerente, quero ver o resultado de forma clara, da regra de negócio criada, em texto ou em código. | 8  | 2 | RF3 |
| #4  | Média | Como gerente, quero conseguir visualizar os funcionários, as lojas e as marcas e especificações. | 13 | 2 | RF4 |
| #5  | Média | Como gerente, quero conseguir calcular as comissões dos funcionários, as lojas e as marcas e especificações. | 13 | 2 | RF5 |
| #6  | Média | Como gerente, quero conseguir auditar o cálculo de comissão. | 13 | 3 | RF6 |
| #7  | Baixa | Como gerente, quero acompanhar e observar o funcionamento do sistema para entender seu desempenho e eficiência. | 8  | 3 | RF9 |

<br><br>

## 🧭 Requisitos Funcionais

| Código | Descrição (derivada das US) |
|:-----:|:------------------------------|
| RF01 | O sistema deve permitir que o usuário crie novas regras de negócio utilizando linguagem natural em texto, facilitando a definição de comissões. |
| RF02 | O sistema deve permitir a listagem das regras de negócio vigentes, apresentando uma visão geral ao usuário. |
| RF03 | O sistema deve apresentar de forma clara o resultado da regra de negócio criada, podendo ser exibido em formato textual ou em código. |
| RF04 | O sistema deve permitir a visualização dos funcionários, das lojas, das marcas e suas especificações. |
| RF05 | O sistema deve permitir o cálculo das comissões considerando funcionários, lojas, marcas e suas especificações. |
| RF06 | O sistema deve permitir a auditoria das comissões. |
| RF07 | O sistema deve permitir o acompanhamento e a observação do funcionamento da aplicação, fornecendo informações sobre desempenho e eficiência. |

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
<img width="1920" height="1080" alt="PHOENIX TEAM - 6SEM - DomRock" src="https://github.com/user-attachments/assets/7c7ea29d-de1f-4a30-b1bf-493749b3f9ff" />

<br>

## 🗂️ Documentos das Sprints

[Sprint 1](./Documentação%20das%20sprints/sprint-1.md)

[Sprint 2](./Documentação%20das%20sprints/sprint2.md)

[Sprint 3](./Documentação%20das%20sprints/sprint3.md)

[Manual do Usuário](./Documentação%20das%20sprints/Manual%20do%20usuário.md)

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
