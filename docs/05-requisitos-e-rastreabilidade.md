# 5. Requisitos e rastreabilidade

[Início](../README.md) | Anterior: [TO-BE](04-arquitetura-alvo-to-be.md) | Próximo: [Migração](06-migracao-e-governanca.md)

Os requisitos abaixo são **propostos** e precisam de validação. “Essencial” significa candidato ao piloto, não aprovação formal.

| ID | Classificação | Requisito / regra | Prioridade proposta | Capacidade e verificação |
|---|---|---|---|---|
| RF01 | Funcional | Registrar adesão e condições aceitas | Essencial | Cliente; consulta e auditoria da adesão |
| RF02 | Funcional | Receber transação e verificar elegibilidade | Essencial | Integração e elegibilidade; transações válidas e inválidas |
| RF03 | Funcional | Calcular e registrar o benefício | Essencial | Cashback; verificar regras e limites |
| RF04 | Funcional | Conceder, consultar e estornar benefício | Essencial | Recompensa; verificar crédito, extrato e reversão |
| RF05 | Funcional | Conciliar registros e tratar divergências | Essencial | Operações; simular ausência e diferença de valores |
| RNF01 | Não funcional | Evitar benefício duplicado e garantir rastreabilidade | Essencial | Integração; repetir evento e consultar trilha |
| RNF02 | Não funcional | Proteger dados e restringir acesso | Essencial | Segurança; revisão de acesso e privacidade |
| RNF03 | Não funcional | Definir disponibilidade, recuperação e monitoração | Essencial | Operação; metas e testes a acordar |
| REG01 | Regra de negócio | Definir elegibilidade, limites e prazo de crédito | Essencial | Produto e parceiro; aprovação das regras |
| REG02 | Restrição | Validar obrigações legais, regulatórias e contábeis | Essencial | Jurídico, conformidade e finanças; parecer aplicável |
| OBJ01 | Objetivo | Aumentar engajamento e avaliar retorno | Estratégico | Produto e finanças; definir linha de base e metas |

A rastreabilidade relaciona o objetivo à jornada, às capacidades e aos testes. Os valores de disponibilidade, prazos, metas e custo são pendentes; não foram definidos no case.
