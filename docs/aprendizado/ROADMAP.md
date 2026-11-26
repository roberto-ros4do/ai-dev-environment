# Roadmap — AI Dev Environment

> Jornada prática de aprendizado em AI Engineering por meio da evolução de um ambiente profissional de desenvolvimento de software assistido por IA.

Este documento é a **fonte oficial do planejamento** da jornada. O estado do conhecimento fica em [`ESTADO_APRENDIZADO.md`](ESTADO_APRENDIZADO.md) e o histórico cronológico em [`DIARIO.md`](DIARIO.md).

## Objetivo

Aprender e aplicar conceitos de AI Engineering enquanto aprimoro progressivamente meu fluxo de desenvolvimento com inteligência artificial.

O foco é investigar problemas reais, compreender as tecnologias envolvidas, experimentar soluções e documentar os aprendizados.

A jornada tem dois objetivos complementares:

1. **Evolução do ambiente profissional** de desenvolvimento assistido por IA — o projeto profissional é o laboratório prático prioritário.
2. **Aprendizado dos fundamentos** de AI Engineering e engenharia de software — compreender o motivo de cada decisão, e não apenas reproduzir implementações.

**Princípio central:** compreender, planejar e validar antes de modificar.

---

## Situação atual

| Item | Situação |
|---|---|
| Etapa atual | **Etapa 1 — Context Engineering** (em andamento) |
| Etapas concluídas | Etapa 0 — Diagnóstico e linha de base |
| Próximo objetivo | Analisar a versão revisada do `architecture.md` do projeto profissional |

Última revisão deste roadmap: 2026-11-24.

## Legenda

- `[x]` concluído.
- `[~]` em andamento ou parcialmente realizado.
- `[ ]` não iniciado.

Status de etapa: **Planejada**, **Em andamento** ou **Concluída**.

## Regras para mudança de etapa

- Uma etapa só é concluída quando seus objetivos e critérios de conclusão forem atendidos — não porque seus assuntos foram apresentados.
- Marcar uma atividade como concluída exige que ela tenha sido efetivamente realizada.
- Atividades de uma etapa futura podem ser antecipadas quando houver necessidade real, sem que isso conclua a etapa.

---

## Contexto inicial

> Registro do momento em que a jornada foi planejada (novembro de 2026). Não representa garantia do estado atual do ambiente profissional.

O ambiente de desenvolvimento utiliza:

- **Editor:** Visual Studio Code.
- **Assistente de IA:** Claude, inicialmente utilizado por meio de chat com acesso ao projeto.
- **Tecnologias do sistema:** PHP, JavaScript e MySQL.
- **Execução:** ambiente local.
- **Testes:** predominantemente manuais, com auditorias orientadas por cenários e perfis de usuários.

O sistema profissional está na fase final de preparação para produção, após um processo de refatoração e auditoria.

A prioridade é concluir as atividades pendentes antes de realizar mudanças significativas no ambiente de desenvolvimento.

## Trilha paralela — React e TypeScript

O estudo de React e TypeScript continua em paralelo e **não é substituído** por esta jornada. Ele não está detalhado neste roadmap.

---

## Etapa 0 — Diagnóstico e linha de base

**Status:** Concluída.

**Objetivo:** compreender o funcionamento atual do ambiente e identificar oportunidades de melhoria sem alterar o projeto.

### Atividades

- [x] Confirmar o modo de integração do Claude e as ferramentas disponíveis.
- [x] Mapear a estrutura geral do projeto e suas principais responsabilidades.
- [x] Identificar comandos, ferramentas, Git, banco de dados e ambientes.
- [x] Documentar o fluxo atual de implementação de funcionalidades.
- [x] Documentar o fluxo atual de auditoria e testes.
- [x] Analisar os resultados da auditoria em andamento.
- [x] Identificar dificuldades recorrentes e oportunidades de automação.
- [x] Definir limites de acesso, segurança e aprovação.
- [x] Estabelecer indicadores iniciais para futuras comparações.

