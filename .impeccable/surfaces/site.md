---
version: 1
slug: "site"
primary_target: "site"
related_targets: []
---

# Surface: dedetizamed institutional site (Início, Sobre, Serviços, Contato)

**Mode:** Persuade (lead generation via WhatsApp; credibility as supporting objective).

**Audience / job:** (1) residents/businesses in Medianeira-PR with an active pest problem wanting a fast quote; (2) B2B compliance buyers (indústria alimentícia, bares/restaurantes, clínicas, farmácias) evaluating whether this provider can be trusted to issue the laudo técnico they're legally required to have.

**Proof / content on hand:** +20 anos de mercado, licenciada/registrada, garantia de 3 meses, produtos seguros para crianças/pets, emissão de laudo técnico, CNPJ/razão social/endereço confirmados. No real photography yet — hero/team photo slots stay honest placeholders, not disguised as real; no client logos or testimonials exist, so social proof leans on named segments served instead of fabricated quotes.

**Constraints:** HTML/CSS/JS puro, sem framework. Nenhum formulário — todo CTA aponta pro WhatsApp. Maringá nunca é mencionada aqui (só na sua landing page). CNPJ/razão social no rodapé de toda página.

## Redesign (v2) — why

The client rejected the v1 direction ("não gostei") as too cartoonish (large bright-yellow circle badges, bouncy rounded icons) for a pest-control company whose B2B buyers need to trust it with sanitary compliance. They pinned two references as the target register: **dedetizadoraberbert.com.br** and **biotratsaneamentos.com.br** — both established Brazilian pest-control competitors presenting as confident, corporate, credibility-forward operations (dark dominant base, bold accent color used with weight not decoration, real photography, certification badges, years-in-business as a hero-level number, client-logo/testimonial social proof, floating WhatsApp button, compact icon+label rows rather than big illustrated badges).

Per the brief-wins principle, this redesign preserves dedetizamed's own pinned brand commitments (red `#FF0000` / yellow `#FFF000` / charcoal `#323232`, the existing logo, the company's real facts) but replaces the *rendition* — translating the references' corporate-confidence material into dedetizamed's own palette rather than adopting their teal/navy. No real photography exists yet, so the confidence has to come from typography, structure and honest credibility content instead of a photographic hero.

## Direction contract

**THESIS:** dedetizamed reads as an established operator a compliance buyer can trust with a health inspection, not a friendly neighborhood app. Weight and restraint replace bounce and brightness: a near-black base carries the page the way the competitors' dark navy/teal does, red is spent deliberately (CTAs, one bold accent band, thin urgency bar) rather than smeared across icon badges, and yellow drops to a rare accent instead of a repeated shape.

**OWN-WORLD:** Color strategy: Committed, not Full-palette — near-black `#181818` (hero/major sections, replaces the previous everywhere-charcoal with something darker/richer), `#323232` charcoal (secondary dark sections/text), red `#FF0000`/`#E60000` action (CTAs, one full-bleed accent section, thin top urgency bar, arc accent), yellow `#FFF000` demoted to rare small highlights only (a certification-style badge, an underline, never a background fill behind an icon). Display type: **Barlow Condensed** (Black/Bold, uppercase for hero headline) — a confident, slightly industrial condensed grotesk that reads as authority rather than playfulness, the register the references both use for their headlines; body: **Karla** — clean, humanist, unshowy, does not compete with the display face. The dm-logo arc motif survives but is translated from "big colored ring behind every icon" into a single large, low-opacity structural accent (bleeding off a section corner, echoing the competitors' diagonal swoosh without copying it) rather than a repeated per-icon decoration. Icons shrink from big circle badges to small inline glyphs beside their label, chip-style at most (thin border, no fill) — matching the references' compact icon+label rows. Corners stay rounded on buttons/cards (brand continuity) but far less bubbly — smaller radius, no big pill badges except the WhatsApp CTA itself.

**STORY:** The visitor reads the hero and immediately believes this is a real, licensed, 20+-year operator — not a stock landing page — because the page states its proof (license, years, guarantee, laudo) with the same typographic confidence a photo would carry. They scroll through an actual pain section (pragas não esperam), a credibility section (diferenciais), a de-risking "como funciona" walkthrough, a segments-served trust section (no fake logos/quotes), and a residential-vs-business split, never more than one section away from the WhatsApp CTA, plus a floating WhatsApp button that never leaves the viewport.

**FIRST VIEWPORT (Início):** Thin red urgency bar across the very top ("Atendimento imediato pelo WhatsApp"). Below it, a full-bleed near-black hero: large uppercase Barlow Condensed headline stating the core promise, the arc accent bleeding from a bottom corner at low opacity, a red WhatsApp CTA button, and a compact microproof row (4 short items with tiny inline icons, not badges) directly under the CTA — credibility is legible without scrolling.

**FORM:** "Confident local-authority page," reordered and rewritten from the client's own reference copy (adapted to real, non-fabricated facts): thin urgency bar → hero → dor real (pain) → diferenciais (autoridade) → como funciona (steps) → serviços em destaque (cards, icon+heading+description+text-link, not big badges) → segmentos atendidos (trust via named client categories, no invented logos/quotes) → residencial × empresa split → garantia/segurança closing → CTA final → footer with certification-style badges (licenciada, +20 anos, garantia). A floating WhatsApp button persists across the whole site (institutional pages and LPs). Decided directly from the client's pinned references rather than a fresh concept-seed tournament: the brief already named its target register with two concrete, viewable competitor sites, which the brief-wins principle treats as pinned material to translate, not a blank slate to re-roll.

**FINISH:** unreviewed and undocumented is unfinished; this build ends with the finish review, the verdict, DESIGN.md, and every shipping raster carrying its provenance.

## Unresolved decisions

- Whether to eventually source real photography (technician, van, equipment) to replace the typographic hero once the client has material — noted as a fast-follow, not blocking this redesign.
- LP pages inherit this world's palette/type/floating-WhatsApp but keep their own narrower single-purpose composition (still no top nav, still no exit links); the thin urgency bar is skipped on LPs to keep them minimal.
