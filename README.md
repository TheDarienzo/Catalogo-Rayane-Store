# Rayane Store — Catálogo

Site do catálogo (build pronto do app React), publicado pelo GitHub Pages em https://catalogo.rayanestore.com.br.

- `index.html`, `assets/`, ícones e `logo.png`: o app, como foi construído (Vite).
- `404.html`: cópia do `index.html`, para que rotas do app (ex.: `/p/<id-do-produto>`) abram direto pelo link.
- `CNAME`: domínio próprio no GitHub Pages.
- A gestão de acessos do painel (`/api/usuarios` no antigo Worker) passou para a Edge Function `usuarios`
  no próprio Supabase do catálogo (`supabase/functions/usuarios/`).

Migrado do Cloudflare Workers (`rayane-catalogo`). Diferença: a prévia com foto do produto ao compartilhar
`/p/<id>` (tags Open Graph) não é gerada no GitHub Pages; o link abre normalmente, mas com prévia genérica.
