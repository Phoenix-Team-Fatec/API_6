## 📋 Backlog da Sprint 3

| RANK | TIPO | ITEM | STATUS |
| :--: | :-- | :-- | :--: |
|#1|Frontend| Tela de login de usuário |🕓|
|#2|Frontend| Validação de campos no login (email/senha) |🕓|
|#3|Frontend| Persistência de sessão do usuário autenticado |🕓|
|#4|Frontend| Tela de gerenciamento de usuários (listagem) |🕓|
|#5|Frontend| Formulário para cadastro e edição de usuários |🕓|
|#6|Frontend| Exibição de mensagens de erro e sucesso (feedback ao usuário) |🕓|
|#7|Back/Front| Integração do fluxo de autenticação entre frontend e backend |🕓|
|#8|Backend| Implementar autenticação (login) com validação de credenciais |🕓|
|#9|Backend| Implementar geração de token (JWT ou similar) |🕓|
|#10|Backend| Implementar middleware de autorização |🕓|
|#11|Backend| CRUD de usuários |🕓|
|#12|Backend| Definição de perfis de acesso (admin, padrão) |🕓|
|#13|Backend| Proteção de rotas sensíveis |🕓|
|#14|Backend| Implementar logs de operações do sistema |🕓|
|#15|Backend| Melhorar tratamento de erros e exceções |🕓|
|#16|Backend| Implementar paginação nas listagens |🕓|
|#17|Backend| Implementar filtros avançados (funcionário, loja, marca) |🕓|
|#18|Backend| Otimizar performance das consultas ao banco |🕓|
|#19|ML/IA| Melhorar precisão do agente na geração de regras de negócio |🕓|
|#20|ML/IA| Implementar fallback para falhas do agente |🕓|
|#21|Scrum Master| Revisar PRs, validar entregas e realizar merge |🕓|

---

## ✅ Critérios de Aceitação da Sprint 3

| RANK | ITEM | STATUS |
| :--: | :-- | :--: |
|#1|O sistema deve exibir uma tela de login funcional para o usuário.|🕓|
|#2|O sistema deve validar corretamente os campos obrigatórios no login.|🕓|
|#3|O sistema deve manter o usuário autenticado durante a sessão.|🕓|
|#4|O sistema deve exibir a listagem de usuários cadastrados.|🕓|
|#5|O sistema deve permitir cadastro e edição de usuários.|🕓|
|#6|O sistema deve exibir mensagens claras de erro e sucesso.|🕓|
|#7|Frontend e backend devem estar integrados no fluxo de autenticação.|🕓|
|#8|O sistema deve validar credenciais corretamente no backend.|🕓|
|#9|O sistema deve gerar token de autenticação válido.|🕓|
|#10|O sistema deve restringir acesso com base em autorização.|🕓|
|#11|O sistema deve permitir CRUD completo de usuários.|🕓|
|#12|O sistema deve diferenciar perfis de usuário.|🕓|
|#13|O sistema deve proteger rotas que exigem autenticação.|🕓|
|#14|O sistema deve registrar logs das operações realizadas.|🕓|
|#15|O sistema deve tratar erros de forma controlada.|🕓|
|#16|O sistema deve implementar paginação nas listagens.|🕓|
|#17|O sistema deve permitir aplicação de filtros nos dados.|🕓|
|#18|O sistema deve apresentar melhoria de performance nas consultas.|🕓|
|#19|O agente de IA deve gerar regras com maior precisão.|🕓|
|#20|O sistema deve tratar falhas do agente com fallback adequado.|🕓|
|#21|Os PRs devem ser revisados e integrados corretamente.|🕓|

---

