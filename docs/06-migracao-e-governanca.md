# 6. Migração e governança

[Início](../README.md) | Anterior: [Requisitos](05-requisitos-e-rastreabilidade.md) | Próximo: [Método](07-metodo-e-building-blocks.md)

## Estados de arquitetura

```mermaid
flowchart LR
    A["AS-IS fictício: silos"] --> B["Transição 1: piloto"]
    B --> C["Transição 2: expansão"]
    C --> D["TO-BE evolutivo"]
```

| Estado | Resultado esperado | Evidência para avançar |
|---|---|---|
| AS-IS a confirmar | Inventário de serviços, dados, contratos e controles | Responsáveis e dependências identificados |
| Transição 1 | Cashback para um produto e um parceiro, com adaptador e operação de exceções | Crédito e estorno testados; conciliação comprovada; economia aceita |
| Transição 2 | Outros produtos e parceiros integrados por ondas | Estabilidade, capacidade e controles aceitos |
| Alvo evolutivo | Capacidades reutilizáveis e revisão de duplicações | Equivalência comprovada e decisão de manter ou retirar componentes |

## Coexistência e reversão

Os produtos atuais permanecem como fontes das transações durante o piloto. Cada integração deve definir sistema responsável, contratos, estado do benefício e reconciliação. Antes de ampliar o escopo, documentar como suspender novas concessões, preservar registros, tratar benefícios pendentes e recuperar a operação anterior. O detalhe dependerá do mecanismo de crédito escolhido. Nenhum legado é desligado automaticamente.

## Governança

Produto, arquitetura, segurança, risco, jurídico, finanças e operações validam as decisões de sua competência. Registrar decisões e exceções; testar regras, integração e observabilidade; revisar acessos; acompanhar resultados e incidentes. A arquitetura de transição inspira-se na modernização gradual (*Strangler Fig*), sem prazo ou orçamento presumido.
