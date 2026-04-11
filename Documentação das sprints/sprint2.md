## 📥 Definition of Ready (DoR)
### Sprint 2
Uma User Story só poderá entrar na Sprint 2 se:
- Atender todos os critérios do DoR da Sprint 1
- Estiver relacionada à avaliação, histórico ou versionamento
- Depender de funcionalidades já implementadas na Sprint 1
- Possuir fluxo de uso claramente definido
- Estiver refinada e compreendida pelo time

## ✅ Definition of Done (DoD)
### Sprint 2
Uma User Story será considerada concluída quando:
- Funcionalidades de avaliação, histórico ou versionamento estiverem implementadas
- O histórico de alterações estiver sendo registrado corretamente
- A restauração de versões funcionar sem inconsistências
- As avaliações de resposta forem armazenadas corretamente
- Não houver erros críticos
- Estiver testada e validada
  
---

## 📋 Backlog da Sprint 2

| RANK | TIPO | ITEM | STATUS |
| :--: | :-- | :-- | :--: |
|#1|Frontend| Input para usuário dar um nome a regra |🕓|
|#2|Frontend| Tela para visualização de funcionários, comissões, marcas |🕓|
|#3|Frontend| Listagem de funcionários, comissões, marcas e lojas de acordo com os dados do excel fornecidos|🕓|
|#4|Frontend| Botão para para cálculo de comissão por marca, loja e funcionário |🕓|
|#5|Frontend| Card para exibir resultado do cálculo de comissão |🕓|
|#6|Frontend| Exibir regras de negócio atreladas a um funcionário, marca ou loja ao calcular o comissioanamento |🕓|
|#7|Back/Front| Integração entre frontend e backend |🕓|
|#8|Backend| Criar classe Comissão e Cargo|🕓|
|#9|Backend| MVC Funcionário |🕓|
|#10|Backend| MVC Loja |🕓|
|#11|Backend| MVC Marcas |🕓|
|#12|Backend| MVC Regras de negócio |🕓|
|#13|Backend| Rota para calcular comissão |🕓|
|#14|ML/IA| Criar workflow com langgraph permitindo criar um agente com padrão ReAct, o agente deve seguir o seguinte fluxo: start -> agent <-> contexto -> code_generator -> code_review -> end |🕓|
|#15|ML/IA| Criar rota para direcionar input do usuário para o agente  |🕓|
|#16|ML/IA| Criar rota para realizar o cálculo do comissionamento |🕓|
|#17|ML/IA| Gerar objeto da regra de negócio solicitada pelo usuário |🕓|
|#18|ML/IA| Método para validação da regra de negócio gerada (pandas ou texto) |🕓|
|#19|ML/IA| Revisão de código gerado antes da geração do objeto |🕓|
|#20|ML/IA| Aplicar observabilidade do agente para controlar latência de resposta, quantidade de tokens, versionamento de prompts, qualidade da resposta |🕓|
|#21|Scrum Master| Aceitar pull requests e realizar merge |🕓|

## ✅ Critérios de Aceitação da Sprint 2

