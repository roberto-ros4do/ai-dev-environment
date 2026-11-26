# Estado de aprendizado

> Fotografia atual do conhecimento — **não** é um diário cronológico. É atualizado sempre que há um avanço relevante ou uma nova evidência de aprendizado. O planejamento está em [`ROADMAP.md`](ROADMAP.md); o histórico, em [`DIARIO.md`](DIARIO.md).

Última atualização: 2026-11-24 — reconstrução inicial a partir dos registros históricos e da confirmação do usuário.

## Como ler este documento

### Estados de conhecimento

| Estado | Significado |
|---|---|
| Não estudado | Ainda não foi abordado. |
| Introduzido | O conceito foi apresentado; não há evidência de compreensão. |
| Compreensão parcial | Entendimento demonstrado, mas com lacunas — ou evidência insuficiente para afirmar mais. |
| Compreensão demonstrada | Respostas e explicações sustentam o entendimento. |
| Aplicação demonstrada | Aplicação prática realizada por mim, com compreensão do que foi feito. |
| Precisa revisar | Dificuldade ou esquecimento identificado. |

**Compreensão conceitual e aplicação prática são avaliadas separadamente.** Código ou documentos escritos pela IA não contam como aplicação minha.

### Origem da evidência

- **Direta:** observada durante as sessões de estudo, com data.
- **Confirmada:** registrada nos relatórios históricos e confirmada por mim em 2026-11-24.
- **Indireta:** registrada apenas nos relatórios históricos.
- **Autodeclarada:** informada por mim, sem avaliação.

### Fontes históricas

- **[H1]** Relatório de atividades e aprendizado — Context Engineering.
- **[H2]** Contexto de continuidade — Jornada de Context Engineering e AI Engineering.

Ambas são resumos da fase em que aprendizado e documentação aconteciam em conversas separadas; não contêm as conversas originais. Não são publicadas neste repositório.

---

## A. Situação atual

