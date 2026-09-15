# Dedetizamed — Especificação do Site

> Reconstrução completa (v2) de 2026-09-15: o cliente rejeitou a primeira versão
> ("não gostei", depois "recomeçar do zero") e pediu um visual mais moderno,
> com fotos reais, inspirado em dois concorrentes (dedetizadoraberbert.com.br,
> vetpragas.com.br). Este documento reflete o estado atual.

## 1. Objetivo

Construir:
1. Um **site institucional** (4 páginas) apresentando a empresa e seus serviços.
2. **2 landing pages (LPs) isoladas**, sem navegação, para rodar tráfego pago
   (Google/Meta Ads): uma para Medianeira e região, uma para Maringá.

Objetivo primário: geração de lead via WhatsApp. Credibilidade institucional é objetivo secundário, atendido pelo site institucional.

## 2. A empresa

- **Nome fantasia**: dedetizamed — Soluções em Controle Ambiental
- **Razão social**: Antonio Clair Rodrigues Muniz Dedetização
- **CNPJ**: 04.946.748/0001-32 *(exibir no rodapé de todas as páginas do site institucional)*
- **Tempo de mercado**: +20 anos de experiência
- **Matriz**: Rua Rio Grande do Norte, nº 2371 — Casa — Cidade Alta, Medianeira-PR
- **Filial**: Maringá-PR (recém aberta; atende **somente** controle de pragas, sem limpeza de caixa d'água). A filial de Maringá **não** aparece no site institucional — só na LP de Maringá.
- **Contato oficial (Medianeira)**: WhatsApp/telefone (45) 99810-2698
- **Contato Maringá (só na LP de Maringá)**: WhatsApp 44 98833-4877
- **E-mail**: não exibir (não existe / não é necessário)

### Diferenciais

- ✔️ Especialistas em controle ambiental
- ✔️ Diagnóstico correto para cada tipo de praga
- ✔️ Métodos seguros para pessoas e pets
- ✔️ Atendimento rápido e organizado
- ✔️ Garantia de serviço (3 meses)
- Empresa registrada e licenciada
- **Emissão de Laudo Técnico** — destacado como serviço/diferencial próprio, principal gatilho de conversão do público B2B

## 3. Identidade visual

**Marca (fixa, não muda entre versões)**: vermelho `#FF0000`, amarelo `#FFF000`, cinza-chumbo `#323232`, logo em `MANUAL DE IDENTIDADE/`.

**Direção v2 (atual)** — confiante/corporativa, inspirada em dedetizadoraberbert.com.br e vetpragas.com.br, traduzida pra paleta própria (sem introduzir azul):
- Base quase-preta (`#161616`) dominante em seções de peso; vermelho gasto com intenção (CTAs, faixa de urgência no topo, seções cheias); amarelo como acento raro só em fundos escuros.
- Tipografia: **Barlow Condensed** (títulos, uppercase só em h1 e labels curtos) + **Karla** (corpo).
- Assinatura visual: títulos em duas linhas (`heading-duo`), primeira linha cor `ink`, segunda em vermelho/amarelo.
- Ícones: sprite SVG geométrico autoral (não emoji/unicode), em badges quadrados escuros (serviços) ou chips com contorno (linhas compactas).
- Fotografia real (banco gratuito, ver `PHOTO-CREDITS.md`): técnico aplicando produto (hero/Sobre/LPs de pragas) + grid circular de 5 fotos macro de pragas (baratas, ratos, cupim, formigas, escorpiões) na Home e nas LPs de pragas.
- Sem eyebrow/kicker acima de títulos (banido pelo skill de design usado na implementação).

## 4. Site institucional

Sem CMS. 4 páginas estáticas, navegação completa entre elas. Idioma: português (Brasil). Sem menção à filial de Maringá em nenhuma página.

### Páginas

1. **Início** — hero com foto real + proposta de valor + prova social; seção de dor real; diferenciais; grid de pragas combatidas; como funciona; serviços em destaque + laudo técnico; segmentos atendidos (sem logo/depoimento fabricado); residencial × empresa; garantia; FAQ; CTA final.
2. **Sobre** — história (+20 anos) com foto real, diferenciais, dados legais (CNPJ/razão social).
3. **Serviços** — lista completa: dedetização, desratização, descupinização, controle de escorpiões, limpeza de caixa d'água (exclusiva Medianeira), emissão de laudo técnico; segmentos atendidos por serviço.
4. **Contato** — WhatsApp/telefone, endereço da matriz, link para o Google Maps, CNPJ/razão social no rodapé (repetido em todas as páginas).

### CTA de WhatsApp (site institucional)

Mensagem pré-preenchida genérica: **"Olá, vim pelo site"**. Botão flutuante de WhatsApp presente em todas as páginas (institucionais e LPs).

### Imagens

Fotos reais de banco gratuito (Openverse — Flickr/Wikimedia, licenças livres), créditos em `PHOTO-CREDITS.md` e em comentário HTML acima de cada `<img>`. Trocar por material próprio assim que o cliente fornecer.

## 5. Landing Pages (tráfego pago)

Isoladas: **sem header de navegação, sem menu, sem links de saída**. Único CTA é o botão de WhatsApp (fixo + inline). Sem formulário.

| LP | URL | Escopo | WhatsApp | Mensagem pré-preenchida |
|---|---|---|---|---|
| LP1 | `/lp/pragas-medianeira.html` | Controle de pragas em Medianeira e região | (45) 99810-2698 (matriz) | "Olá, vim pelo site e quero um orçamento para controle de pragas" |
| LP2 | `/lp/pragas-maringa.html` | Idêntica à LP1, headline citando **Maringá** | 44 98833-4877 | "Olá, vim pelo site e quero um orçamento para controle de pragas" |

Notas:
- LP2 é a única página do projeto onde Maringá é mencionada.
- Hero das LPs usa a foto real do técnico como fundo escurecido (mesma foto do hero institucional).
- Limpeza de caixa d'água não tem LP dedicada nesta rodada (fora de escopo por ora); continua listada como serviço em `servicos.html`.

## 6. Rastreamento de anúncios

Nenhuma tag configurada ainda (Meta Pixel / Google Ads Conversion Tag). Cliente vai configurar após o site estar pronto.

## 7. Stack técnica

- **HTML/CSS/JS puro**, sem framework, sem build step, sem CMS.
- Todas as edições de conteúdo serão feitas via Claude Code diretamente no código-fonte.
- Multi-página (não SPA): cada página institucional e cada LP é um arquivo `.html` próprio, com o sprite de ícones inlinado em cada uma (`<use>` cross-documento é pouco confiável — ver histórico do projeto).

## 8. Domínio e hospedagem

- **Domínio**: `dedetizamed.com.br` — registro ativo e pago, gerenciado no painel da **Hostinger** (cliente tem acesso de login).
- **Hospedagem de destino**: **Vercel**. Cliente já tem conta e fará o "Import from GitHub" manualmente, apontando o Root Directory pra `public`.

## 9. Controle de versão

- Repositório: `https://github.com/victordmuniz/dedetizamed`
- Fluxo: desenvolvimento local via Claude Code → commit → push.

## 10. Fora de escopo (por ora)

- CMS ou painel de edição de conteúdo para o cliente.
- Blog.
- Formulários de contato (tudo via WhatsApp).
- Meta Pixel / Google Ads Tag.
- Banner de cookies / aviso de privacidade.
- LP dedicada de limpeza de caixa d'água.
- Fotos próprias do cliente (usando banco gratuito por ora, ver `PHOTO-CREDITS.md`).