### Decisões registradas

- A evolução começa pela organização do contexto, antes da migração efetiva para Claude Code.
- O projeto profissional é o laboratório prático.
- A migração para Claude Code será gradual, sem comprometer entregas e estabilidade.
- O levantamento arquitetural foi inicial e parcial, não uma auditoria completa: informações que embasem decisões devem ser confirmadas no código.

### Resultado esperado

Um diagnóstico do ambiente atual, contendo pontos fortes, limitações, oportunidades de melhoria e uma linha de base para avaliar a evolução.

---

## Etapa 1 — Context Engineering

**Status:** Em andamento.

**Objetivo:** aprender a organizar e fornecer contexto relevante para que a IA compreenda melhor o projeto e execute tarefas com maior consistência.

### Conceitos

- Context Engineering.
- Instruções persistentes.
- Organização e recuperação de contexto.
- Gerenciamento da janela de contexto.
- Documentação modular.
- Boas práticas de utilização do `CLAUDE.md`.
- Progressive Disclosure.
- Separação entre instruções, contexto e conhecimento especializado.

### Atividades

- [~] Estudar os fundamentos de Context Engineering. — trabalhados: instruções permanentes × documentação especializada, `CLAUDE.md` como ponto de entrada, Progressive Disclosure, documentação arquitetural. Ainda não abordados: gerenciamento da janela de contexto, organização e recuperação de contexto.
- [ ] Investigar como o Claude utiliza o contexto do projeto.
- [x] Avaliar a organização atual das informações fornecidas à IA.
- [x] Planejar um `CLAUDE.md` como ponto de entrada para instruções persistentes. — seções iniciais implementadas no projeto profissional (fluxo de desenvolvimento, operações sensíveis, preservação da arquitetura, arquitetura e padrões); ainda não validadas no Claude Code.
- [~] Propor documentação modular para arquitetura, convenções, autorização e testes. — estrutura proposta; `architecture.md` com primeira versão revisada conceitualmente e **versão revisada aguardando análise**; demais documentos não iniciados.
- [~] Validar manualmente as informações antes de transformá-las em instruções permanentes. — em curso pela revisão do `architecture.md`.
- [ ] Implementar a estrutura aprovada em momento apropriado.
- [ ] Organizar referências entre o `CLAUDE.md` e os documentos especializados.
- [ ] Avaliar os resultados em tarefas reais e comparar com o fluxo anterior.
- [ ] Identificar informações redundantes, desatualizadas ou desnecessárias.
- [ ] Aprender estratégias para reduzir o consumo desnecessário da janela de contexto.
- [ ] Validar o uso do `CLAUDE.md` no Claude Code.

### Estrutura proposta para avaliação

```text
CLAUDE.md
docs/
└── ai/
    ├── architecture.md
    ├── conventions.md
    ├── authorization.md
    └── testing.md
```

Essa estrutura é uma proposta inicial, não uma decisão definitiva. Novos documentos poderão ser adicionados quando houver necessidade real de separar conhecimentos específicos (por exemplo, um documento de banco de dados e relacionamentos, citado nos registros históricos).

### Claude Code

A migração para Claude Code será avaliada após a conclusão e estabilização das atividades prioritárias do MVP.

A migração não é um pré-requisito para estudar Context Engineering.

### Resultado esperado

Uma estratégia de gerenciamento de contexto validada, documentada e testada, capaz de reduzir instruções repetitivas e melhorar a consistência do trabalho com IA.

---

## Etapa 2 — Skills e workflows reutilizáveis

**Status:** Planejada.

**Objetivo:** transformar processos repetitivos de desenvolvimento em fluxos estruturados, previsíveis e reutilizáveis.

### Conceitos

- Skills.
- Workflows.
- Instruções reutilizáveis.
- Separação de responsabilidades.
- Revisão humana.
- Padronização de processos.
- Composição de ferramentas e instruções.
- Contexto específico por tarefa.

