
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
<h2>🎯 Cenários de Teste da Sprint 1</h2>

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Gerente acessa a funcionalidade de criação de regras e insere a frase em linguagem natural "Vendedores recebem 10% de comissão em vendas acima de 1000 reais".<br><br>**Resultado esperado:** Sistema interpreta o texto, cria a regra de negócio e exibe o resultado das regras de negócio aplicadas. | **Ação:** Gerente tenta cadastrar uma regra com texto inválido ou incompreensível.<br><br>**Resultado esperado:** Sistema informa que a regra não pôde ser interpretada e solicita revsão. |
| **#02** | **Ação:** Gerente acessa a página de listagem de regras de negócio.<br><br>**Resultado esperado:** Sistema exibe todas as regras vigentes cadastradas e histórico. | **Ação:** Gerente acessa a listagem quando não existem regras cadastradas.<br><br>**Resultado esperado:** Sistema exibe mensagem informando que não há regras vigentes. |
| **#03** | **Ação:** Gerente acessa a lista de regras e seleciona uma regra cadastrada para visualizar.<br><br>**Resultado esperado:** Sistema exibe o resultado da regra de forma clara em formato de texto. | **Ação:** Gerente seleciona a opção de visualizar a regra em formato de código.<br><br>**Resultado esperado:** Sistema apresenta o código gerado para a regra correspondente. |

<a href="../README.md">
  <button>⬅️ Voltar ao README</button>
</a>