## 🎯 Cenários de Teste da Sprint 3

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Usuário acessa tela de login.<br><br>**Resultado esperado:** Tela é exibida corretamente. | **Ação:** Tela não carrega.<br><br>**Resultado esperado:** Sistema informa erro ao usuário. |
| **#02** | **Ação:** Usuário preenche login corretamente.<br><br>**Resultado esperado:** Acesso autorizado. | **Ação:** Campos inválidos.<br><br>**Resultado esperado:** Sistema exibe erro de validação. |
| **#03** | **Ação:** Usuário permanece logado.<br><br>**Resultado esperado:** Sessão mantida. | **Ação:** Sessão expira.<br><br>**Resultado esperado:** Sistema solicita novo login. |
| **#04** | **Ação:** Usuário acessa listagem de usuários.<br><br>**Resultado esperado:** Dados exibidos corretamente. | **Ação:** Sem usuários cadastrados.<br><br>**Resultado esperado:** Sistema informa ausência de dados. |
| **#05** | **Ação:** Usuário cadastra novo usuário.<br><br>**Resultado esperado:** Usuário salvo com sucesso. | **Ação:** Dados inválidos.<br><br>**Resultado esperado:** Sistema bloqueia cadastro. |
| **#06** | **Ação:** Sistema exibe mensagem de sucesso.<br><br>**Resultado esperado:** Feedback visível ao usuário. | **Ação:** Ocorre erro.<br><br>**Resultado esperado:** Mensagem clara de erro. |
| **#07** | **Ação:** Frontend envia login ao backend.<br><br>**Resultado esperado:** Backend responde corretamente. | **Ação:** Backend indisponível.<br><br>**Resultado esperado:** Sistema trata erro. |
| **#08** | **Ação:** Usuário realiza login válido.<br><br>**Resultado esperado:** Backend autentica corretamente. | **Ação:** Login inválido.<br><br>**Resultado esperado:** Acesso negado. |
| **#09** | **Ação:** Sistema gera token.<br><br>**Resultado esperado:** Token válido retornado. | **Ação:** Falha na geração.<br><br>**Resultado esperado:** Sistema retorna erro. |
| **#10** | **Ação:** Usuário acessa rota protegida.<br><br>**Resultado esperado:** Acesso permitido com token. | **Ação:** Sem token.<br><br>**Resultado esperado:** Acesso negado. |
| **#11** | **Ação:** CRUD de usuário executado.<br><br>**Resultado esperado:** Operação concluída com sucesso. | **Ação:** Falha na operação.<br><br>**Resultado esperado:** Erro tratado. |
| **#12** | **Ação:** Sistema identifica perfil do usuário.<br><br>**Resultado esperado:** Permissões aplicadas. | **Ação:** Perfil inválido.<br><br>**Resultado esperado:** Acesso bloqueado. |
| **#13** | **Ação:** Usuário tenta acessar rota protegida.<br><br>**Resultado esperado:** Validação aplicada. | **Ação:** Token inválido.<br><br>**Resultado esperado:** Acesso negado. |
| **#14** | **Ação:** Sistema registra log.<br><br>**Resultado esperado:** Log armazenado corretamente. | **Ação:** Falha no log.<br><br>**Resultado esperado:** Sistema continua operação. |
| **#15** | **Ação:** Erro ocorre no sistema.<br><br>**Resultado esperado:** Tratamento adequado. | **Ação:** Erro crítico.<br><br>**Resultado esperado:** Sistema não quebra. |
| **#16** | **Ação:** Listagem com paginação.<br><br>**Resultado esperado:** Dados paginados. | **Ação:** Página inválida.<br><br>**Resultado esperado:** Sistema corrige ou informa erro. |
| **#17** | **Ação:** Usuário aplica filtro.<br><br>**Resultado esperado:** Dados filtrados corretamente. | **Ação:** Filtro inválido.<br><br>**Resultado esperado:** Sistema trata erro. |
| **#18** | **Ação:** Consulta otimizada.<br><br>**Resultado esperado:** Resposta mais rápida. | **Ação:** Alto volume de dados.<br><br>**Resultado esperado:** Sistema mantém performance. |
| **#19** | **Ação:** IA gera regra de negócio.<br><br>**Resultado esperado:** Regra mais precisa. | **Ação:** Input complexo.<br><br>**Resultado esperado:** IA responde corretamente. |
| **#20** | **Ação:** Falha no agente.<br><br>**Resultado esperado:** Sistema usa fallback. | **Ação:** Falha crítica.<br><br>**Resultado esperado:** Sistema informa erro. |
| **#21** | **Ação:** PR criado.<br><br>**Resultado esperado:** Revisado e aprovado. | **Ação:** PR com erro.<br><br>**Resultado esperado:** Correção solicitada. |

<br>
<a href="../README.md">
  <button>⬅️ Voltar ao README</button>
</a>