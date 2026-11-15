# Roadmap — AI Dev Environment

> Jornada prática de aprendizado em AI Engineering por meio da evolução de um ambiente profissional de desenvolvimento de software assistido por IA.

## Objetivo

Aprender e aplicar conceitos de AI Engineering enquanto aprimoro progressivamente meu fluxo de desenvolvimento com inteligência artificial.

O foco é investigar problemas reais, compreender as tecnologias envolvidas, experimentar soluções e documentar os aprendizados.

Este roadmap representa o planejamento da jornada. As experiências realizadas, dificuldades e descobertas serão registradas no diretório [`journal/`](journal/).

## Contexto inicial

O ambiente de desenvolvimento utiliza:

- **Editor:** Visual Studio Code.
- **Assistente de IA:** Claude, inicialmente utilizado por meio de chat com acesso ao projeto.
- **Tecnologias do sistema:** PHP, JavaScript e MySQL.
- **Execução:** ambiente local.
- **Testes:** predominantemente manuais, com auditorias orientadas por cenários e perfis de usuários.

O sistema profissional está na fase final de preparação para produção, após um processo de refatoração e auditoria.

A prioridade é concluir as atividades pendentes antes de realizar mudanças significativas no ambiente de desenvolvimento.

**Princípio central:** compreender, planejar e validar antes de modificar.

---

## Etapa 0 — Diagnóstico e linha de base

**Objetivo:** compreender o funcionamento atual do ambiente e identificar oportunidades de melhoria sem alterar o projeto.

### Atividades

- [ ] Confirmar o modo de integração do Claude e as ferramentas disponíveis.
- [ ] Mapear a estrutura geral do projeto e suas principais responsabilidades.
- [ ] Identificar comandos, ferramentas, Git, banco de dados e ambientes.
- [ ] Documentar o fluxo atual de implementação de funcionalidades.
- [ ] Documentar o fluxo atual de auditoria e testes.
- [ ] Analisar os resultados da auditoria em andamento.
- [ ] Identificar dificuldades recorrentes e oportunidades de automação.
- [ ] Definir limites de acesso, segurança e aprovação.
- [ ] Estabelecer indicadores iniciais para futuras comparações.

### Resultado esperado

Um diagnóstico do ambiente atual, contendo pontos fortes, limitações, oportunidades de melhoria e uma linha de base para avaliar a evolução.

---

## Etapa 1 — Context Engineering

**Objetivo:** aprender a organizar e fornecer contexto relevante para que a IA compreenda melhor o projeto e execute tarefas com maior consistência.

### Conceitos

- Context Engineering.
- Instruções persistentes.
- Organização e recuperação de contexto.
- Gerenciamento da janela de contexto.
- Documentação modular.
- Boas práticas de utilização do `CLAUDE.md`.

### Atividades

- [ ] Estudar os fundamentos de Context Engineering.
- [ ] Investigar como o Claude utiliza o contexto do projeto.
- [ ] Avaliar a organização atual das informações fornecidas à IA.
- [ ] Planejar um `CLAUDE.md` como ponto de entrada para instruções persistentes.
- [ ] Propor documentação modular para arquitetura, convenções, autorização e testes.
- [ ] Validar manualmente as informações antes de transformá-las em instruções permanentes.
- [ ] Implementar a estrutura aprovada em momento apropriado.
- [ ] Avaliar os resultados em tarefas reais e comparar com o fluxo anterior.

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

Essa estrutura é uma proposta inicial, não uma decisão definitiva.

### Claude Code

A migração para Claude Code será avaliada após a conclusão e estabilização das atividades prioritárias do MVP.

A migração não é um pré-requisito para estudar Context Engineering.

### Resultado esperado

Uma estratégia de gerenciamento de contexto validada, documentada e testada, capaz de reduzir instruções repetitivas e melhorar a consistência do trabalho com IA.

---

## Etapa 2 — Skills e workflows reutilizáveis

**Objetivo:** transformar processos repetitivos de desenvolvimento em fluxos estruturados, previsíveis e reutilizáveis.

### Conceitos

- Skills.
- Workflows.
- Instruções reutilizáveis.
- Separação de responsabilidades.
- Revisão humana.
- Padronização de processos.

### Atividades

- [ ] Estudar o funcionamento de skills e workflows.
- [ ] Mapear o processo atual de implementação de funcionalidades.
- [ ] Estruturar um workflow de implementação.
- [ ] Estruturar um workflow de auditoria por perfil de usuário.
- [ ] Criar uma estratégia de revisão de código e diffs.
- [ ] Definir pontos de aprovação humana.
- [ ] Experiment