### Atividades

- [ ] Estudar o funcionamento de skills e workflows.
- [ ] Mapear o processo atual de implementação de funcionalidades.
- [ ] Estruturar um workflow de implementação.
- [ ] Estruturar um workflow de auditoria por perfil de usuário.
- [ ] Criar uma estratégia de revisão de código e diffs.
- [ ] Definir pontos de aprovação humana.
- [ ] Experimentar a criação de uma skill para um processo recorrente.
- [ ] Avaliar quando utilizar uma skill e quando uma instrução simples é suficiente.
- [ ] Testar os workflows em tarefas controladas.
- [ ] Registrar limitações, resultados e oportunidades de melhoria.
- [ ] Reutilizar e aprimorar os workflows conforme novas necessidades surgirem.

### Workflows inicialmente planejados

**Workflow de implementação**

1. Compreender os requisitos e critérios de aceitação.
2. Explorar o código existente.
3. Identificar padrões e dependências.
4. Elaborar um plano de implementação.
5. Apresentar o plano para aprovação.
6. Implementar a alteração aprovada.
7. Executar testes e verificações.
8. Revisar o diff.
9. Documentar o resultado.

**Workflow de auditoria**

1. Selecionar o perfil de usuário.
2. Acessar o menu correspondente.
3. Verificar a visibilidade das funcionalidades.
4. Avaliar listagens e vínculos.
5. Testar cadastros, edições e exclusões.
6. Testar o acesso direto aos endpoints.
7. Verificar tentativas de acesso não autorizado.
8. Registrar evidências e resultados.

### Limites de atuação

- Não modificar o esquema do banco de dados sem aprovação.
- Não alterar dados reais ou executar operações destrutivas sem autorização.
- Não introduzir dependências sem justificativa e aprovação.
- Manter a revisão humana nas alterações relevantes.

### Resultado esperado

Um conjunto inicial de skills e workflows reutilizáveis, capaz de padronizar processos recorrentes e reduzir a necessidade de repetir instruções extensas.

---

## Etapa 3 — Testes e automação

**Status:** Planejada.

**Objetivo:** evoluir progressivamente as verificações manuais para processos automatizados e reproduzíveis, aumentando a confiabilidade das alterações realizadas com IA.

### Conceitos

- Testes unitários.
- Testes de integração.
- Testes end-to-end.
- Automação de testes.
- Playwright.
- Hooks.
- Lint e análise estática.
- Ambientes isolados.
- Evidências e cobertura de testes.

### Atividades

- [ ] Analisar as possibilidades de testes automatizados no projeto.
- [ ] Identificar funções e regras de negócio que possam ser testadas isoladamente.
- [ ] Mapear dependências externas que precisam ser isoladas nos testes.
- [ ] Introduzir testes unitários para lógicas isoladas.
- [ ] Planejar testes de integração para banco de dados, APIs, permissões e vínculos.
- [ ] Garantir que endpoints sejam testados diretamente, não apenas pela interface.
- [ ] Avaliar a utilização do Playwright para automatizar fluxos da interface.
- [ ] Preparar um ambiente local isolado com dados fictícios.
- [ ] Estruturar cenários de testes por perfil de usuário.
- [ ] Avaliar a utilização de hooks para executar verificações automaticamente.
- [ ] Integrar comandos confiáveis de lint e testes ao fluxo de desenvolvimento.
- [ ] Registrar resultados, evidências, falhas e cobertura dos testes.
- [ ] Comparar a confiabilidade do processo automatizado com as auditorias manuais.

### Estratégia de evolução

A automação será introduzida gradualmente:

1. Começar por testes simples e previsíveis.
2. Priorizar funções isoladas e regras de negócio.
3. Evoluir para testes de integração.
4. Automatizar fluxos de interface com Playwright.
5. Introduzir hooks somente quando os comandos executados forem confiáveis.
6. Ampliar a cobertura conforme os resultados demonstrarem necessidade.

