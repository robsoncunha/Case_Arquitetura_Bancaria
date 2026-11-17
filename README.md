# Arquitetura empresarial para evolução do portfólio bancário

**Case de avaliação | Autor: Robson Cunha**

Este repositório apresenta uma visão de arquitetura para um banco com produtos de crédito organizados em silos. A proposta prioriza um programa de cashback com parceiros e uma evolução gradual das capacidades do banco, mantendo o estilo de microservices informado no case.

## Como interpretar as informações

- **Fato do case:** informação fornecida no enunciado.
- **AS-IS fictício:** cenário criado para demonstrar o raciocínio arquitetural. Não descreve sistemas confirmados.
- **Hipótese:** condição que precisa de evidência.
- **Proposta:** recomendação sujeita à decisão das áreas responsáveis.

A escolha de cashback não está baseada em números de custo ou retorno, pois esses dados não foram fornecidos. A arquitetura atual fictícia é independente de qualquer banco real.

## Consulta rápida

| Pergunta | Local |
|---|---|
| Por que cashback e não conta de pagamentos? | [Decisão executiva](docs/01-contexto-e-decisao.md#recomendação-e-alternativas) |
| Onde estão os silos e seus impactos? | [AS-IS fictício](docs/03-arquitetura-atual-as-is.md) |
| Como será a integração alvo? | [TO-BE proposto](docs/04-arquitetura-alvo-to-be.md) |
| Como ocorre a transição sem desligamento abrupto? | [Migração](docs/06-migracao-e-governanca.md) |

## Referências conceituais

- [The Open Group — TOGAF e ArchiMate](https://help.opengroup.org/hc/en-us/articles/32115987894930-How-the-ArchiMate-Language-and-the-TOGAF-Standard-Complement-Each-Other)
- [Banco Central do Brasil — contas de pagamento](https://www.bcb.gov.br/meubc/faqs/s/contas-de-pagamento)
- [Martin Fowler — Strangler Fig](https://martinfowler.com/bliki/StranglerFigApplication.html)