| RANK | ITEM | STATUS |
| :--: | :-- | :--: |
|#1|O sistema deve permitir ao usuário inserir e salvar um nome válido para a regra de negócio.|🕓|
|#2|O sistema deve exibir uma tela com visualização organizada de funcionários, comissões e marcas.|🕓|
|#3|O sistema deve listar corretamente funcionários, comissões, marcas e lojas com base nos dados do Excel fornecido.|🕓|
|#4|O sistema deve permitir acionar o cálculo de comissão por meio de um botão funcional na interface.|🕓|
|#5|O sistema deve exibir o resultado do cálculo de comissão em formato de card visual.|🕓|
|#6|O sistema deve apresentar as regras de negócio aplicadas ao cálculo conforme funcionário, marca ou loja.|🕓|
|#7|O frontend e backend devem estar integrados garantindo comunicação consistente via API.|🕓|
|#8|O sistema deve possuir uma classe Comissão com a comissão de cada cargo e uma classe Cargo, com os tipos de cargo.|🕓|
|#9|O sistema deve implementar a vizualização para a entidade Funcionário.|🕓|
|#10|O sistema deve implementar a vizualização para a entidade Loja.|🕓|
|#11|O sistema deve implementar a vizualização para a entidade Marca.|🕓|
|#12|O sistema deve implementar operações de CRUD para regras de negócio.|🕓|
|#13|O sistema deve disponibilizar uma rota que realize o cálculo de comissão com base nos parâmetros informados.|🕓|
|#14|O sistema deve implementar um workflow com LangGraph seguindo o padrão ReAct definido.|🕓|
|#15|O sistema deve disponibilizar uma rota que receba o input do usuário e direcione ao agente de IA.|🕓|
|#16|O sistema deve disponibilizar uma rota para cálculo de comissionamento utilizando IA.|🕓|
|#17|O sistema deve gerar automaticamente um objeto de regra de negócio a partir do input do usuário.|🕓|
|#18|O sistema deve validar a regra de negócio gerada antes de sua execução.|🕓|
|#19|O sistema deve revisar o código gerado pelo agente antes de transformá-lo em regra válida.|🕓|
|#20|O sistema deve implementar observabilidade do agente incluindo métricas de latência, tokens e qualidade.|🕓|
|#21|Os pull requests devem ser revisados, aprovados e integrados corretamente à branch principal.|🕓|

## 🎯 Cenários de Teste da Sprint 2

