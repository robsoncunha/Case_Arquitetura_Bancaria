# Documento de arquitetura de solução — visão inicial

## Situação e limites
Proposta conceitual para avaliação de Enterprise Architecture. Não constitui desenho detalhado nem comprova aderência regulatória. A fase A é o foco; as decisões técnicas abaixo exigem investigação nas fases B a D.

## Componentes lógicos
| ABB | Responsabilidade | SBB candidato, sujeito a seleção |
|---|---|---|
| Cliente e elegibilidade | Identificar cliente e verificar condições | API existente ou novo serviço |
| Gestão de parceiros | Manter parceiros e condições comerciais | Serviço de parceiros ou plataforma contratada |
| Cashback | Calcular, registrar e reverter benefícios | Serviço de recompensa com dados próprios |
| Integração | Trocar comandos e eventos com legados | APIs, adaptadores e mensageria existentes ou selecionados |
| Conciliação | Comparar transações, benefícios e créditos | Componente de conciliação e fila de exceções |

## Princípios técnicos
Decompor por capacidade e limites de domínio; evitar compartilhamento direto de banco entre contextos; contratos versionados; registros auditáveis; autorização por responsabilidade. Avaliar outbox transacional, idempotência, reprocessamento e compensação para eventos. A escolha entre chamada síncrona e evento depende da operação e do requisito de consistência.

## DDD tático: exemplo
No contexto Cashback, um **Benefício** pode ser um agregado com identidade, valor, origem e estado. O cálculo aplica regras de elegibilidade. Um evento `BeneficioCalculado` pode comunicar o resultado após persistência confiável. Estorno e crédito devem respeitar as invariantes definidas no domínio. Este é um modelo inicial a validar.

## Pendências críticas
Origem e qualidade dos eventos; elegibilidade dos produtos; meio de crédito; contratos e financiamento dos parceiros; segurança e privacidade; regras contábeis e regulatórias; níveis de serviço; dados pessoais; capacidade de conciliar e reverter. Envolver negócio, jurídico, risco, segurança, operações e finanças.
