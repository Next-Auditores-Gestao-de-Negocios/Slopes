# Materiais — Next Auditores

Página de índice dos materiais publicados, servida pelo GitHub Pages.

## Estrutura

```
index.html                 página principal
.nojekyll                  desliga o processamento Jekyll do GitHub
assets/fontes/             fontes da marca (Caslon, Maison Neue, Neue Haas)
assets/img/capa.png        imagem da prévia do link (1200×630)
assets/img/favicon.png     ícone da aba
assets/img/linhas.png      textura de fundo
assets/logos/              wordmark
```

## Publicar

1. Suba todos os arquivos na raiz do repositório.
2. **Settings → Pages → Source:** `Deploy from a branch`, branch `main`, pasta `/ (root)`.
3. Abra `https://SEUUSUARIO.github.io/SEUREPO/` para conferir.

## Antes de divulgar o link

No `index.html`, troque `SEUUSUARIO` e `SEUREPO` nas duas tags `og:url` e
`og:image`. Elas exigem URL completa — caminho relativo não funciona na prévia.

## Adicionar um material

Duplique um bloco `<a class="item">` dentro de `<main>` e aponte o `href` para a
pasta ou o PDF do material.
