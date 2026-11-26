# Diário da jornada

> Histórico cronológico da jornada: atividades efetivamente realizadas, conceitos estudados, implementações, testes, decisões, dificuldades e resultados. Não substitui o estado de aprendizado ([`ESTADO_APRENDIZADO.md`](ESTADO_APRENDIZADO.md)) nem o planejamento ([`ROADMAP.md`](ROADMAP.md)).

Entradas em ordem cronológica (a mais antiga primeiro). Cada entrada deixa claro o que foi efetivamente realizado e o que ainda é hipótese ou intenção.

## Modelo de entrada

```markdown
### AAAA-MM-DD — Tema

- **Contexto:** por que estudei ou investiguei isso?
- **O que fiz:** ações realmente executadas (por mim ou pela IA).
- **Conceitos trabalhados:** o que foi estudado (a avaliação da compreensão fica no estado de aprendizado).
- **Decisões:** o que foi decidido e por quê.
- **Dificuldades e dúvidas:** o que não funcionou ou ainda não ficou claro.
- **Resultado:** o que mudou de fato.
- **Próximo passo:** o que pretendo investigar depois.
- **Fontes:** commits ou registros que sustentam a entrada.
```

Tipos de entrada: **registro de sessão** (uma sessão de estudo) e **relatório de período** (consolidação desde o relatório anterior).

## Controle de relatórios

Ponto de partida de cada relatório de período.

| ID | Data | Período analisado (commit base → último commit analisado) | Commit do registro |
|---|---|---|---|
| — | — | Nenhum relatório registrado ainda | — |

> Primeiro relatório: o commit base deve ser confirmado. Candidato: `7b91046`.

---

## Entradas

### Antes da jornada (a partir de julho de 2026) — Ponto de partida

- **Contexto:** comecei no trabalho atual em julho de 2026.
- **Fluxo utilizado:** Claude Desktop com acesso à pasta do projeto profissional; prompts detalhados com requisitos, exceções, fluxos, padrões, banco de dados e cenários de teste; prompts de auditoria simulando perfis de usuário; testes predominantemente manuais.
- **Dificuldade percebida:** precisava repetir manualmente arquitetura, padrões, regras de negócio, estrutura do banco, vínculos e contexto das operações em diferentes conversas, o que prejudicava a previsibilidade e aumentava a supervisão.

### 2026-11-14 — Montagem do repositório

- **O que fiz:** criei o repositório com `README.md`, `ROADMAP.md` (Etapas 0–6 e princípios) e `journal/README.md` (índice e modelo de entrada).
- **Resultado:** repositório em planejamento; nenhuma atividade concluída.
- **Fontes:** commit `7891c25`.

### 2026-11-15 — Alinhamento do roadmap com o plano de avanço

- **O que fiz:** reestruturei o roadmap com o contexto inicial do ambiente, a Etapa 0 detalhada e a Etapa 1 com a estrutura proposta de documentação (`CLAUDE.md` + `docs/ai/`).
- **Observação (2026-11-24):** a versão commitada ficou cortada no meio da Etapa 2.
- **Fontes:** commit `7b91046`.

### Data não registrada — Etapa 0: diagnóstico do ambiente profissional

- **O que fiz:** analisei o fluxo de desenvolvimento com Claude Desktop; fiz um levantamento arquitetural **inicial e parcial** do projeto profissional; identifiquei arquivos sensíveis e operações que exigem autorização explícita.
- **Decisões:** começar a evolução pela organização do contexto, antes da migração efetiva para Claude Code; usar o projeto profissional como laboratório prático; migrar de forma gradual, sem comprometer a estabilidade do MVP.
- **Resultado:** Etapa 0 concluída.

### Data não registrada — Etapa 1: Context Engineering e `CLAUDE.md` do projeto profissional

- **Conceitos trabalhados:** fundamentos de Context Engineering; instruções permanentes × documentação especializada; `CLAUDE.md` como ponto de entrada; Progressive Disclosure; organização de documentos especializados.
- **O que fiz:** defini e implementei no `CLAUDE.md` do projeto profissional seções sobre fluxo de desenvolvimento, análise de padrões antes de implementar, plano antes de editar, preservação da arquitetura, prevenção de refatorações fora do escopo, testes seguros, operações sensíveis, e arquitetura e padrões.
- **Decisão:** manter as instruções permanentes curtas e objetivas, deixando detalhes para documentação complementar.
- **Resultado:** seções iniciais implementadas; `CLAUDE.md` ainda não validado no Claude Code.

### Data não registrada — Documentação arquitetural (`architecture.md`)

- **Conceitos trabalhados:** finalidade da documentação arquitetural; diferença entre documentar a arquitetura e reproduzir o código-fonte; responsabilidades e relações entre componentes.
- **Dúvida:** se o documento deveria explicar a finalidade de uma função. Esclarecido que funções importantes podem ser descritas, com foco em responsabilidades, módulos, dependências e fluxos; a função era apenas um exemplo.
- **O que foi feito:** a IA produziu um primeiro rascunho a partir do levantamento e da conferência do código; o rascunho foi revisado conceitualmente.
- **Ajustes identificados:** reduzir a duplicação de autenticação e autorização; manter limitações arquiteturais relevantes; separar problemas técnicos pontuais; evitar estatísticas que envelhecem; preservar a descrição dos módulos e do fluxo de requisições; diferenciar fatos verificados, inferências e informações não confirmadas.
- **Resultado:** versão revisada solicitada, **aguardando análise e validação**; não integrada ao projeto.

### 2026-11-24 — Organização do acompanhamento da jornada

- **Contexto:** até aqui, o estudo e a documentação aconteciam em conversas separadas. Passei a concentrar os dois no Claude Code.
- **O que foi feito:** a documentação foi reorganizada em `docs/aprendizado/` (roadmap, estado de aprendizado e este diário); o estado de aprendizado foi reconstruído a partir dos registros anteriores; o roadmap foi revisado e as Etapas 2 e 3 detalhadas.
- **Dificuldade:** o roadmap ficou cortado mais de uma vez ao ser salvo (na Etapa 2 em `7b91046`; na Etapa 4 na revisão de 2026-11-24).
- **Resultado:** documentação reorganizada; nenhuma nova evidência de aprendizado nesta sessão.
- **Próximo passo:** completar a Etapa 4 do roadmap; analisar a versão revisada do `architecture.md`.