### Cuidados

- Não executar testes destrutivos em produção.
- Utilizar dados fictícios e ambientes isolados.
- Não confundir navegação automatizada com garantia de segurança.
- Validar permissões no backend, independentemente do comportamento da interface.
- Evitar hooks que executem ações destrutivas ou difíceis de reverter.

### Resultado esperado

Uma estratégia de testes progressivamente automatizada, com cenários reproduzíveis, evidências verificáveis e maior segurança nas alterações realizadas com IA.

---

## Etapa 4 — MCP, ferramentas e agentes

**Status:** Planejada.

**Objetivo:** compreender como ampliar as capacidades da IA por meio da integração com ferramentas externas, protocolos de comunicação e agentes especializados.

### Conceitos

- Model Context Protocol (MCP).
- Servidores e clientes MCP.
- Tool Calling.
- Integração com ferramentas externas.
- Permissões e escopos de ferramentas.
- Agentes especializados.
- Delegação de tarefas.
- Coordenação entre agentes.
- RAG e recuperação de informações.

### Atividades

- [ ] Avaliar a utilização do Claude Code CLI ou de uma integração compatível.
- [ ] Compreender como o Claude Code interage com arquivos, terminal e ferramentas.
- [ ] Estudar a arquitetura do Model Context Protocol.
- [ ] Investigar como servidores MCP disponibilizam ferramentas e recursos.
- [ ] Inspecionar o funcionamento do Playwright MCP.
- [ ] Experimentar ferramentas MCP em tarefas controladas.
- [ ] Avaliar a criação de um servidor MCP próprio, inicialmente somente leitura.
- [ ] Definir permissões e limites de acesso para ferramentas externas.
- [ ] Investigar o funcionamento de agentes especializados.
- [ ] Avaliar a separação de tarefas entre agentes de implementação, revisão e testes.
- [ ] Comparar o uso de agentes com workflows mais simples.
- [ ] Investigar RAG quando a quantidade ou dispersão da documentação justificar recuperação semântica.
- [ ] Registrar os benefícios, limitações, custos e riscos das integrações experimentadas.

### Critérios para adoção

Nem toda tecnologia precisa ser incorporada ao ambiente.

A decisão de utilizar MCP, agentes ou RAG deve considerar:

- Problema concreto que a tecnologia resolve.
- Ganho em relação ao processo atual.
- Complexidade adicional introduzida.
- Custos de execução e manutenção.
- Segurança e permissões necessárias.
- Possibilidade de validar os resultados.

### Resultado esperado

Compreender e experimentar integrações com ferramentas externas e agentes, adotando somente aquelas que apresentarem benefícios concretos para o ambiente de desenvolvimento.

---

## Primeiro ciclo de 7 dias

Este ciclo serve como referência para colocar os primeiros aprendizados em prática após a aprovação do planejamento.

Ele não representa um prazo obrigatório para concluir as etapas.

1. **Dia 1:** inventário de arquitetura, regras e dependências, somente leitura.
2. **Dia 2:** proposta de `CLAUDE.md` e documentação especializada, sem criação automática.
3. **Dia 3:** revisão humana e validação dos padrões identificados.
4. **Dia 4:** criação do primeiro workflow reutilizável de implementação.
5. **Dia 5:** elaboração de uma matriz de auditoria por perfil e vínculos.
6. **Dia 6:** definição de comandos de teste e plano de automação segura.
7. **Dia 7:** execução de uma tarefa pequena e comparação com o fluxo anterior.

O ciclo poderá ser adaptado conforme o andamento do projeto e os resultados observados.

---

## Indicadores e avaliação de resultados

**Objetivo:** avaliar se as mudanças realmente melhoram o fluxo de desenvolvimento, em vez de adotar tecnologias apenas por sua novidade.

### Indicadores

