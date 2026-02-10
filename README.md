# moltbot-vs-contextual-agents

Este repositório apresenta uma análise arquitetural comparativa entre:

- agentes generalistas expostos a ambientes públicos (estudo de caso: Moltbot/Moltbook)
- agentes contextualizados e governáveis (referência: arquitetura aplicada no Chatbot Vânia)

O objetivo não é avaliar pessoas, projetos ou intenções, e sim discutir padrões de engenharia que tornam agentes mais previsíveis, seguros e alinhados ao domínio de negócio.

## Premissas e método

- Não inferimos implementação interna de terceiros.
- A análise se baseia em comportamento observável, riscos típicos de sistemas agentic e boas práticas de arquitetura de contexto e governança.

## O ponto central

O problema raramente é a capacidade do modelo.  
O risco aparece quando um agente é colocado em operação sem:

- contexto de domínio explícito
- regras de comportamento
- limites operacionais e de ação

## Conteúdo

- `moltbot-moltbook-case.md` — fenômeno observado e hipóteses arquiteturais plausíveis
- `architecture-comparison.md` — comparação “agente generalista exposto” vs “agente contextualizado”
- `architecture.md` — camadas, responsabilidades e fluxo
- `context-engineering.md` — como contexto define domínio e comportamento
- `security.md` — riscos típicos e controles recomendados
- `operations.md` — observabilidade, auditoria e fallback humano
- `decisions.md` — decisões arquiteturais e trade-offs
- `limitations.md` — limites desta análise
- `glossary.md` — termos e definições

## Nota sobre código

Este repositório é deliberadamente focado em documentação.  
Quando exemplos forem necessários, serão apresentados como pseudocódigo e diagramas, evitando exposição de implementações proprietárias.
