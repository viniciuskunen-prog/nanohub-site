# AGENTS.md — OV Stúdio

## OV STÚDIO — Norma transversal de engenharia (v1.0; 16/10/2026)

Fonte canônica: https://docs.google.com/document/d/1sNETKe0Lro4GVlQChUqLfJNWIbjFiv6CNHeibpjdNro/edit
Política de GitHub Actions **prioritária**: https://docs.google.com/document/d/1SjNmzQY7w2CsAAXDpCOqRXCwMMuG1pjGBu997T20KdY/edit

Esta camada complementa instruções locais; NÃO revoga restrições específicas. Em divergências, preservar segurança/custo mais restritivos e decisões expressas do proprietário; documentar conflitos.

1. Antes de alterar: explicitar objetivo, exclusões (o que NÃO alterar), pré-validação/dry-run e prova de resultado. Classificar risco R0–R3.
2. Alterar apenas o escopo; preservar autoria, licença, dados, interfaces, proteções do sistema e compatibilidade. Dependências novas exigem justificativa.
3. Bug reproduzível: criar regressão que falhe antes e passe depois; se inviável, justificar e registrar passo de teste manual. Testar código real, não apenas mocks hipotéticos.
4. Reportar apenas comandos e resultados realmente executados. CI bloqueada NÃO significa teste aprovado.
5. Não commitar segredos, dados de clientes ou tokens. Dados fictícios nos testes; menor privilégio e confirmação antes de operações irreversíveis.
6. CI econômica: checar gatilhos e cota ANTES de alterar workflows. Priorizar testes locais, agrupar commits, evitar runners macOS hospedados automáticos, builds caros e reexecuções cegas. Não desabilitar gates de segurança.
7. Release exige versão identificável, smoke test, backup e rollback proporcionais ao risco. Deploy e migração destrutiva exigem validação antes e depois.
8. Na entrega: registrar diff, testes feitos/não feitos, riscos, rollback e pendências. Reconciliar o estado canônico do projeto em GPT WORKSPACE no Drive; não presumir sincronização automática.

Foco local: Preservar integrações e URLs públicas; testar responsividade sem criar CI de alto custo.