- Tempo necessário para concluir tarefas.
- Quantidade de instruções repetidas.
- Frequência de erros encontrados durante revisões.
- Problemas detectados antes do commit.
- Falhas identificadas pelos testes.
- Regressões introduzidas por alterações.
- Reutilização de skills e workflows.
- Necessidade de intervenção humana para corrigir resultados da IA.
- Custos e complexidade das ferramentas utilizadas.

### Critérios de avaliação

Cada melhoria deverá ser avaliada considerando:

1. Qual problema motivou a mudança?
2. Como o processo funcionava anteriormente?
3. Qual solução foi experimentada?
4. Quais resultados foram observados?
5. Quais limitações ou efeitos negativos surgiram?
6. Vale a pena manter a solução?

Os resultados serão registrados no [diário](DIARIO.md).

---

## Segurança e limites de atuação

A evolução do ambiente deverá respeitar os seguintes princípios:

- Preservar dados de alunos, responsáveis e demais informações confidenciais.
- Não enviar credenciais, segredos ou informações sensíveis a modelos.
- Utilizar branches e revisão de diffs antes de alterações relevantes.
- Exigir aprovação explícita para operações críticas.
- Realizar backups quando necessário.
- Evitar testes destrutivos em produção ou sobre dados reais.
- Utilizar ambientes e contas de teste sempre que possível.
- Conceder às ferramentas somente as permissões necessárias.
- Não executar migrações, alterações de dados ou operações externas sem autorização.
- Registrar decisões relevantes e resultados das experimentações.

---

## Diretrizes da jornada

- Aprender os fundamentos antes de depender de ferramentas.
- Priorizar problemas reais do ambiente profissional.
- Experimentar uma tecnologia por vez sempre que possível.
- Não adotar ferramentas apenas por estarem em evidência.
- Validar manualmente informações antes de transformá-las em instruções permanentes.
- Diferenciar fatos confirmados, hipóteses e decisões.
- Documentar tanto os resultados positivos quanto os negativos.
- Preservar a estabilidade e a segurança do projeto profissional.
- Evoluir gradualmente, sem antecipar etapas desnecessariamente.

---

## Como retomar

Mensagem sugerida:

> Vamos continuar o projeto AI Dev Environment, seguindo o roadmap e o diário de aprendizado.
>
> Identifique a etapa atual, considere os conhecimentos e as atividades já realizadas e continue de forma didática.
>
> Explique os conceitos antes de propor desafios práticos. Não invente conhecimentos ou experiências que ainda não foram demonstrados.
>
> Priorize problemas reais do ambiente profissional, proponha antes de alterar e respeite os limites de segurança e aprovação.

---

## Escopo futuro

O projeto pessoal de desenvolvimento não integra este acompanhamento.

O conhecimento adquirido durante a evolução do ambiente profissional poderá ser aplicado posteriormente em projetos pessoais, conforme fizer sentido.

---

## Assuntos do universo planejado ainda sem posição definida

Fundamentos de LLMs, structured outputs e avaliações (evals) fazem parte do universo de estudos da jornada, mas ainda não têm posição definida neste roadmap.

---

**Este roadmap é um documento vivo.** As etapas, atividades e prioridades poderão ser atualizadas conforme os aprendizados, necessidades e resultados observados durante a jornada.

## Histórico de alterações do roadmap

| Data | Alteração | Origem |
|---|---|---|
| 2026-11-14 | Versão inicial (Etapas 0–6 e princípios) | commit `7891c25` |
| 2026-11-15 | Alinhamento com o plano de avanço; versão commitada cortada no meio da Etapa 2 | commit `7b91046` |
| 2026-11-24 | Movido para `docs/aprendizado/`; Etapa 0 concluída; Etapas 1–3 revisadas; Etapa 4 reúne MCP, ferramentas, agentes e RAG; antigas Etapas 5–7 substituídas; adicionados primeiro ciclo de 7 dias, indicadores, segurança, diretrizes, como retomar e escopo futuro | não commitado |
