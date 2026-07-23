# Audit checklist — the GATE (run on every slide before delivering; the rubric in review)

A slide passes only when **every** box holds. Report a failure as: **element → what's wrong → fix**,
citing the rule. These map 1:1 to the hard rules in `SKILL.md`. No exceptions, no "close enough."

> **Cover slide?** Audit it by **§8 only**. The cover is exempt from §0 (compose-fresh), §2
> (density / fill-frame), the no-photo clause of §4, and the rail / `Source:` / anchor-every-cell items —
> see SKILL.md **THE COVER**. §1 typography, §3 signal & color, and §4 flatness (square corners, ivory
> ground, no shadow/gradient/glow) **still apply** to the cover. §7's icon allowance does **not** extend
> to the cover — the cover carries **zero icons** (§8 checks it).

## 0. Compose-fresh (Rule 0)
- [ ] Slide was **built fresh** from `assets/tokens.css` primitives — not copied from a prior slide.
- [ ] No demo/residue labels carried over (residue test: every label fits THIS subject).
- [ ] `assets/tokens.css` is **inlined**; tokens not redefined or altered per slide.

## 1. Typography
- [ ] **Montserrat only** — one family; hierarchy from weight + size + color, no 2nd typeface.
- [ ] Only the **3–4 sizes** in the scale: title 30px · body 15px · value 14px · label 12px · source 11px.
- [ ] **Title** is light (300–400), navy/ink, sentence/entity case, **not big-and-bold, not centered**.
- [ ] **Header is ONE title on ONE line** — a single title element, **no wrapping**: a very short
      summary sentence of the slide (shorten until it fits one line); **no eyebrow above, no
      subtitle/definer below**; framing/scope info lives in content cells, not the header.
- [ ] Body 15px/400; **bold spine** is 700 in the SAME ink (emphasis = weight, never color).
- [ ] Keys/chips/tags 12px/600 UPPERCASE; source 11px/400 **italic** muted.
- [ ] **Metric number** 600, **navy**, **≤ title size (never above)**, never black, never on a colored chip.
- [ ] Case discipline: sentence-case default; Title Case only proper nouns; ALL-CAPS only labels/tags;
      italic only cited titles; acronyms expanded-then-`(PARENTHESIZED)` on first use.
- [ ] No type shadows/outlines/wide tracking.

## 2. Format & density
- [ ] Slide is a **dense bounded-cell fact-card**: title + label gutters/keystrips + bounded panels +
      right rail of key→value fields + source foot.
- [ ] **Frame filled** at fact-card density; content zones flex to occupy full height — **no empty/dead
      space** (verify by render: bottom-ink near row ~678/720).
- [ ] Every region is a **bounded cell** (faint `--panel` fill or `--hair` hairline).
- [ ] **Nothing overflows** 1280×720; rows/cells capped and sized to fit.
- [ ] Arrangement varies by job; it is still a **fact-card grid** (not a divergent/sparse layout).
- [ ] **No floating label-as-heading** — labels sit in bounded gray cells.

## 3. Signal & color (one signal = one meaning)
- [ ] navy=structure/ink · gray=secondary/inactive · muted=tertiary.
- [ ] **teal `#2F8F86` = ACTIVE only** (current/selected/best/positive); used for nothing else.
- [ ] **gold `#A9853F`** = caveat / link / 2px accent rule / scope tag only.
- [ ] **≤ one teal element per comparison axis** (one row-winner, one current node).
- [ ] **No red/amber/green** anywhere — a decline is gray ▼; "at risk" is a small **gold tag**.
- [ ] No signal reused for a 2nd job; no color-for-emphasis; no gold "premium" wash.

