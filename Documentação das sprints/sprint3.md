## 📥 Definition of Ready (DoR)
### Sprint 3
Uma User Story só poderá entrar na Sprint 3 se:
- Atender todos os critérios do DoR da Sprint 2  
- Estiver relacionada à autenticação, gestão de usuários, segurança ou melhorias do sistema  
- Depender de funcionalidades já consolidadas nas Sprints anteriores  
- Possuir regras de negócio e fluxos de autenticação bem definidos  
- Estiver refinada, priorizada e compreendida pelo time  

## ✅ Definition of Done (DoD)
### Sprint 3
Uma User Story será considerada concluída quando:
- O fluxo de autenticação (login, token e autorização) estiver funcional  
- O CRUD de usuários estiver implementado e validado  
- As rotas protegidas estiverem devidamente seguras  
- O sistema apresentar tratamento adequado de erros e exceções  
- Logs e métricas básicas estiverem sendo registrados corretamente  
- Não houver erros críticos que comprometam segurança ou funcionamento  

---

## 📋 Backlog da Sprint 3

| RANK | TIPO | ITEM | US | STATUS |
| :--: | :-- | :-- | :--: | :--: |
|#1|Frontend| Tela de login de usuário | - |🕓|
|#2|Frontend| Validação de campos no login (email/senha) | - |🕓|
|#3|Frontend| Persistência de sessão do usuário autenticado | - |🕓|
|#4|Frontend| Tela de gerenciamento de usuários (listagem) | - |🕓|
|#5|Frontend| Formulário para cadastro e edição de usuários | - |🕓|
|#6|Frontend| Exibição de mensagens de erro e sucesso (feedback ao usuário) | - |🕓|
|#7|Frontend| Validação das regras de negócio | - |🕓|
|#8|Back/Front| Integração do fluxo de autenticação entre frontend e backend | - |🕓|
|#9|Backend| Implementar autenticação (login) com validação de credenciais | - |🕓|
|#10|Backend| Implementar geração de token (JWT ou similar) | - |🕓|
|#11|Backend| Implementar middleware de autorização | - |🕓|
|#12|Backend| CRUD de usuários | - |🕓|
|#13|Backend| Definição de perfis de acesso (admin, padrão) | - |🕓|
|#14|Backend| Proteção de rotas sensíveis | - |🕓|
|#15|Backend| Implementar logs de operações do sistema | - |🕓|
|#16|Backend| Melhorar tratamento de erros e exceções | - |🕓|
|#17|Backend| Implementar paginação nas listagens | - |🕓|
|#18|ML/IA| Melhorar precisão do agente na geração de regras de negócio | - |🕓|
|#19|ML/IA| Implementar fallback para falhas do agente | - |🕓|
|#20|ML/IA| Mostrar quantidade de tokens | - |🕓|
|#21|Scrum Master| Revisar PRs, validar entregas e realizar merge | - |🕓|

---

## ✅ Critérios de Aceitação da Sprint 3

| RANK | ITEM | STATUS |
| :--: | :-- | :--: |
|#1|O sistema deve apresentar uma tela de login funcional para acesso do usuário.|🕓|
|#2|O sistema deve validar corretamente os campos de email e senha.|🕓|
|#3|O sistema deve manter a sessão do usuário autenticado ativa conforme configuração.|🕓|
|#4|O sistema deve permitir a visualização da lista de usuários cadastrados.|🕓|
|#5|O sistema deve permitir cadastrar e editar usuários através de formulário.|🕓|
|#6|O sistema deve exibir mensagens claras de erro e sucesso ao usuário.|🕓|
|#7|O sistema deve validar regras de negócio antes de sua execução.|🕓|
|#8|O fluxo de autenticação deve estar integrado entre frontend e backend.|🕓|
|#9|O sistema deve autenticar usuários com base em credenciais válidas.|🕓|
|#10|O sistema deve gerar tokens de autenticação seguros (JWT ou similar).|🕓|
|#11|O sistema deve restringir acessos através de middleware de autorização.|🕓|
|#12|O sistema deve permitir operações de CRUD para usuários.|🕓|
|#13|O sistema deve diferenciar perfis de acesso (admin e padrão).|🕓|
|#14|O sistema deve proteger rotas sensíveis contra acessos não autorizados.|🕓|
|#15|O sistema deve registrar logs das operações realizadas.|🕓|
|#16|O sistema deve tratar erros e exceções de forma controlada.|🕓|
|#17|O sistema deve implementar paginação nas listagens.|🕓|
|#18|O agente de IA deve apresentar melhoria na precisão das respostas.|🕓|
|#19|O sistema deve possuir fallback para falhas do agente de IA.|🕓|
|#20|O sistema deve exibir a quantidade de tokens utilizados pelo agente.|🕓|
|#21|Os pull requests devem ser revisados, aprovados e integrados corretamente.|🕓|

---

