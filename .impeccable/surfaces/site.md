---
version: 1
slug: "site"
primary_target: "site"
related_targets: []
---

# Surface: dedetizamed institutional site (Início, Sobre, Serviços, Contato)

**Mode:** Persuade (lead generation via WhatsApp; credibility as supporting objective).

**Audience / job:** (1) residents/businesses in Medianeira-PR with an active pest problem wanting a fast quote; (2) B2B compliance buyers (indústria alimentícia, bares/restaurantes, clínicas, farmácias) evaluating whether this provider can be trusted to issue the laudo técnico they're legally required to have.

**Proof / content on hand:** +20 anos de mercado, licenciada/registrada, garantia de 3 meses, produtos seguros para crianças/pets, emissão de laudo técnico, CNPJ/razão social/endereço confirmados. No real photography yet — service icons stand in; hero/team/Sobre photo slots are placeholders, clearly marked, not disguised as real.

**Constraints:** HTML/CSS/JS puro, sem framework. Nenhum formulário — todo CTA aponta pro WhatsApp. Maringá nunca é mencionada aqui (só na sua landing page). CNPJ/razão social no rodapé de toda página.

## Direction contract

**THESIS:** dedetizamed convinces through committed color and immediate proof, not the muted gray-corporate register every compliance-adjacent local service defaults to into safety. Red and yellow claim full page regions the way they already claim the logo mark; credibility (licença, laudo, garantia) rides inside that same commercial energy instead of retreating to a quiet, "professional" beige.

**OWN-WORLD:** Full palette, committed at page scale: vermelho `#FF0000` (ação/urgência — CTAs, faixas inteiras), amarelo `#FFF000` (atenção/destaque — badges, ícones, realces), cinza-chumbo `#323232` (autoridade/texto, seções escuras), branco (respiro, cartões). Display type: Fredoka (peso Bold/heavy) para títulos — ecoa o peso e os cantos arredondados do próprio wordmark da marca. Corpo de texto: Nunito Sans — legível, também arredondado no caráter, nunca compete com o display. Ícones de serviço: geométricos, preenchidos (não outline), cantos arredondados, um traço/peso consistente — construídos a partir do mesmo vocabulário de anéis/arcos concêntricos da própria logo "dm" (o arco é o motivo gráfico recorrente do sistema: aparece como divisor de seção, moldura atrás de ícones, contorno de botão). Cantos arredondados em todo componente (botões, cards, badges) — nunca esquadro vivo.

**STORY:** O visitante entende em segundos que a dedetizamed resolve seu problema de praga (ou emite o laudo que sua empresa precisa) com uma equipe licenciada há mais de 20 anos; acredita que é segura (produtos pet/kid-safe), garantida (3 meses) e rápida; age clicando no WhatsApp — o CTA nunca está a mais de uma rolagem de distância, e para o público B2B o Laudo Técnico tem destaque próprio, não escondido dentro de uma lista corrida de serviços.

**FIRST VIEWPORT (Início):** Hero em bloco cheio (fundo cinza-chumbo ou vermelho — decidir no build pela leitura de contraste), motivo de arcos concêntricos da logo como elemento gráfico de fundo, título em Fredoco Bold declarando a promessa central, botão de WhatsApp em destaque (vermelho ou amarelo conforme contraste) acima da dobra, e uma faixa curta de credibilidade (licença · +20 anos · garantia de 3 meses) logo abaixo do título — não faz o visitante rolar pra achar prova de confiança.

**FORM:** Composição de "página direta de serviço local confiante" — hero cheio, faixa de credibilidade, grade de serviços com ícones (arco como moldura), bloco próprio de destaque para "Emissão de Laudo Técnico", faixa final de CTA. Decidido por confirmação compacta (pergunta de energia visual: "vibrante e comercial"; pergunta de estilo de ícone: "geométrico e arredondado"), não por sorteio via concept-seed — o brief já vinha extensamente fixado pelo SPEC.md/PRODUCT.md (conteúdo, prova, estrutura, restrições) e o projeto é code-led, sem geração de imagem disponível nesta sessão; um torneio completo de direções não se justificava para o tamanho e orçamento deste site.

**FINISH:** unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance.

## Unresolved decisions

- Hero background: charcoal vs red — decide by contrast-check once headline copy is set.
- Whether the arc motif also appears on the 3 landing pages (they extend this world, narrower composition, no nav) — likely yes for visual continuity, confirm during LP build.