## 4. Flatness
- [ ] Flat throughout: ivory ground, **square corners**, edges from hairlines/fills only.
- [ ] **No** shadow / gradient / glow / photo *(content slides; the cover's one photo is §8)* / rounded
      marketing pill / icon rainbow *(sparing monochrome Lucide icons are the ONE sanctioned form — §7)*
      / 3D.
- [ ] Ground is `#FAFBFC` — **never pure `#FFFFFF`**.
- [ ] **No rule/border beneath the title.**
- [ ] No metric number on a colored chip or above title size (no KPI-dashboard look).

## 5. Credibility & honesty (anchor-or-cut)
- [ ] **Every** cell/value/figure anchored to a date, a fully-named authority `(ACRONYM)`, or an
      *italic* dated document title. No "experts say / recently / bare logo".
- [ ] Exactly **one** quiet italic muted `Source:` foot, bottom-left; links **underline-only** (no blue,
      no raw URL, no "various/internal").
- [ ] Parallel units identical (same template, equal counts, matched phrasing) — they compare like-for-like.
- [ ] **No N/A / — / TBD**, no invented values, no filler padding — schema bent to the data.

## 6. Reading & scope
- [ ] Works at three speeds: **title → bold-only skim → full detail**; every region labeled.
- [ ] **One slide, one job** (not two subjects/arguments — else split it).
- [ ] **Deck at minimum length** — every slide has a distinct job; no agenda / section-divider / quote /
      recap / thank-you filler; no two slides whose jobs one dense fact-card could carry.
- [ ] Reading order supports random access; the bold spine alone reconstructs the gist.

## 7. Icons (slight & functional — content slides ONLY; see SKILL.md **Icons**)
- [ ] **Lucide stroke icons only**, written `<i data-lucide="name" class="icon"></i>` with the Lucide CDN
      script; every name shows a **rendered glyph** in the screenshot (a bad name renders an empty gap —
      fix and re-render).
- [ ] **Monochrome `currentColor`** — each icon wears its cell's text color; teal/gold only when the cell
      itself carries that signal. No multicolor/filled blobs, no emoji, no second icon set.
- [ ] Every icon sits **beside the text label it reinforces** — none floats as decoration, none replaces
      words, none parked in a corner.
- [ ] **Icons present: typically 2–4 on this content slide** (≥ 1 always); **≤ 1 per labeled region,
      ≤ 6 per slide**; same concept = same icon deck-wide; no two icons for one concept.
- [ ] **Icons legible at a glance** in the render (~17px beside a 12px label via `.icon`) — no specks
      you must hunt for.

## 8. Cover slide (apply ONLY to the deck cover — see SKILL.md **THE COVER**)
- [ ] Started from **`assets/cover.html`**; only the **title, date, and image** slots were changed.
- [ ] **Title** navy/ink, **light 300**, left-aligned, sentence/entity case, **at title size** — not
      enlarged, centered, or recolored (**no gold title**); **no rule beneath it.**
- [ ] **Gold appears ONLY as the two 2px frame bars** — nowhere else on the slide.
- [ ] **Zero icons** anywhere on the cover (the §7 allowance is content-slides-only).
- [ ] Left text column is ivory `#FAFBFC` (**never pure white**); exactly **one** bounded photo; **square
      corners**; no shadow / gradient / glow.
- [ ] **Date** is a real, honest date (no TBD / placeholder); **one slide, one job** (deck title only).
- [ ] **Image:** the user was **asked** for one. If provided, it's embedded **raw**; if not, the image
      column is a flat **`--navy`** panel (the navy fallback) — never invented/off-topic filler. (Online or
      AI-generated images only on the user's explicit request; see SKILL.md sourcing process.)
- [ ] Renders exactly **1280×720**; the photo **bleeds to its edges**; nothing overflows the frame.

## §9 V2 additions (user-added rules — gate every slide on these too)
- [ ] **Palette**: default palette unless the user NAMED an optional palette (e.g. ODA). Under ODA:
      locked hexes only, no invented grays/tints, no brown (`#815B3B`), no dark icon fills —
      icon tiles are blue with white icons; white ground is allowed.
- [ ] **One font**: Montserrat everywhere, including titles and covers. No serif, no second family.
      NEVER Thin or Light (100-300): minimum weight Regular 400, titles included; no light weights
      in the font link; PPTX exports must resolve static weights, not a variable-font Thin instance.
- [ ] **No em-dashes** anywhere in copy (colon/semicolon/comma instead); en-dashes only in ranges.
- [ ] **Facts only**: every claim sourced; source opinions are excluded-and-flagged or explicitly
      attributed; the deck's own classifications are labeled as such on the slide.
- [ ] **Layout choice**: bounded-cell fact-card by default; the airy hairline row variant is used
      ONLY when the slide has too many items to avoid looking boxy — and then the slide's defining
      criteria sit in one distinct header band under the title, not in a peer cell.
- [ ] **Logos**: real vendor logos only on entity/profile content, each visually verified as the
      right company; unverifiable/generic items get a palette icon tile — never a guessed logo.
- [ ] **Icons**: cap relaxed on list/profile slides, but still monochrome, label-adjacent,
      same concept = same icon, legible in the render.
- [ ] **Profile cards**: 2x2 grid; logo + name + CATEGORY · HQ subline; filled category pill +
      outline ownership pill; one-line description; STRENGTHS / PROJECTS / BEST FOR panels;
      gold disclaimer strip for caveats; odd counts filled with an attributed REPORT NOTE card.
- [ ] **Foot**: upright 11px darkest-ink source line, minimized, page number far right (none on covers).
- [ ] **Deliverables**: HTML + merged PDF always (render-verified); native shape-level PPTX when an
      editable deck is requested, verified via LibreOffice conversion before delivery.
