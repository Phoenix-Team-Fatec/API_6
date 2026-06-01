## 📥 Definition of Ready (DoR)
### Sprint 3
Uma User Story só poderá entrar na Sprint 3 se:
- Atender todos os critérios do DoR da Sprint 2  
- Estiver relacionada à auditoria de comissões, monitoramento ou observabilidade do sistema  
- Depender de funcionalidades já consolidadas nas Sprints anteriores  
- Possuir regras de negócio e fluxos de auditoria bem definidos  
- Estiver refinada, priorizada e compreendida pelo time  

## ✅ Definition of Done (DoD)
### Sprint 3
Uma User Story será considerada concluída quando:
- O fluxo de auditoria de cálculo de comissão estiver funcional e validado  
- O painel/mecanismo de monitoramento de desempenho e eficiência do sistema estiver operando  
- O sistema apresentar tratamento adequado de erros e exceções nas novas rotas  
- Logs e métricas de funcionamento do sistema estiverem sendo registrados corretamente  
- Não houver erros críticos que comprometam as regras de auditoria ou a coleta de dados de desempenho  

---

## 📋 Backlog da Sprint 3

| RANK | TIPO | ITEM | US | STATUS |
| :--: | :-- | :-- | :--: | :--: |
|#1|Frontend| Tela/Painel para visualização da auditoria de cálculo de comissão | US #6 |✅|
|#2|Frontend| Tela/Dashboard de acompanhamento e observabilidade do sistema (gráficos/indicadores) | US #7 |✅|
|#3|Frontend| Exibição de mensagens de erro e sucesso (feedback ao usuário nas telas de auditoria/métricas) | US #6 / US #7 |✅|
|#4|Frontend| Validação das regras de negócio de auditoria na interface | US #6 |✅|
|#5|Back/Front| Integração do fluxo de auditoria e logs de monitoramento entre frontend e backend | US #6 / US #7 |✅|
|#6|Backend| Implementar motor/regras de auditoria do cálculo de comissão | US #6 |✅|
|#7|Backend| Implementar a coleta de logs e métricas de desempenho/eficiência do sistema | US #7 |✅|
|#8|Backend| Criar endpoints para fornecer dados de auditoria e desempenho ao frontend | US #6 / US #7 |✅|
|#9|Backend| Melhorar tratamento de erros e exceções nos fluxos de auditoria e monitoramento | US #6 / US #7 |✅|
|#10|Backend| Implementar paginação nas listagens de auditoria/logs | US #6 / US #7 |✅|
|#11|ML/IA| Melhorar precisão do agente na geração e explicação de regras para fins de auditoria | US #6 |✅|
|#12|ML/IA| Implementar fallback para falhas do agente na análise de auditoria | US #6 |✅|
|#13|ML/IA| Mostrar quantidade de tokens consumidos nas interações e logs de observabilidade | US #7 |✅|
|#14|Scrum Master| Revisar PRs, validar entregas e realizar merge | - |✅|

---

## ✅ Critérios de Aceitação da Sprint 3

| RANK | ITEM | STATUS |
| :--: | :-- | :--: |
|#1|O sistema deve apresentar uma tela/painel funcional para auditar o cálculo de comissões.|✅|
|#2|O sistema deve permitir o acompanhamento e observação do desempenho do sistema através de indicadores claros.|✅|
|#3|O sistema deve exibir mensagens claras de erro e sucesso ao usuário ao realizar ações de auditoria ou carregar métricas.|✅|
|#4|O sistema deve validar as regras de negócio associadas à auditoria antes de sua exibição/execução.|✅|
|#5|O fluxo de auditoria e o envio de dados de observabilidade devem estar integrados entre frontend e backend.|✅|
|#6|O backend deve calcular e expor o histórico estruturado dos passos do cálculo de comissão para fins de auditoria.|✅|
|#7|O sistema deve registrar logs detalhados de operação para que o gestor entenda o desempenho e a eficiência da aplicação.|✅|
|#8|O backend deve fornecer dados otimizados para a construção de gráficos de desempenho no frontend.|✅|
|#9|O sistema deve tratar erros e exceções de forma controlada nos novos módulos de auditoria e logs.|✅|
|#10|O sistema deve implementar paginação nas listagens de auditoria e logs volumosos.|✅|
|#11|O agente de IA deve apresentar melhoria na precisão ao detalhar o porquê do cálculo da comissão.|✅|
|#12|O sistema deve possuir fallback para falhas do agente de IA nos fluxos de auditoria.|✅|
|#13|O sistema deve exibir e registrar de forma clara a quantidade de tokens utilizados pelo agente para monitoramento.|✅|
|#14|Os pull requests devem ser revisados, aprovados e integrados corretamente pela liderança técnica/Scrum Master.|✅|

---

