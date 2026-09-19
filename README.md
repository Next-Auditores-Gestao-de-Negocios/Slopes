<img width="1000" height="204" alt="Wordmark-Completa-Branco-Transparente" src="https://github.com/user-attachments/assets/ddc3f840-cfec-42bf-a003-a1a6479847a7" />

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">

<!-- ========================================================================
     NOME NA ABA DO NAVEGADOR
     ======================================================================== -->
<title>Next Auditores — Materiais e publicações</title>
<meta name="description" content="Relatórios, pareceres e materiais técnicos publicados pela Next Auditores.">

<!-- ========================================================================
     ÍCONE DA ABA
     ======================================================================== -->
<link rel="icon" type="image/png" href="assets/img/favicon.png">
<link rel="apple-touch-icon" href="assets/img/apple-touch-icon.png">

<!-- ========================================================================
     PRÉVIA DO LINK (WhatsApp, Teams, LinkedIn, e-mail)
     TROQUE "SEUUSUARIO" E "SEUREPO" PELOS SEUS — precisa ser URL completa.
     ======================================================================== -->
<meta property="og:type" content="website">
<meta property="og:site_name" content="Next Auditores">
<meta property="og:locale" content="pt_BR">
<meta property="og:title" content="Next Auditores — Materiais e publicações">
<meta property="og:description" content="Relatórios, pareceres e materiais técnicos publicados pela Next Auditores.">
<meta property="og:url" content="https://next-auditores-gestao-de-negocios.github.io/Slopes/">
<meta property="og:image" content="https://next-auditores-gestao-de-negocios.github.io/Slopes/assets/img/capa.png">
<meta property="og:image:width" content="1200">
<meta property="og:image:height" content="630">
<meta property="og:image:alt" content="Marca Next Auditores sobre fundo verde escuro.">
<meta name="twitter:card" content="summary_large_image">

<style>
@font-face{font-family:"Caslon";src:url("assets/fontes/CaslonMedium.ttf") format("truetype");font-weight:500;font-display:swap}
@font-face{font-family:"NHaas";src:url("assets/fontes/NHaasGroteskDSPro-75Bd.otf") format("opentype");font-weight:700;font-display:swap}
@font-face{font-family:"Maison";src:url("assets/fontes/MaisonNeue-Book.ttf") format("truetype");font-weight:400;font-display:swap}
@font-face{font-family:"Maison";src:url("assets/fontes/MaisonNeue-Medium.ttf") format("truetype");font-weight:500;font-display:swap}
@font-face{font-family:"Maison";src:url("assets/fontes/MaisonNeue-Bold.ttf") format("truetype");font-weight:700;font-display:swap}

:root{
  --verde-escuro:#001600;
  --verde-medio:#444C47;
  --cinza-medio:#E1DCDC;
  --cinza-claro:#F3F2ED;
  --dourado:#85754E;
  --medida:68ch;
}

*{box-sizing:border-box}
html{-webkit-text-size-adjust:100%}
body{
  margin:0;
  background:var(--cinza-claro);
  color:var(--verde-escuro);
  font-family:"Maison",Helvetica Neue,Arial,sans-serif;
  font-size:17px;
  line-height:1.65;
}

.faixa{max-width:1080px;margin:0 auto;padding:0 32px}

/* ---------- topo ---------- */
.capa{
  background:var(--verde-escuro);
  color:var(--cinza-claro);
  padding:88px 0 96px;
  position:relative;
  overflow:hidden;
}
.capa::after{
  content:"";position:absolute;inset:0;
  background:url("assets/img/linhas.png") center/cover no-repeat;
  opacity:.16;pointer-events:none;
}
.capa .faixa{position:relative;z-index:1}
.marca{width:230px;max-width:60vw;display:block;margin-bottom:56px}
.capa h1{
  font-family:"Caslon",Georgia,serif;
  font-weight:500;
  font-size:clamp(2.3rem,6vw,3.6rem);
  line-height:1.15;
  margin:0 0 20px;
  max-width:18ch;
}
.capa p{
  margin:0;max-width:54ch;
  color:var(--cinza-medio);
  font-size:1.05rem;
}

