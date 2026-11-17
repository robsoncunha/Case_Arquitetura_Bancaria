# 7. Método e conceitos

[Início](../README.md) | Anterior: [Migração](06-migracao-e-governanca.md)

## Aplicação proporcional do TOGAF ADM

A entrega foca a fase **A — Visão de Arquitetura**. As demais fases indicam como aprofundar e governar a proposta; não representam trabalho já executado.

| Etapa | Aplicação ao case | Evidência esperada |
|---|---|---|
| Preliminar | Princípios, governança e responsabilidade | Mandato e princípios acordados |
| A — Visão | Objetivos, stakeholders, escopo e recomendação | Visão aprovada e hipóteses registradas |
| B — Negócio | Capacidades, domínios e jornada | Mapa de capacidades e regras validadas |
| C — Dados e aplicações | Dados, contextos e integrações | Inventário, contratos e responsabilidades |
| D — Tecnologia | Infraestrutura, segurança e operação | Escolhas técnicas e requisitos acordados |
| E — Oportunidades | Opções e pacotes de trabalho | Alternativas e arquiteturas intermediárias |
| F — Migração | Sequência, dependências e transição | Plano e critérios de passagem |
| G — Implementação | Acompanhar aderência da entrega | Revisões e evidências de conformidade |
| H — Mudança | Avaliar mudanças no negócio e na arquitetura | Impactos e decisões documentadas |
| Contínuo | Gestão de requisitos | Rastreabilidade e controle de alterações |

O ADM é iterativo: descobertas em dados, aplicações ou tecnologia podem alterar decisões anteriores.

## Por que usar estas abordagens?

- **ADM:** organiza visão, arquitetura, transição e governança conforme o escopo do case.
- **DDD estratégico:** ajuda a separar responsabilidades de negócio e definir contratos entre contextos.
- **DDD tático:** ajuda a explicitar regras e invariantes dentro de cada contexto.
- **Microservices:** é uma restrição do case. A decomposição proposta começa por capacidades e contextos, seguida de validação de coesão, dados e autonomia operacional.
- **Strangler Fig:** orienta a substituição gradual quando ela se mostrar necessária, preservando coexistência e reversão.

## ABB e SBB

Um **Architecture Building Block (ABB)** descreve uma capacidade ou componente lógico necessário à arquitetura. Um **Solution Building Block (SBB)** é uma solução concreta que realiza capacidades arquiteturais. Por exemplo, “gestão de cashback” é um ABB candidato; um serviço específico de recompensas, escolhido e implementado, pode ser um SBB. Veja a tabela de [blocos propostos](04-arquitetura-alvo-to-be.md#candidatos-a-contextos-e-building-blocks).
