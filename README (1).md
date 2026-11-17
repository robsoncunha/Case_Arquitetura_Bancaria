# Case de Enterprise Architecture: cashback bancário

**Autor:** Robson Cunha  
**Situação:** proposta de arquitetura para avaliação, sujeita a validação de negócio e tecnologia.

## Contexto e recomendação
Um banco com portfólio de crédito desenvolvido em silos deseja ampliar o engajamento e acelerar novos lançamentos. O case informa boa aceitação de conta de pagamentos e cashback. A recomendação preliminar é **priorizar cashback**, começando com um produto e um parceiro, condicionada à validação econômica, operacional e regulatória. A aquisição de um core bancário permanece uma decisão posterior.

## Navegação
- [Resumo executivo](resumo_executivo.md)
- [Visão de arquitetura e diagramas](visao-arquitetura-banco.md)
- [Documento de arquitetura de solução em alto nível](DAS.md)
- [Fases do ADM](adm/README.md)
- [Decisão de produto e aquisição de core](decisoes/001-priorizar-cashback.md)
- [Apresentação principal](apresentacoes/Case_Enterprise_Architecture.pptx) e [capa e conclusão](apresentacoes/Capa_e_Conclusao_Robson_Cunha.pptx)

## Convenções
**Fato:** fornecido no enunciado. **Hipótese:** ainda precisa de evidência. **Proposta:** decisão não aprovada. **A validar:** dado, responsável ou critério ainda não informado. Não há diagnóstico real das aplicações nem métricas verificadas. O ADM é iterativo e o detalhamento das fases posteriores é indicativo.

## Fontes
- [The Open Group: TOGAF e ArchiMate](https://help.opengroup.org/hc/en-us/articles/32115987894930-How-the-ArchiMate-Language-and-the-TOGAF-Standard-Complement-Each-Other)
- [Banco Central: contas de pagamento](https://www.bcb.gov.br/meubc/faqs/s/contas-de-pagamento)
- [Martin Fowler: Strangler Fig](https://martinfowler.com/bliki/StranglerFigApplication.html)

## Preparar um repositório Git
Na pasta extraída: `git init -b main`, `git add .` e `git commit -m "Documenta visão de arquitetura do case bancário"`. Depois associe o endereço do repositório desejado com `git remote add origin <URL_DO_REPOSITORIO>` e execute `git push -u origin main`. A criação e a visibilidade do repositório dependem da sua escolha no GitHub.