- **Etapa atual:** ver [`ROADMAP.md` → Situação atual](ROADMAP.md#situação-atual) (Etapa 1 — Context Engineering).
- **Último assunto estudado:** documentação arquitetural — finalidade do `architecture.md` e sua diferença em relação ao código-fonte.
- **Última implementação:** seções iniciais do `CLAUDE.md` do projeto profissional (fluxo de desenvolvimento, operações sensíveis, preservação da arquitetura, arquitetura e padrões); ainda não validadas no Claude Code.
- **Próxima atividade de aprendizado:** analisar a versão revisada do `architecture.md`.

## Quadro-resumo

| Conceito | Compreensão conceitual | Aplicação prática | Evidência |
|---|---|---|---|
| Instruções permanentes × documentação especializada | Compreensão demonstrada | Em andamento (seções do `CLAUDE.md`, não validadas) | Confirmada |
| `CLAUDE.md` como ponto de entrada do contexto | Compreensão demonstrada | Em andamento (idem) | Confirmada |
| Progressive Disclosure | Compreensão demonstrada | Não iniciada (referências do `CLAUDE.md` pendentes) | Confirmada |
| Documentação arquitetural × reprodução do código-fonte | Compreensão demonstrada | Em andamento (revisão do `architecture.md`) | Confirmada |
| Descrição de responsabilidades e relações entre componentes | Compreensão demonstrada | Em andamento (idem) | Confirmada |
| Organização de documentos especializados | Compreensão parcial | Em andamento (estrutura proposta) | Confirmada (trabalhado) |
| Context Engineering — fundamentos | Compreensão parcial | — | Confirmada (parcial) |
| Documentar a arquitetura existente, não a idealizada | Compreensão parcial | — | Indireta |
| Prompt Engineering | Introduzido | Experiência prática prévia | Autodeclarada |
| Gerenciamento da janela de contexto | Não estudado | — | — |

---

## B. Conhecimentos desenvolvidos

### B1. Instruções permanentes × documentação especializada

- **Estado:** conceitual — Compreensão demonstrada · prática — em andamento · evidência — confirmada.
- **Compreensão:** instruções permanentes (fluxo de trabalho, regras, restrições) ficam no arquivo principal, curtas e objetivas; detalhes específicos (arquitetura, autorização, testes) ficam em documentos especializados consultados quando relevantes [H1 §2–3; H2 §6.3].
- **Entendimento inicial, dúvidas e equívocos:** não registrados nas fontes.
- **Aplicação:** implementei no `CLAUDE.md` do projeto profissional seções de caráter permanente — fluxo de desenvolvimento, análise de padrões antes de implementar, plano antes de editar, preservação da arquitetura, prevenção de refatorações fora do escopo, testes seguros, operações sensíveis [H1 §3]. Ainda não validadas no Claude Code.

### B2. `CLAUDE.md` como ponto de entrada do contexto

- **Estado:** conceitual — Compreensão demonstrada · prática — em andamento · evidência — confirmada.
- **Compreensão:** o `CLAUDE.md` contém as instruções gerais do projeto e orienta o agente sobre onde encontrar o contexto especializado [H1 §6; H2 §6.3].
- **Lacuna conhecida:** como o Claude Code carrega e utiliza o `CLAUDE.md` na prática ainda não foi estudado nem validado.
- **Aplicação:** a mesma de B1; a ligação com os documentos especializados ainda não foi feita.

### B3. Progressive Disclosure

- **Estado:** conceitual — Compreensão demonstrada · prática — não iniciada · evidência — confirmada.
- **Compreensão:** fornecer ao agente o contexto específico conforme a necessidade da tarefa, em vez de concentrar todo o conhecimento em um único documento carregado sempre [H1 §2].
- **Observação histórica:** [H1] registrava o conceito como demonstrado; [H2] registrava apenas que havia sido discutido. A divergência foi resolvida pela confirmação de 2026-11-24.
- **Próxima aplicação:** organizar as referências do `CLAUDE.md` aos documentos especializados.

### B4. Documentação arquitetural × reprodução do código-fonte

- **Estado:** conceitual — Compreensão demonstrada · prática — em andamento · evidência — confirmada.
- **Dúvida inicial:** perguntei se o `architecture.md` deveria explicar, por exemplo, a finalidade de uma função específica — uma dúvida sobre o **nível de detalhe** do documento [H2 §6.4].
- **Esclarecimento:** funções importantes podem ser descritas, mas o foco é explicar responsabilidades, módulos, dependências e fluxos — não reproduzir a implementação [H1 §4; H2 §6.4].
- **Evolução:** confirmei a compreensão e esclareci que a função mencionada era apenas um exemplo [H2 §6.4].
- **Aplicação:** a primeira versão do `architecture.md` foi produzida pela IA e revisada conceitualmente; os ajustes identificados incluíram reduzir duplicação com o futuro documento de autorização, separar problemas técnicos pontuais, evitar estatísticas que envelhecem e diferenciar fatos verificados de inferências [H1 §5]. A versão revisada aguarda análise.

### B5. Descrição de responsabilidades e relações entre componentes

- **Estado:** conceitual — Compreensão demonstrada · prática — em andamento · evidência — confirmada.
- **Compreensão:** a documentação arquitetural descreve o papel de cada módulo e como os componentes se relacionam (organização dos includes, módulos, fluxo de requisições) [H1 §4–5].
- **Aplicação:** será exercitada na análise da versão revisada do `architecture.md`.

---

## C. Conhecimentos em desenvolvimento

### C1. Context Engineering — fundamentos

- **Estado:** Compreensão parcial.
- **Evidência:** identifiquei, a partir da minha própria experiência, que precisava repetir arquitetura, padrões, regras de negócio, estrutura do banco e vínculos em diferentes conversas, e que isso prejudicava a previsibilidade [H2 §3.1]. Compreendi que informações que permanecem relevantes entre tarefas podem ser preservadas em arquivos de contexto [H2 §6.2].
- **Lacunas:** gerenciamento da janela de contexto, organização e recuperação de contexto e como o agente consome o contexto ainda não foram abordados.

### C2. Organização de documentos especializados

- **Estado:** Compreensão parcial · evidência — confirmada como assunto trabalhado.
- **Evidência:** trabalhada a organização de documentos especializados para preservar contexto sem sobrecarregar o arquivo principal, e a separação de responsabilidades entre documentos para reduzir redundância [H1 §6].
- **Para avançar:** aplicar o critério na estrutura real (`architecture.md`, autorização, convenções, testes), decidindo onde cada informação deve ficar.

### C3. Documentar a arquitetura existente, não uma arquitetura idealizada

- **Estado:** Compreensão parcial · evidência — indireta, fonte única [H1 §6].
- **Para avançar:** avaliar durante a análise do `architecture.md` revisado.

### C4. Prompt Engineering

- **Estado:** conceitual — Introduzido · prática — experiência prévia.
- **Experiência prévia:** antes da jornada, eu já elaborava prompts detalhados para desenvolvimento, com requisitos, exceções, fluxos, padrões existentes e desejados, estrutura de banco de dados, requisitos de páginas e cenários positivos e negativos; também usava prompts de auditoria simulando perfis de usuário [H2 §3.1, §6.1].
- **Limitação:** não houve estudo sistemático das técnicas de Prompt Engineering; não há domínio registrado de técnicas específicas (few-shot, Chain of Thought etc.).

### Dificuldades identificadas

Nenhuma registrada nos documentos históricos.

### Assuntos a revisitar

Nenhum no momento.

---

## D. Conhecimentos ainda não estudados

| Conceito | Etapa prevista |
|---|---|
| Gerenciamento da janela de contexto | Etapa 1 |
| Organização e recuperação de contexto | Etapa 1 |
| Funcionamento do Claude Code | Etapa 1 |
| Skills e workflows reutilizáveis | Etapa 2 |
| Testes automatizados, Playwright, lint | Etapa 3 |
| Hooks | Etapa 3 |
| MCP e tool calling | Etapa 4 |
| Agentes e orquestração, controle de autonomia | Etapa 4 e seguintes |
| Embeddings, busca semântica, RAG | A definir no roadmap |
| Fundamentos de LLMs, structured outputs, evals | Sem etapa definida |

## Trilha paralela — React e TypeScript

Em andamento fora deste registro. Nenhuma evidência registrada aqui.

---

## Registro de atualizações

| Data | Alteração |
|---|---|
| 2026-11-24 | Reconstrução inicial a partir de [H1] e [H2]. Avaliações de Context Engineering confirmadas pelo usuário. |
