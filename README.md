# dataskill.app — site

Site estático (um único `index.html`), pronto para o GitHub Pages.

## Publicar

1. Crie um repositório no GitHub (ex.: `dataskill-site`) e envie estes arquivos para a branch `main`.
2. No repositório: **Settings → Pages → Build and deployment → Deploy from a branch → main / (root)**.
3. Em **Custom domain**, digite `dataskill.app` (o arquivo `CNAME` já está aqui) e marque **Enforce HTTPS** quando liberar.

## DNS (no painel onde você comprou o domínio)

| Tipo | Nome | Valor |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| AAAA | @ | 2606:50c0:8000::153 |
| AAAA | @ | 2606:50c0:8001::153 |
| AAAA | @ | 2606:50c0:8002::153 |
| AAAA | @ | 2606:50c0:8003::153 |
| CNAME | www | SEU-USUARIO.github.io |

Confira os valores atuais na documentação do GitHub Pages ("Managing a custom domain"). A propagação pode levar algumas horas.

Domínios `.app` exigem HTTPS no navegador: o site só abre depois que o GitHub emitir o certificado (passo 3).

## Arquivos

- `index.html` — o site completo (HTML, CSS e JS num arquivo só)
- `favicon.svg` — ícone da aba
- `logo-simbolo.svg` / `logo-simbolo-claro.svg` — símbolo para fundo escuro e claro
- `CNAME` — domínio personalizado

## Editar

- Textos e seções: direto no `index.html`
- Cores: bloco `:root` no topo do `<style>`
- Exemplos por tipo de negócio: objeto `segs`; gráfico do topo: array `dados` (ambos no `<script>` do fim do arquivo)