| US | Cenário de Teste 1 | Cenário de Teste 2 |
|----|------------------|--------------------|
| **#01** | **Ação:** Usuário insere um nome válido para a regra de negócio e salva.<br><br>**Resultado esperado:** Sistema salva o nome corretamente e permite prosseguir com a criação da regra. | **Ação:** Usuário tenta salvar a regra sem preencher o nome.<br><br>**Resultado esperado:** Sistema exibe mensagem de erro informando que o nome é obrigatório. |
| **#02** | **Ação:** Usuário acessa a tela de visualização de funcionários, comissões e marcas.<br><br>**Resultado esperado:** Sistema exibe os dados organizados corretamente na interface. | **Ação:** Usuário acessa a tela sem dados disponíveis.<br><br>**Resultado esperado:** Sistema exibe mensagem informando ausência de dados. |
| **#03** | **Ação:** Sistema carrega os dados a partir do Excel fornecido.<br><br>**Resultado esperado:** Dados são exibidos corretamente na listagem (funcionários, comissões, marcas e lojas). | **Ação:** Sistema tenta carregar um arquivo Excel inválido ou corrompido.<br><br>**Resultado esperado:** Sistema exibe erro de leitura e não apresenta dados inconsistentes. |
| **#04** | **Ação:** Usuário clica no botão de calcular comissão.<br><br>**Resultado esperado:** Sistema executa o cálculo e inicia o processamento. | **Ação:** Usuário clica múltiplas vezes rapidamente no botão.<br><br>**Resultado esperado:** Sistema evita múltiplas execuções simultâneas. |
| **#05** | **Ação:** Após cálculo, sistema exibe o resultado no card.<br><br>**Resultado esperado:** Card apresenta valor da comissão e contexto corretamente. | **Ação:** Novo cálculo é realizado.<br><br>**Resultado esperado:** Card é atualizado com os novos dados. |
| **#06** | **Ação:** Usuário realiza cálculo de comissão para um funcionário específico.<br><br>**Resultado esperado:** Sistema exibe as regras de negócio aplicadas ao cálculo. | **Ação:** Usuário realiza cálculo sem regras cadastradas.<br><br>**Resultado esperado:** Sistema informa que não há regras aplicáveis. |
| **#07** | **Ação:** Frontend envia requisição ao backend para cálculo.<br><br>**Resultado esperado:** Backend processa e retorna resposta válida. | **Ação:** Backend está indisponível.<br><br>**Resultado esperado:** Frontend exibe mensagem de erro amigável ao usuário. |
| **#08** | **Ação:** Sistema instancia a classe Comissão associada a um Cargo.<br><br>**Resultado esperado:** Comissão é calculada corretamente conforme o tipo de cargo definido. | **Ação:** Sistema tenta calcular comissão para um cargo inexistente.<br><br>**Resultado esperado:** Sistema retorna erro informando que o cargo é inválido ou não encontrado. |
| **#09** | **Ação:** Usuário acessa a visualização de Funcionários.<br><br>**Resultado esperado:** Sistema exibe a lista de funcionários com seus dados corretamente. | **Ação:** Usuário acessa a visualização sem funcionários cadastrados.<br><br>**Resultado esperado:** Sistema exibe mensagem informando ausência de registros. |
| **#10** | **Ação:** Usuário acessa a visualização de Lojas.<br><br>**Resultado esperado:** Sistema exibe a lista de lojas cadastradas corretamente. | **Ação:** Usuário acessa a visualização sem lojas cadastradas.<br><br>**Resultado esperado:** Sistema exibe mensagem informando ausência de registros. |
| **#11** | **Ação:** Usuário acessa a visualização de Marcas.<br><br>**Resultado esperado:** Sistema exibe a lista de marcas cadastradas corretamente. | **Ação:** Usuário acessa a visualização sem marcas cadastradas.<br><br>**Resultado esperado:** Sistema exibe mensagem informando ausência de registros. |
| **#12** | **Ação:** Usuário cria uma nova regra de negócio.<br><br>**Resultado esperado:** Regra é salva e associada corretamente. | **Ação:** Usuário tenta criar regra inválida.<br><br>**Resultado esperado:** Sistema retorna erro de validação. |
| **#13** | **Ação:** Sistema recebe requisição na rota de cálculo.<br><br>**Resultado esperado:** Retorna valor de comissão calculado corretamente. | **Ação:** Requisição com parâmetros inválidos é enviada.<br><br>**Resultado esperado:** Sistema retorna erro informativo. |
| **#14** | **Ação:** Agente executa workflow completo no LangGraph.<br><br>**Resultado esperado:** Fluxo é concluído sem falhas. | **Ação:** Falha ocorre em uma etapa do fluxo.<br><br>**Resultado esperado:** Sistema registra erro e interrompe execução. |
| **#15** | **Ação:** Usuário envia input textual para o agente.<br><br>**Resultado esperado:** Sistema processa e retorna resposta estruturada. | **Ação:** Input inválido é enviado.<br><br>**Resultado esperado:** Sistema retorna mensagem de erro. |
| **#16** | **Ação:** Sistema executa cálculo via IA.<br><br>**Resultado esperado:** Resultado é consistente com regras aplicadas. | **Ação:** Falha ocorre no agente.<br><br>**Resultado esperado:** Sistema utiliza fallback ou informa erro. |
| **#17** | **Ação:** Agente gera objeto de regra a partir do input.<br><br>**Resultado esperado:** Objeto válido é criado. | **Ação:** Input ambíguo é fornecido.<br><br>**Resultado esperado:** Sistema solicita ajuste ou rejeita a regra. |
| **#18** | **Ação:** Sistema valida regra antes da execução.<br><br>**Resultado esperado:** Regra válida é aprovada. | **Ação:** Regra inconsistente é validada.<br><br>**Resultado esperado:** Sistema bloqueia execução e informa erro. |
| **#19** | **Ação:** Código gerado pelo agente passa por revisão.<br><br>**Resultado esperado:** Código aprovado segue para execução. | **Ação:** Código contém erro ou risco.<br><br>**Resultado esperado:** Sistema reprova e não executa. |
| **#20** | **Ação:** Sistema registra métricas do agente durante execução.<br><br>**Resultado esperado:** Dados de latência, tokens e qualidade são armazenados. | **Ação:** Falha na coleta de métricas.<br><br>**Resultado esperado:** Sistema registra erro sem impactar execução principal. |
| **#21** | **Ação:** Desenvolvedor abre pull request.<br><br>**Resultado esperado:** PR é revisado e aprovado. | **Ação:** PR contém conflitos ou falhas.<br><br>**Resultado esperado:** PR não é aprovado até correção. |

<br>
<a href="../README.md">
  <button>⬅️ Voltar ao README</button>
</a>
