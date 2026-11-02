# Nova Saúde — Protocolo de 90 Dias (site)

Site estático para GitHub Pages, com domínio **umanovavidahoje.com**. Sem servidor e sem build.

## 1. Publicar no GitHub
1. Crie um repositório público (ex.: `novasaude`).
2. Envie TODOS os arquivos desta pasta para a raiz (inclusive `.nojekyll` e `CNAME`).
3. Em **Settings > Pages**: *Deploy from a branch*, branch **main**, pasta **/ (root)**, Save.

## 2. Domínio umanovavidahoje.com
O arquivo `CNAME` já contém o domínio. Em **Settings > Pages > Custom domain**, confirme `umanovavidahoje.com`.

No painel onde você registrou o domínio (DNS), crie:

| Tipo  | Nome (host) | Valor |
|-------|-------------|-------|
| A     | @           | 185.199.108.153 |
| A     | @           | 185.199.109.153 |
| A     | @           | 185.199.110.153 |
| A     | @           | 185.199.111.153 |
| CNAME | www         | SEU-USUARIO.github.io |

Aguarde a propagação (de minutos a 24h), volte em Settings > Pages e marque **Enforce HTTPS**.
Com isso, `www.umanovavidahoje.com` redireciona para `umanovavidahoje.com`.

## 3. Depois de publicar
- Teste o compartilhamento em https://developers.facebook.com/tools/debug/ (imagem og-image.png).
- Cadastre o site no Google Search Console e envie `https://umanovavidahoje.com/sitemap.xml`.

## Arquivos
- `index.html`: página de vendas (configurações em `SITE_CONFIG`)
- `termos.html`, `privacidade.html`: modelos iniciais (revise com profissional jurídico)
- `404.html`, `CNAME`, `robots.txt`, `sitemap.xml`, `.nojekyll`
- `favicon.svg`, `apple-touch-icon.png`, `icon-512.png`, `logo.svg`, `og-image.png`
