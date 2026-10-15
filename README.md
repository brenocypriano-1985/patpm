# Painel Territorial PATPM — publicação em articuladorasterritoriais.com

Conteúdo deste pacote
- `index.html` — ciclo mais recente (julho a setembro de 2026).
- `setembro-2026/index.html` — mesma versão, em endereço fixo por ciclo. A cada novo ciclo, acrescenta-se uma pasta (`outubro-2026/`) e substitui-se o `index.html` da raiz.
- `CNAME` — nome do domínio, usado pelo GitHub Pages.

Opção A — GitHub Pages (gratuito, estável, com HTTPS automático)
1. Crie uma conta em github.com (ou use a existente) e um repositório público chamado `painel` (qualquer nome serve).
2. Envie os arquivos deste pacote para a raiz do repositório (botão "Add file" → "Upload files"), mantendo a pasta `setembro-2026`.
3. Em Settings → Pages: Source = "Deploy from a branch", Branch = `main`, pasta `/ (root)`. Salve.
4. Ainda em Settings → Pages, em "Custom domain", digite `articuladorasterritoriais.com` e salve; marque "Enforce HTTPS" quando a opção ficar disponível (alguns minutos depois do DNS).

DNS no Wix (painel do domínio → "Gerenciar registros DNS")
- Quatro registros A para o domínio raiz (host `@`), apontando para: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153.
- Um registro CNAME para `www`, apontando para `SEU-USUARIO.github.io` (o usuário da conta GitHub).
- Remova registros A/CNAME que o Wix tenha criado para o site dele, se não for usar um site Wix no mesmo domínio.
- Propagação: de alguns minutos a 24 h. Teste em https://articuladorasterritoriais.com e, no celular, pelo QR do relatório.

Opção B — Cloudflare Pages ou Netlify
- Arraste a pasta deste pacote para "Create project" (Cloudflare Pages) ou "Deploy manually" (Netlify) e, nas configurações do projeto, adicione o domínio personalizado; o serviço informa os registros DNS a criar no Wix (um CNAME ou registros A).

Atualização a cada ciclo
- Substituir `index.html` pela nova versão e acrescentar a pasta do ciclo. O endereço não muda; o QR e o link dos relatórios continuam válidos.

Observação
- A página é um único arquivo, sem servidor nem banco; carrega apenas as fontes do Google Fonts. Não há dados pessoais nem identificação de instituições.
