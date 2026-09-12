# Dedetizamed — Especificação do Site

> Documento de referência para implementação. Reflete as decisões tomadas na entrevista de escopo (grilling) de 2026-09-12.

## 1. Objetivo

Construir:
1. Um **site institucional** (4 páginas) apresentando a empresa e seus serviços.
2. **3 landing pages (LPs) isoladas**, sem navegação, para rodar tráfego pago (Google/Meta Ads) em cidades específicas.

Objetivo primário: geração de lead via WhatsApp. Credibilidade institucional é objetivo secundário, atendido pelo site institucional.

## 2. A empresa

- **Nome fantasia**: dedetizamed — Soluções em Controle Ambiental
- **Razão social**: Antonio Clair Rodrigues Muniz Dedetização
- **CNPJ**: 04.946.748/0001-32 *(exibir no rodapé de todas as páginas do site institucional)*
- **Tempo de mercado**: +20 anos de experiência
- **Matriz**: Rua Rio Grande do Norte, nº 2371 — Casa — Cidade Alta, Medianeira-PR
- **Filial**: Maringá-PR (recém aberta; atende **somente** controle de pragas, sem limpeza de caixa d'água). A filial de Maringá **não** aparece no site institucional — só na LP de Maringá.
- **Contato oficial (Medianeira)**: WhatsApp/telefone (45) 99810-2698
- **E-mail**: não exibir (não existe / não é necessário)

### Diferenciais (usar como copy de destaque na home e/ou seção "Por que a dedetizamed")

- ✔️ Especialistas em controle ambiental
- ✔️ Diagnóstico correto para cada tipo de praga
- ✔️ Métodos seguros para pessoas e pets
- ✔️ Atendimento rápido e organizado
- ✔️ Garantia de serviço (3 meses)
- Empresa registrada e licenciada
- **Emissão de Laudo Técnico** — destacar como serviço/diferencial próprio, é o principal gatilho de conversão do público B2B (ver seção 4)

## 3. Identidade visual

Ativos em `MANUAL DE IDENTIDADE/` (todos os arquivos de logo contêm a mesma marca, apesar dos nomes de arquivo — não há versões conflitantes a resolver).

**Cores** (usar os hex do arquivo `cores.png`, que é a paleta oficial da marca — ignorar os tons do arquivo `paleta.JPG`, que é só uma referência de inspiração genérica):

| Uso | Hex |
|---|---|
| Vermelho (primária) | `#FF0000` |
| Amarelo (destaque/CTA) | `#FFF000` |
| Cinza-chumbo (texto/contraste) | `#323232` |

**Logo**: usar arquivos da pasta `MANUAL DE IDENTIDADE/` (versão com o slogan "Soluções em Controle Ambiental" no cabeçalho/hero; pode-se usar só o símbolo "dm" — arquivo `a.png` — como favicon).

**Tipografia/tom**: manter a mistura já usada na marca (wordmark bold + slogan em script) como referência de personalidade — definir fontes web equivalentes na implementação.

## 4. Site institucional

Sem CMS. 4 páginas estáticas, navegação completa entre elas. Idioma: português (Brasil). Sem menção à filial de Maringá em nenhuma página.

### Páginas

1. **Início** — hero com proposta de valor + diferenciais + CTA WhatsApp + prévia dos serviços.
2. **Sobre** — história (+20 anos), diferenciais, licenciamento, CNPJ/razão social.
3. **Serviços** — lista completa:
   - Dedetização (baratas/formigas)
   - Desratização
   - Descupinização
   - Controle de escorpiões
   - Limpeza de caixa d'água
   - Emissão de Laudo Técnico *(serviço/diferencial próprio — ver seção 2)*
   - Segmentos atendidos: residencial, comercial, industrial, condomínios, indústria alimentícia, bares/restaurantes, clínicas, farmácias — qualquer empresa que precise de laudo para operar.
4. **Contato** — WhatsApp/telefone, endereço da matriz, CNPJ/razão social no rodapé (repetido em todas as páginas).

### CTA de WhatsApp (site institucional)

Mensagem pré-preenchida genérica em todos os botões: **"Olá, vim pelo site"**.

### Imagens

Sem material fotográfico disponível ainda. Estratégia:
- **Cards de serviço**: ícones ilustrativos desenhados nas cores da marca (baratas, ratos, cupim, escorpião, caixa d'água, laudo/documento) — não usar banco de imagens genérico, não deixar em branco.
- **Hero, equipe, seção "Sobre", antes/depois**: reservar espaço com placeholder visualmente identificado (ex: bloco com ícone de câmera + texto discreto), para substituição futura por fotos reais do cliente.

## 5. Landing Pages (tráfego pago)

Isoladas: **sem header de navegação, sem menu, sem links de saída** para o site institucional. Única ação disponível na página é o botão de WhatsApp. Cada LP tem sua própria URL.

| LP | URL sugerida | Escopo | WhatsApp | Mensagem pré-preenchida |
|---|---|---|---|---|
| LP1 | `/lp/pragas-medianeira` | Todo controle de pragas (sem caixa d'água) | (45) 99810-2698 (matriz) | "Olá, vim pelo site e quero um orçamento para controle de pragas" |
| LP2 | `/lp/pragas-maringa` | Idêntica à LP1, headline citando **Maringá** explicitamente (relevância de anúncio) | 44 98833-4877 | "Olá, vim pelo site e quero um orçamento para controle de pragas" |
| LP3 | `/lp/caixa-dagua` | Limpeza de caixa d'água (exclusivo Medianeira) | (45) 99810-2698 (matriz) | "Olá, quero um orçamento para limpeza de caixa d'água" |

Notas:
- LP2 é a única página do projeto onde Maringá é mencionada.
- Nenhuma LP tem formulário — conversão é 100% via clique no WhatsApp.
- Preparar os botões com hooks/atributos (`data-*` ou IDs previsíveis) prontos para receber Meta Pixel / Google Ads Tag depois, sem precisar reestruturar o HTML.

## 6. Rastreamento de anúncios

Nenhuma tag configurada ainda (Meta Pixel / Google Ads Conversion Tag). Cliente vai configurar após o site estar pronto. Deixar os pontos de instrumentação (cliques de WhatsApp, page view) fáceis de conectar depois, mas **não** instalar pixels agora. Sem banner de cookies por enquanto (reavaliar quando as tags entrarem).

## 7. Stack técnica

- **HTML/CSS/JS puro**, sem framework, sem build step, sem CMS.
- Todas as edições de conteúdo serão feitas via Claude Code diretamente no código-fonte.
- Multi-página (não SPA): cada página institucional e cada LP é um arquivo `.html` próprio.

## 8. Domínio e hospedagem

- **Domínio**: `dedetizamed.com.br` — registro ativo e pago, gerenciado no painel da **Hostinger** (cliente tem acesso de login).
- **Hospedagem de destino**: **Vercel**. Hospedagem atual na Hostinger não está sendo usada/paga — DNS precisa ser repontado para a Vercel.
- Cliente já tem conta na Vercel; fará o **"Import from GitHub"** manualmente quando o repositório estiver pronto, e aplicará os registros DNS que forem indicados no painel da Hostinger.

## 9. Controle de versão

- Repositório: `https://github.com/victordmuniz/dedetizamed`
- Fluxo: desenvolvimento local via Claude Code neste diretório → commit → push para o repositório do cliente.
- ⚠️ Autenticação: nesta sessão não havia GitHub CLI/config configurados; um Personal Access Token foi fornecido pelo cliente no chat para viabilizar o primeiro push. Ele deve ser usado apenas localmente (credential store), nunca commitado, e **revogado/rotacionado** pelo cliente assim que a configuração inicial funcionar (foi exposto em texto de chat).

## 10. Fora de escopo (por ora)

- CMS ou painel de edição de conteúdo para o cliente.
- Blog.
- Formulários de contato (tudo via WhatsApp).
- Meta Pixel / Google Ads Tag (a configurar depois pelo cliente).
- Banner de cookies / aviso de privacidade (reavaliar quando pixels entrarem).
- Fotos reais (aguardando material do cliente).