## 🎯 Cenários de Teste da Sprint 3

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Usuário acessa a tela de login.<br><br>**Resultado esperado:** Tela é exibida corretamente. | **Ação:** Página de login falha ao carregar.<br><br>**Resultado esperado:** Sistema informa erro ao usuário. |
| **#02** | **Ação:** Usuário insere email e senha válidos.<br><br>**Resultado esperado:** Validação é aceita. | **Ação:** Usuário insere dados inválidos.<br><br>**Resultado esperado:** Sistema exibe erro de validação. |
| **#03** | **Ação:** Usuário realiza login com sucesso.<br><br>**Resultado esperado:** Sessão é mantida ativa. | **Ação:** Sessão expira.<br><br>**Resultado esperado:** Usuário é redirecionado para login. |
| **#04** | **Ação:** Usuário acessa listagem de usuários.<br><br>**Resultado esperado:** Lista é exibida corretamente. | **Ação:** Não há usuários cadastrados.<br><br>**Resultado esperado:** Sistema informa ausência de dados. |
| **#05** | **Ação:** Usuário cadastra novo usuário.<br><br>**Resultado esperado:** Dados são salvos corretamente. | **Ação:** Usuário envia dados inválidos.<br><br>**Resultado esperado:** Sistema bloqueia e informa erro. |
| **#06** | **Ação:** Sistema exibe mensagem de sucesso após operação.<br><br>**Resultado esperado:** Feedback é claro ao usuário. | **Ação:** Ocorre erro na operação.<br><br>**Resultado esperado:** Sistema exibe mensagem de erro. |
| **#07** | **Ação:** Sistema valida regra antes da execução.<br><br>**Resultado esperado:** Regra válida é aceita. | **Ação:** Regra inválida é enviada.<br><br>**Resultado esperado:** Sistema bloqueia execução. |
| **#08** | **Ação:** Frontend envia login ao backend.<br><br>**Resultado esperado:** Backend retorna autenticação válida. | **Ação:** Backend indisponível.<br><br>**Resultado esperado:** Sistema informa erro. |
| **#09** | **Ação:** Usuário realiza login com credenciais válidas.<br><br>**Resultado esperado:** Sistema autentica corretamente. | **Ação:** Credenciais inválidas.<br><br>**Resultado esperado:** Acesso negado. |
| **#10** | **Ação:** Sistema gera token após login.<br><br>**Resultado esperado:** Token válido é retornado. | **Ação:** Falha na geração.<br><br>**Resultado esperado:** Sistema retorna erro. |
| **#11** | **Ação:** Usuário acessa rota protegida com token válido.<br><br>**Resultado esperado:** Acesso permitido. | **Ação:** Acesso sem token.<br><br>**Resultado esperado:** Acesso negado. |
| **#12** | **Ação:** Usuário executa operação CRUD.<br><br>**Resultado esperado:** Operação concluída com sucesso. | **Ação:** Operação inválida.<br><br>**Resultado esperado:** Sistema retorna erro. |
| **#13** | **Ação:** Usuário admin acessa funcionalidade restrita.<br><br>**Resultado esperado:** Acesso permitido. | **Ação:** Usuário padrão tenta acessar.<br><br>**Resultado esperado:** Acesso negado. |
| **#14** | **Ação:** Usuário acessa rota protegida.<br><br>**Resultado esperado:** Sistema valida autorização. | **Ação:** Tentativa de acesso indevido.<br><br>**Resultado esperado:** Bloqueio do acesso. |
| **#15** | **Ação:** Sistema registra operação realizada.<br><br>**Resultado esperado:** Log armazenado corretamente. | **Ação:** Falha ao registrar log.<br><br>**Resultado esperado:** Sistema registra erro interno. |
| **#16** | **Ação:** Sistema trata erro inesperado.<br><br>**Resultado esperado:** Retorna mensagem controlada. | **Ação:** Erro não tratado ocorre.<br><br>**Resultado esperado:** Sistema não quebra. |
| **#17** | **Ação:** Usuário navega em lista paginada.<br><br>**Resultado esperado:** Dados são carregados por página. | **Ação:** Página inválida é solicitada.<br><br>**Resultado esperado:** Sistema retorna erro controlado. |
| **#18** | **Ação:** Agente gera regra com maior precisão.<br><br>**Resultado esperado:** Resultado mais assertivo. | **Ação:** Input ambíguo.<br><br>**Resultado esperado:** Sistema solicita ajuste. |
| **#19** | **Ação:** Agente falha durante execução.<br><br>**Resultado esperado:** Sistema ativa fallback. | **Ação:** Fallback falha.<br><br>**Resultado esperado:** Sistema informa erro. |
| **#20** | **Ação:** Sistema exibe tokens utilizados.<br><br>**Resultado esperado:** Informação visível ao usuário. | **Ação:** Falha na coleta.<br><br>**Resultado esperado:** Sistema não quebra fluxo. |
| **#21** | **Ação:** PR é submetido.<br><br>**Resultado esperado:** Revisado e aprovado. | **Ação:** PR com erro.<br><br>**Resultado esperado:** Rejeitado até correção. |

<br>
<a href="../README.md">
  <button>⬅️ Voltar ao README</button>
</a>
