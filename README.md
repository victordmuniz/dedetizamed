# dedetizamed

Site institucional + landing pages de anúncio da dedetizamed (Medianeira-PR).

## Estrutura

- `public/` — código-fonte do site (o que é publicado). Configure o **Root Directory** do projeto na Vercel como `public`.
  - `index.html`, `sobre.html`, `servicos.html`, `contato.html` — site institucional.
  - `lp/pragas-medianeira.html`, `lp/pragas-maringa.html` — landing pages isoladas para anúncio (sem menu).
  - `assets/photos/` — fotos reais de banco gratuito, ver `PHOTO-CREDITS.md`.
- `MANUAL DE IDENTIDADE/` — arquivos originais de logo e paleta de cores da marca (referência, não servido pelo site).
- `SPEC.md` — especificação funcional do projeto.
- `PHOTO-CREDITS.md` — créditos e licenças das fotos usadas.

## Stack

HTML/CSS/JS puro, sem framework, sem build step. Deploy via Vercel a partir deste repositório GitHub (`victordmuniz/dedetizamed`).

## Direção visual

Confiante/corporativa: base quase-preta, vermelho usado com peso (CTAs, faixa de urgência, seções cheias), amarelo como acento raro, tipografia Barlow Condensed (títulos) + Karla (corpo), títulos em duas linhas (ink + vermelho). Referências: dedetizadoraberbert.com.br, vetpragas.com.br — traduzidas pra paleta própria da marca (vermelho/amarelo/cinza-chumbo), sem introduzir azul.
