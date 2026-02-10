# Decisões arquiteturais

Este repositório adota algumas decisões de arquitetura fundamentais:

## 1. Separação entre IA e governança
O modelo de linguagem não é responsável por definir seu próprio comportamento.  
A governança é implementada fora do modelo, em uma camada de contexto.

## 2. Domínio explícito
Todo agente deve operar dentro de um escopo definido.  
Agentes sem domínio tendem a comportamento imprevisível.

## 3. Regras antes da resposta
As regras de comportamento devem ser aplicadas antes da geração da resposta, e não como correção posterior.

## 4. Limites operacionais
Integrações e ações devem ser explicitamente autorizadas pela arquitetura.

Essas decisões visam criar agentes previsíveis, auditáveis e alinhados ao domínio de negócio.