/* ---------- lista de materiais ---------- */
.materiais{padding:80px 0 40px}
.materiais > .faixa > h2{
  font-family:"NHaas",Arial,sans-serif;
  font-size:.95rem;
  letter-spacing:.06em;
  color:var(--verde-medio);
  margin:0 0 28px;
  font-weight:700;
}
.item{
  text-decoration:none;
  color:inherit;
  padding:28px 0;
  border-top:1px solid var(--cinza-medio);
  display:grid;
  grid-template-columns:1fr auto;
  gap:8px 32px;
  align-items:baseline;
  transition:border-color .2s ease;
}
.item:last-of-type{border-bottom:1px solid var(--cinza-medio)}
.item:hover,.item:focus-visible{border-top-color:var(--dourado)}
.item:focus-visible{outline:2px solid var(--dourado);outline-offset:4px}
.item h3{
  font-family:"Caslon",Georgia,serif;
  font-weight:500;
  font-size:1.6rem;
  line-height:1.25;
  margin:0;
}
.item p{
  grid-column:1/2;
  margin:0;
  color:var(--verde-medio);
  max-width:var(--medida);
}
.selo{
  grid-row:1/2;grid-column:2/3;
  font-family:"NHaas",Arial,sans-serif;
  font-size:.75rem;
  letter-spacing:.08em;
  color:var(--dourado);
  white-space:nowrap;
}

/* ---------- rodapé ---------- */
.rodape{
  background:var(--verde-escuro);
  color:var(--cinza-medio);
  margin-top:72px;
  padding:56px 0;
  font-size:.9rem;
}
.rodape .faixa{display:flex;gap:24px;align-items:center;justify-content:space-between;flex-wrap:wrap}
.rodape img{width:44px;height:44px}
.rodape a{color:var(--cinza-claro)}

@media (max-width:640px){
  .capa{padding:56px 0 64px}
  .materiais{padding:56px 0 24px}
  .item{grid-template-columns:1fr}
  .selo{grid-row:auto;grid-column:1/2;order:-1}
}
@media (prefers-reduced-motion:reduce){*{transition:none!important}}
</style>
</head>

<body>

<header class="capa">
  <div class="faixa">
    <img class="marca" src="assets/logos/Wordmark-Completa-Branco-Transparente.png"
         alt="Next Auditores">
    <h1>Materiais técnicos e publicações</h1>
    <p>Relatórios, pareceres e conteúdos produzidos pela equipe da Next Auditores.</p>
  </div>
</header>

<main class="materiais">
  <div class="faixa">
    <h2>Disponíveis para leitura</h2>

    <!-- Duplique um bloco destes para cada material publicado -->
    <a class="item" href="relatorio-anual/">
      <h3>Relatório anual de auditoria</h3>
      <span class="selo">2026</span>
      <p>Demonstrações financeiras, notas explicativas e o parecer da equipe.</p>
    </a>

    <a class="item" href="guia-tributario/">
      <h3>Guia de apuração tributária</h3>
      <span class="selo">Guia prático</span>
      <p>Passo a passo de apuração para empresas do setor de transporte.</p>
    </a>

    <a class="item" href="arquivos/parecer.pdf">
      <h3>Parecer técnico</h3>
      <span class="selo">PDF</span>
      <p>Análise e conclusão sobre o tema consultado pelo cliente.</p>
    </a>

  </div>
</main>

<footer class="rodape">
  <div class="faixa">
    <img src="assets/img/favicon.png" alt="">
    <span>Next Auditores</span>
    <a href="mailto:contato@nextauditores.com.br">contato@nextauditores.com.br</a>
  </div>
</footer>

</body>
</html>

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

