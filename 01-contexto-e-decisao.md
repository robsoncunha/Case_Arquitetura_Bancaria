# 1. Contexto e decisão executiva

[Início](../README.md) | Próximo: [Negócio](02-arquitetura-de-negocio.md)

## Fatos fornecidos

O banco, oferece os produtos CDC, cartão de crédito, crédito pessoal, consignado e empréstimos com garantia. As capacidades foram construídas em silos, com baixo reaproveitamento. Conta de pagamentos e cashback com parcerias tiveram boa aceitação em testes, mas a direção pretende priorizar apenas um dos produtos. O estilo arquitetural vigente é microservices. O CTO sugere avaliar a aquisição de uma plataforma de core bancário.

O enunciado não informa resultados numéricos dos testes, custos, contratos, integração existente, indicadores ou nomes de sistemas. Esses dados devem ser levantados antes de uma decisão definitiva.

## Objetivos

- Aumentar a frequência de relacionamento com os clientes.
- Habilitar um novo produto com valor mensurável.
- Reduzir dependências entre silos e aumentar o reaproveitamento.
- Preservar a continuidade dos produtos existentes durante a mudança.

## Recomendação e alternativas

**Proposta:** iniciar um piloto de cashback para um produto de crédito e um parceiro. O piloto permite testar a hipótese de que transações e relacionamentos existentes podem viabilizar engajamento e capacidades reutilizáveis. O meio de crédito da recompensa ainda precisa ser definido.

| Critério | Cashback com parcerias | Conta de pagamentos |
|---|---|---|
| Aceitação | Positiva no teste, sem dados comparativos | Positiva no teste, sem dados comparativos |
| Dependências | Parceiros, transações elegíveis, cálculo e crédito de recompensas | Conta, saldos, pagamentos, liquidação e operação, conforme escopo |
| Valor esperado | Estimular transações e relacionamento | Ampliar possibilidades de uso recorrente |
| Incerteza econômica | Financiamento e custo dos benefícios, acordos com parceiros | Investimento, operação, receitas e riscos |

A priorização é uma **hipótese de trabalho**; o case não prova que cashback custará menos ou será mais rentável. Validar custo por benefício, viabilidade da integração e contribuição ao engajamento. Se a hipótese não se confirmar, reavaliar a conta de pagamentos.

## Core bancário

Não há evidência suficiente para decidir a compra. Primeiro, identificar capacidades atuais e lacunas; depois, comparar reutilização, desenvolvimento e aquisição considerando aderência, integração, custo total, operação, migração, segurança e saída do fornecedor. A plataforma pode atender lacunas, mas sua aquisição isolada não elimina silos.

## Indicadores a definir

Adesão, clientes ativos, transações elegíveis, custo por benefício, exceções de conciliação e tempo de lançamento. A linha de base, os objetivos e os responsáveis ainda não foram informados.