## 🎯 Cenários de Teste da Sprint 3

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Gestor acessa o painel de auditoria de comissão.<br><br>**Resultado esperado:** O histórico e os passos do cálculo são exibidos detalhadamente. | **Ação:** Falha ao carregar os dados de auditoria.<br><br>**Resultado esperado:** Sistema informa erro e orienta a tentar novamente. |
| **#02** | **Ação:** Gestor acessa a tela de observabilidade da aplicação.<br><br>**Resultado esperado:** Gráficos e indicadores de desempenho carregam corretamente. | **Ação:** Dados de monitoramento vazios ou indisponíveis.<br><br>**Resultado esperado:** Sistema informa a ausência de dados de forma amigável. |
| **#03** | **Ação:** Sistema exibe feedback após gerar um relatório de auditoria.<br><br>**Resultado esperado:** Feedback visual é claro e indica sucesso. | **Ação:** Ocorre um erro interno ao processar a requisição de logs.<br><br>**Resultado esperado:** Sistema exibe mensagem de erro controlada. |
| **#04** | **Ação:** Frontend valida consistência dos dados de auditoria enviados pelo usuário.<br><br>**Resultado esperado:** Dados consistentes são processados normalmente. | **Ação:** Dados inconsistentes para filtragem de auditoria são inseridos.<br><br>**Resultado esperado:** O sistema bloqueia a requisição e aponta o campo inválido. |
| **#05** | **Ação:** Frontend solicita dados de desempenho em tempo real ao backend.<br><br>**Resultado esperado:** Backend responde e os gráficos atualizam com sucesso. | **Ação:** Backend fica fora do ar durante a atualização dos gráficos.<br><br>**Resultado esperado:** O frontend exibe um aviso de falha na conexão sem quebrar o layout. |
| **#06** | **Ação:** Backend executa a rota que reconstrói a lógica de uma comissão calculada.<br><br>**Resultado esperado:** O cálculo bate perfeitamente com os critérios da regra vigente na época. | **Ação:** Parâmetros de comissão antigos foram corrompidos no banco.<br><br>**Resultado esperado:** Backend lança exceção tratada indicando inconsistência no registro histórico. |
| **#07** | **Ação:** A aplicação realiza uma chamada de IA e registra tempo de resposta e consumo.<br><br>**Resultado esperado:** O log de desempenho é salvo no banco com os dados de eficiência. | **Ação:** Falha na gravação do log de monitoramento.<br><br>**Resultado esperado:** O sistema redireciona a falha para um log secundário e não interrompe a experiência do usuário. |
| **#08** | **Ação:** Frontend consome os endpoints específicos de auditoria e logs.<br><br>**Resultado esperado:** Retorno de dados no formato esperado (JSON estruturado). | **Ação:** Endpoint de métricas de tokens falha.<br><br>**Resultado esperado:** Sistema retorna um código HTTP de erro tratado (ex: 500 ou 503). |
| **#09** | **Ação:** Ocorre uma falha inesperada no motor de cálculo durante a auditoria.<br><br>**Resultado esperado:** O sistema captura o erro e envia uma mensagem limpa para a tela. | **Ação:** Erro crítico não mapeado acontece na observabilidade.<br><br>**Resultado esperado:** O sistema exibe um fallback genérico, mantendo a aplicação de pé. |
| **#10** | **Ação:** Gestor navega pelas páginas do relatório de auditoria de comissões.<br><br>**Resultado esperado:** Dados carregam de forma paginada e rápida. | **Ação:** Página de logs inexistente é solicitada manualmente pela URL.<br><br>**Resultado esperado:** O sistema redireciona para a primeira página ou retorna erro controlado. |
| **#11** | **Ação:** Agente explica os critérios utilizados no cálculo da comissão de uma loja.<br><br>**Resultado esperado:** Explicação clara, precisa e condizente com a regra gravada. | **Ação:** Input de auditoria do agente é confuso ou ambíguo.<br><br>**Resultado esperado:** IA responde pedindo para especificar melhor o período ou funcionário. |
| **#12** | **Ação:** Agente de IA cai ou excede o timeout ao gerar uma análise de eficiência.<br><br>**Resultado esperado:** O sistema ativa o fallback e mostra as regras puras em texto pré-calculadas. | **Ação:** O próprio mecanismo de fallback falha.<br><br>**Resultado esperado:** O sistema apresenta a última versão estável dos dados salvos em cache. |
| **#13** | **Ação:** Sistema coleta dados de uso da API de IA para o painel de eficiência.<br><br>**Resultado esperado:** Quantidade exata de tokens consumidos é exibida em tela. | **Ação:** Falha na contagem ou retorno de tokens pela API externa.<br><br>**Resultado esperado:** O campo exibe "Não disponível" sem interromper o fluxo de monitoramento. |
| **#14** | **Ação:** Um Pull Request focado em melhoria de performance (US #7) é submetido.<br><br>**Resultado esperado:** Scrum Master/Time revisa, valida os critérios de aceitação e aprova. | **Ação:** PR enviado quebra os testes unitários de auditoria.<br><br>**Resultado esperado:** PR é reprovado automaticamente ou pelo revisor até correção. |

<br>
<a href="../README.md">
  <button>⬅️ Voltar ao README</button>
</a>
