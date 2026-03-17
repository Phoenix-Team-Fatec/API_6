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
| #7 | Baixa | Como gerente, quero ter observabilidade do sistema, para avaliar métricas de desempenho e efiência da aplicação. | 8 | 3 | RF7 |
| #8 | Baixa | Como gerente, quero ver graficos com os resultados, para mais explicabilidade da aplicação. | 13 | 3 | RF8 |

<br><br>

## 📋 Backlog da Sprint 1

| RANK | TIPO | ITEM | STATUS |
| :--: | :-- | :-- | :--: |
|#1|Backend|Criar endpoint para receber regra de negócio e parâmetros.|🕓|
|#2|ML/IA|Integrar LLM para interpretar texto e converter em estrutura lógica.|🕓|
|#3|Backend|Persistir regra de negócio convertida no banco de dados.|🕓|
|#4|Frontend|Tela de criação de regra: input de texto + preview.|🕓|
|#5|Frontend|Fluxo de confirmação: usuário revisa e aprova regra interpretada.|🕓|
|#6|Backend|Endpoint de listagem de regras vigentes com filtros.|🕓|
|#7|Frontend|Tela de listagem com tabela: Marca, Cargo, % Comissão, Data.|🕓|
|#8|Frontend|Filtros de pesquisa na listagem: por marca, cargo ou data.|🕓|
|#9|Backend|Endpoint de simulação: recebe parâmetros e retorna cálculo.|🕓|
|#10|Backend|Gerador de representação textual da regra (output interpretável).|🕓|
|#11|Backend|Gerador de representação em código (pseudocódigo da regra).|🕓|
|#12|Frontend|Tela de visualização com alternância entre modo texto e código.|🕓|
|#13|Backend|CRUD de usuários (criar, editar e desativar).|🕓|
|#14|Backend|Importação e mapeamento das bases de RH, Vendas e Comissão.|🕓|
|#15|Backend|Cálculo de vendas individuais por matrícula.|🕓|
|#16|Backend|Consolidação de vendas por loja e cálculo mensal.|🕓|
|#17|QA|Testes unitários dos endpoints principais.|🕓|
|#18|Backend|Configuração do ambiente de desenvolvimento (Docker e dependências).|🕓|
|#19|Backend|Processamento das bases respeitando data de competência.|🕓|
|#20|Backend|Relacionar base de vendas com base de RH por matrícula.|🕓|
|#21|Backend|Relacionar base de vendas com base de RH por código da loja.|🕓|
|#22|Backend|Consolidar vendas mensais por matrícula e loja.|🕓|
|#23|Backend|Regra geral: aplicar percentual de comissão por matrícula.|🕓|
|#24|Backend|Regra de gerente: comissão baseada na venda total da loja.|🕓|
|#25|Backend|Regra de admissão: cálculo proporcional aos dias trabalhados.|🕓|
|#26|Backend|Regra de demissão: cálculo proporcional aos dias efetivamente trabalhados.|🕓|
|#27|Backend|Regra de afastamento menor que 15 dias.|🕓|
|#28|Backend|Regra de afastamento maior que 15 dias.|🕓|
|#29|Backend|Regra de férias: desconto proporcional aos dias de ausência.|🕓|
|#30|Backend|Converter regras de comissão em módulo executável.|🕓|
|#31|ML/IA|Gerar representação em linguagem natural das regras.|🕓|
|#32|ML/IA|Persistir regras em banco vetorial com embeddings.|🕓|
|#33|ML/IA|Endpoint de consulta semântica para busca de regras.|🕓|
|#34|Backend|Implementar versionamento de regras no banco de IA.|🕓|
|#35|QA|Executar testes de regressão para validar cálculos.|🕓|

---

## ✅ Critérios de Aceitação da Sprint 1

| RANK | ITEM | STATUS |
| :--: | :-- | :--: |
|#1|O sistema deve permitir criar regras de negócio via endpoint.|🕓|
|#2|O texto da regra deve ser interpretado automaticamente por IA.|🕓|
|#3|A regra interpretada deve ser persistida no banco de dados.|🕓|
|#6|O sistema deve listar regras com filtros por marca, cargo ou data.|🕓|
|#9|O sistema deve permitir simulação de cálculo de comissão.|🕓|
|#14|O sistema deve importar e mapear corretamente bases de RH e vendas.|🕓|
|#19|O processamento deve respeitar a data de competência mensal.|🕓|
|#23|A comissão deve ser calculada conforme regras definidas.|🕓|
|#25|Admissões devem gerar cálculo proporcional aos dias trabalhados.|🕓|
|#26|Demissões devem gerar cálculo proporcional aos dias efetivos.|🕓|
|#27|Afastamentos menores que 15 dias devem seguir regra específica.|🕓|
|#28|Afastamentos maiores que 15 dias devem seguir regra específica.|🕓|
|#29|Férias devem descontar proporcionalmente os dias ausentes.|🕓|
|#32|As regras devem ser armazenadas em banco vetorial com embeddings.|🕓|
|#33|O usuário deve conseguir consultar regras via busca semântica.|🕓|
|#35|Os testes de regressão devem validar o resultado final das comissões.|🕓|

---
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

<br>

## 🗂️ Documentos das Sprints

- [Sprint 1]

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
