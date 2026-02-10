# Comparação de arquiteturas

Esta seção apresenta uma comparação conceitual entre dois modelos de construção de agentes:

1. Agente generalista exposto a ambientes públicos
2. Agente contextualizado e governável

A comparação é baseada em padrões de engenharia de sistemas agentic e no estudo de caso apresentado neste repositório.

## Visão geral

| Característica | Agente generalista exposto | Agente contextualizado (modelo Vânia) |
|----------------|-----------------------------|----------------------------------------|
| Modelo base | LLM generalista | LLM generalista |
| Contexto de domínio | Ausente ou genérico | Explícito e delimitado |
| Regras de comportamento | Fracas ou inexistentes | Definidas por arquitetura |
| Identidade institucional | Inexistente ou difusa | Clara e consistente |
| Limites operacionais | Amplos ou indefinidos | Claros e controlados |
| Previsibilidade | Baixa | Alta |
| Risco de exposição pública | Alto | Reduzido |
| Governança | Reativa ou inexistente | Estrutural |

## Arquitetura conceitual — agente generalista

Usuário / Ambiente → Agente autônomo → LLM generalista → Ferramentas e APIs → Ações e publicações

Características:

- O LLM opera sem limites claros de domínio
- O agente responde a qualquer estímulo
- Não há uma camada explícita de governança contextual
- O comportamento depende apenas do modelo e do histórico

## Arquitetura conceitual — agente contextualizado

Usuário → Interface de conversa → Camada de contexto e regras → Agente controlado → LLM generalista → Ferramentas autorizadas

Características:

- O contexto define o domínio de atuação
- Regras de comportamento são aplicadas antes da resposta
- O agente possui identidade funcional
- As ações são limitadas a escopos autorizados

## O papel da camada de contexto

A camada de contexto é responsável por:

- Definir o domínio do agente
- Restringir temas e respostas
- Estabelecer regras de conduta
- Controlar ações e integrações
- Garantir identidade institucional

Sem essa camada:

- O agente continua sendo apenas um LLM generalista com acesso a ferramentas

Com essa camada:

- O agente se torna uma entidade funcional, previsível e governável

## Conclusão comparativa

A diferença entre os dois modelos não está no modelo de IA utilizado.

A diferença está na arquitetura que envolve o modelo.

Um agente sem contexto é apenas um modelo generalista com permissões amplas.

Um agente com contexto é um sistema governado, com identidade, domínio e limites operacionais.



