# Landing page da TrustCo — instruções para agentes

## Fluxo de trabalho — Issues e Pull Requests

Toda tarefa de desenvolvimento neste repositório — correção de bug, melhoria ou funcionalidade nova — segue este fluxo. Vale para qualquer agente, de qualquer modelo, trabalhando neste código, e para qualquer pessoa também.

1. **Abra uma Issue antes de começar o trabalho.** Título curto e descritivo, corpo explicando o problema ou o pedido — o "porquê", não só o "o quê". Use os labels `bug`, `enhancement` ou `feature` quando existirem no repositório.
2. **Trabalhe numa branch**, nunca direto em `main`. Nome sugerido: `tipo/descricao-curta` — ex.: `fix/preco-plano-errado`, `feat/exportar-orcamento-pdf`.
3. **Abra um Pull Request** para mesclar a branch, e **mencione a Issue na descrição do PR** (`Closes #12`, `Fixes #12` ou `Refs #12`). Isso fecha a Issue automaticamente na mesclagem e deixa o histórico rastreável — dá para responder "por que essa linha existe" meses depois, olhando a Issue e o PR juntos.
4. **A mesclagem do PR em `main` é o gatilho de deploy** (Vercel ou Railway, conforme o serviço). Por isso mesclar um PR carrega a mesma cautela que subir para produção diretamente: confirme com o dono do projeto antes de mesclar, a menos que ele já tenha dado autorização permanente para isso.

**Exceção:** uma correção trivial e urgente que está travando produção (ex.: variável de ambiente errada) pode ir direto — mas abra a Issue e o PR retroativamente, para o rastro não se perder.
