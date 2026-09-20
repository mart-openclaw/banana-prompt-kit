# Banana Pro AI Image Prompt Playbook (2026)

**A practical guide for creators, marketers, and product teams**

Generate sharper images, edit with conversation, and ship brand-ready assets faster.

**Product:** [Banana Pro AI](https://bananaproai.app/) — AI image generator & photo editor  
**Support:** support@bananaproai.app  
**Companion kit:** `banana-prompt-kit/` (this repository)

---

## Table of Contents

1. [How modern text-to-image prompts work](#1-how-modern-text-to-image-prompts-work)
2. [Prompt formula & anti-patterns](#2-prompt-formula--anti-patterns)
3. [Channel-specific playbooks](#3-channel-specific-playbooks)
4. [Conversational edit recipes](#4-conversational-edit-recipes)
5. [Aspect ratios & export](#5-aspect-ratios--export)
6. [Mini comparison framework](#6-mini-comparison-framework)
7. [20 ready-to-copy prompt examples](#7-20-ready-to-copy-prompt-examples)
8. [End-to-end workflow](#8-end-to-end-workflow)
9. [Resources](#9-resources)

---

## 1. How modern text-to-image prompts work

Modern image models do not “understand” sentences the way a human does. They map language into a visual latent space. The clearer you separate **what** is in the scene from **how** it should look, the more control you get.

### Five building blocks

| Block | Purpose | Example fragments |
|-------|---------|-------------------|
| **Subject** | Who or what is primary | “matte black wireless earbuds in charging case” |
| **Attributes** | Material, color, age, mood, condition | “brushed aluminum, soft cyan LED, dew droplets” |
| **Composition** | Camera, framing, layout | “45° product hero, centered, negative space left for headline” |
| **Style** | Look & feel / medium | “studio product photography, softbox lighting, commercial catalog” |
| **Constraints** | Hard rules & exclusions | “no text overlays, no watermark, pure white background #FFFFFF” |

### Why order and density matter

- Put the **subject first**. Models overweight early tokens.
- Use **concrete nouns and measurable adjectives** (“soft key light from camera-left”) over vague praise (“beautiful, amazing, masterpiece”).
- Prefer **one clear scene** per prompt. Multiple conflicting subjects dilute fidelity.
- Treat style keywords as **direction**, not magic spells. “cinematic” without lighting/lens cues is weak.

### Banana Pro AI strengths to lean on

Banana Pro AI is built for:

- **Text-to-image** with strong subject fidelity  
- **Conversational editing** (iterate without retyping the whole prompt)  
- **2K / 4K** exports for ads and print-adjacent use  
- **Typography in images** when you need readable on-image text  
- **Character consistency** across a set  
- **Multi-reference** guidance when you have product or character refs  

Use references when brand fidelity matters; use conversation when you need surgical fixes (hands, background, copy).

---

## 2. Prompt formula & anti-patterns

### Core formula

```
[Subject + key attributes]
+ [Setting / context]
+ [Composition: angle, framing, depth]
+ [Lighting]
+ [Style / medium]
+ [Color / mood]
+ [Technical: resolution cues, aspect intent]
+ [Constraints / negatives]
```

**Compact template:**

```
[SUBJECT], [2–4 attributes], [setting],
shot as [composition], [lighting],
in the style of [style], [mood/palette],
[constraints].
```

### Worked example (e-commerce)

```
Matte ceramic pour-over coffee dripper in charcoal gray, single piece,
on a light oak cutting board with scattered coffee beans,
45-degree hero angle, shallow depth of field, soft window light from left,
commercial product photography, neutral warm palette,
pure seamless background, no logos, no text, no hands.
```

### Anti-patterns (and fixes)

| Anti-pattern | Why it fails | Fix |
|--------------|--------------|-----|
| Keyword stuffing (“8k uhd masterpiece best quality …”) | Noise; little composition signal | Replace with camera, light, and layout cues |
| Conflicting styles (“anime + photoreal + oil paint”) | Model averages into mush | Pick one primary style; add one accent max |
| Invisible subject (“a vibe of luxury”) | No renderable noun | Name the object and materials |
| Unspecified text (“add catchy headline”) | Glyphs invent themselves | Quote exact words + font mood + placement |
| Overlong novels | Dilutes priority | ≤ ~60–120 words; move edits to conversation |
| No constraints | Extra limbs, watermarks, clutter | Explicit negatives / “clean background” |
| Skipping aspect intent | Awkward crop later | State use case or ratio early |

### Positive vs. conversational strategy

1. **Generate** with a strong first prompt (formula above).  
2. **Edit** with short conversational instructions (“move product 10% left”, “replace background with soft gradient”).  
3. Avoid regenerating from scratch for small fixes—you lose consistency.

---

## 3. Channel-specific playbooks

### 3.1 E-commerce product

**Goal:** Trust, clarity, convert.

- Hero angle + true materials  
- Controlled reflections; avoid fake chrome  
- Leave safe margin for price badges if needed  
- Prefer 1:1 or 4:5 for marketplace grids  

**Prompt skeleton:**

```
[Product full name], [material/finish], [hero angle],
studio softbox lighting, accurate color, commercial catalog photo,
[background: pure white OR lifestyle surface],
no props unless brand-relevant, no text, no watermark.
```

### 3.2 YouTube thumbnail

**Goal:** Stop the scroll in ~0.3s.

- One dominant face or object + high contrast  
- Readable 3–5 word title baked in (or plan overlay in editor)  
- Exaggerated emotion / clear stakes  
- 16:9, faces large, avoid fine detail that dies at small size  

**Prompt skeleton:**

```
Close-up of [creator/character] with [clear emotion],
high-contrast [background color], dramatic key light,
YouTube thumbnail composition, large negative space for title on right,
bold simple shapes, sharp focus on eyes, 16:9.
Text on image: "[EXACT TITLE]" in bold sans-serif, high contrast.
```

### 3.3 Social ad (Meta / TikTok / LinkedIn)

**Goal:** Message + product in one glance.

- Product + benefit visual metaphor  
- Native aspect: 1:1 feed, 9:16 stories/reels  
- Minimal clutter; brand color accent  
- If text-in-image: short claim, high contrast  

### 3.4 Character sheet

**Goal:** Consistency across poses and scenes.

- Lock: age, hair, outfit, distinguishing marks  
- Neutral lighting for “turnaround” sheets  
- Same camera height across views  
- Use multi-reference / character lock features when available  

**Prompt skeleton:**

```
Character design sheet of [name/description], [age], [hair], [outfit],
front view, three-quarter view, side view, on clean white background,
consistent proportions, concept art, even studio lighting, no text.
```

### 3.5 Educational diagram

**Goal:** Clarity over spectacle.

- Flat or isometric; labeled regions  
- Limited palette (3–5 colors)  
- Explicit label strings in quotes  
- Prefer simple shapes over photoreal noise  

---

## 4. Conversational edit recipes

After the first generation, talk to the model like a retoucher.

| Problem | Say something like |
|---------|-------------------|
| Broken hands / fingers | “Fix the hands: five fingers each, natural pose, matching the existing lighting.” |
| Garbled on-image text | “Replace the headline text with exactly: ‘SHIP FREE TODAY’. Keep bold white sans-serif, same position.” |
| Busy / wrong background | “Remove clutter. Soft gradient background in brand blue #0B3D91 to white. Keep subject unchanged.” |
| Flat lighting | “Add soft key light from camera-left and gentle rim light; preserve product colors.” |
| Crop too tight | “Zoom out 20%, keep subject centered, more margin on all sides.” |
| Color drift | “Match product color to reference: charcoal gray #36454F, reduce blue cast.” |
| Extra objects | “Remove the second bottle and the plant. Keep only the hero product.” |
| Face inconsistency | “Keep the same face and hairstyle as the reference; only change the expression to a slight smile.” |
| Soft / muddy detail | “Increase micro-contrast on product edges; keep skin (or fabric) natural, no oversharpen halo.” |
| Wrong aspect feel | “Reframe for 9:16 vertical: subject in upper third, clean space below for CTA.” |

**Rules of thumb**

- One change per message when possible.  
- Quote exact strings for typography.  
- Reference hex colors and brand terms.  
- Say what to **keep** as well as what to change.

---

## 5. Aspect ratios & export

| Ratio | Typical use | Notes |
|-------|-------------|-------|
| **1:1** | Instagram feed, marketplace tiles, avatars | Safest default for catalogs |
| **4:5** | IG portrait feed | Slightly more vertical real estate |
| **16:9** | YouTube, presentations, blog heroes | Thumbnails & headers |
| **9:16** | Stories, Reels, TikTok, Shorts | Face/product in upper third |
| **3:2 / 2:3** | Editorial, print-adjacent | Check bleed if printing |
| **21:9** | Ultra-wide banners | Keep subject away from extreme edges |

### Resolution guidance

| Label | Approx. | Use when |
|-------|---------|----------|
| **2K** | ~2048px on long edge | Social ads, web heroes, most marketing |
| **4K** | ~3840px on long edge | Large banners, detail crops, print-ish proofs |

**Export checklist**

1. Confirm ratio matches channel.  
2. Export 2K for draft review; 4K for final paid placements when detail matters.  
3. Keep a lossless or high-quality master; compress derivatives per platform.  
4. Strip accidental watermarks; verify text spelling at 100% zoom.  
5. Run a brand check: logo clearspace, palette, prohibited claims.

---

## 6. Mini comparison framework

When evaluating any AI image tool (including Banana Pro AI), score **your** workflows—not hype lists.

| Criterion | What “good” looks like | Questions to ask |
|-----------|------------------------|------------------|
| **Subject fidelity** | Product/character matches brief | Can it keep SKU color and shape? |
| **Edit loop** | Conversational or localized edits | Do small fixes require full regen? |
| **Typography** | Readable short headlines | Can you lock exact strings? |
| **Consistency** | Same character/product across a set | Multi-ref or seed/character lock? |
| **Resolution** | Usable 2K/4K | Soft when upscaled? |
| **Speed / cost** | Fits production cadence | Latency under deadline pressure? |
| **Commercial terms** | Rights clear for ads | What does the ToS allow? |
| **Safety / brand** | Controllable refusals & audits | Can you enforce brand negatives? |

Use a 1–5 score per criterion for 2–3 candidate tools on the **same five briefs**. Prefer evidence over affiliate roundups.

---

## 7. 20 ready-to-copy prompt examples

Copy, swap bracketed variables, then iterate with conversation.

### E-commerce (1–4)

**1. Clean packshot**
```
[Product]: frosted glass serum bottle 30ml with white pump, label area blank,
centered on pure white seamless background, soft dual softbox, subtle contact shadow,
commercial beauty product photo, accurate frosted texture, no text, no hand, no logo.
```

**2. Lifestyle kitchen**
```
Stainless steel chef’s knife with black pakkawood handle on marble counter,
shallow depth of field, morning window light, lifestyle product photography,
herbs softly blurred in background, appetizing but uncluttered, no people.
```

**3. Apparel ghost mannequin feel**
```
Navy merino wool crewneck sweater, invisible mannequin product shot,
even studio lighting, true navy color, fabric knit detail visible,
light gray background, e-commerce catalog style, no hanger, no model head.
```

**4. Electronics desk setup**
```
Compact USB-C hub in space gray aluminum on a tidy walnut desk,
top-down 30-degree angle, soft daylight, cable tips neatly arranged,
tech product photography, minimal Scandinavian workspace, no screens on.
```

### YouTube / thumbnails (5–8)

**5. Shock-value face thumbnail**
```
Close-up of a surprised creator facing camera, raised eyebrows, mouth open,
bright yellow background, high contrast, YouTube thumbnail style, 16:9,
large empty space on the right for title text, sharp eyes, dramatic rim light.
Text: "I WAS WRONG" in huge bold white letters with thick black outline.
```

**6. Before/after split**
```
Split-screen thumbnail: left dull messy desk labeled feel, right bright organized desk,
bold center divider, high saturation on the right, 16:9 YouTube thumbnail,
clear visual contrast, space at top for short title.
Text: "FIX YOUR DESK" bold sans-serif top center.
```

**7. Tutorial object focus**
```
Macro shot of hands holding a vintage film camera, instructional vibe,
clean teal backdrop, bright even light, 16:9, subject left-third,
room for text on right, educational YouTube thumbnail, no busy patterns.
Text: "START HERE" in bold cream letters.
```

**8. Gaming energy**
```
Dynamic 3/4 view of a stylized armored game character mid-stride,
neon cyan and magenta rim lights, dark moody background, 16:9 thumbnail,
exaggerated perspective, high clarity silhouette, space upper-left for title.
Text: "NEW BOSS" bold condensed font, high contrast.
```

### Social ads (9–12)

**9. Feed ad — product + claim**
```
Hero shot of reusable stainless water bottle in matte sage green,
soft gradient background sage-to-cream, centered, Instagram ad 1:1,
gentle shadow, premium eco brand feel, room above bottle for headline.
Text: "Hydration, simplified." elegant sans-serif, dark gray.
```

**10. Story / Reel vertical**
```
9:16 vertical ad: skincare dropper bottle in foreground, soft bokeh bathroom,
subject in upper third, creamy light, Gen-Z clean aesthetic,
large lower third empty for swipe CTA, no tiny text.
Text near top: "Glow in 7 days" bold.
```

**11. LinkedIn B2B**
```
Clean isometric illustration of a secure cloud dashboard on a laptop,
soft blue corporate palette, ample whitespace, LinkedIn ad 1.91:1 feel cropped to 16:9,
professional, no cartoon mascots, subtle geometric accents.
Text: "Audit-ready in one click."
```

**12. Flash sale energy**
```
Top-down flat lay of sneaker, shopping bag, and stopwatch on bold red paper,
hard sunlight shadow, high energy sale creative, 1:1,
simple geometric composition, strong focal sneaker.
Text: "48:00:00 LEFT" in bold white with black shadow.
```

### Characters (13–16)

**13. Consistent brand mascot**
```
Friendly fox mascot in a small blue scarf, flat vector-inspired 3D, soft rounded shapes,
centered character turnaround on white, consistent eye style, children's brand mascot,
even lighting, no text, high clarity outline.
```

**14. App game protagonist**
```
Young explorer with copper short hair, teal jacket, leather satchel, determined smile,
full-body character concept, neutral gray background, game art, consistent proportions,
front view, soft studio light, no weapons, no text.
```

**15. Podcast host caricature**
```
Stylized semi-realistic portrait of a podcast host with round glasses and coily hair,
warm key light, subtle studio mic in frame, square composition, friendly approachable mood,
limited background blur, podcast cover art vibe.
```

**16. Multi-outfit lock**
```
Same female character, mid-20s, silver bob haircut, light freckles, calm expression,
outfit variation sheet: casual tee, winter coat, formal blazer, white background,
identical face and hair across three panels, fashion character sheet.
```

### Educational / diagrams (17–20)

**17. Process diagram**
```
Flat educational diagram of a 4-step coffee brewing process, numbered 1–4 left to right,
simple icons, pastel palette, large readable labels, white background, infographic style.
Labels exactly: "Grind", "Bloom", "Pour", "Serve".
```

**18. Labeled anatomy-style (non-medical product)**
```
Exploded-view diagram of a mechanical pencil, parts separated with thin leader lines,
clean technical illustration, white background, muted blue accents, textbook clarity.
Labels: "Tip", "Lead", "Grip", "Eraser".
```

**19. Comparison cards**
```
Side-by-side comparison cards: "Draft" vs "Final", left grayscale messy sketch,
right colorful polished UI mockup, flat design infographic, 16:9, clear headers,
minimal icons, high readability for slides.
```

**20. Map-style conceptual**
```
Simplified isometric map of a customer journey: Awareness → Consideration → Purchase → Loyalty,
soft pastel tiles, arrows between stages, presentation diagram, generous spacing, no tiny text.
Stage labels exactly as written above.
```

---

## 8. End-to-end workflow

```
Brief → Generate → Iterate → Brand check → Export
```

### Step-by-step

1. **Brief (5–10 min)**  
   Audience, channel, ratio, must-have objects, forbidden elements, exact on-image copy, brand colors (hex).

2. **Generate**  
   One strong prompt using the formula. Generate 2–4 variations if the tool allows; pick a base.

3. **Iterate (conversation)**  
   Surgical edits: hands, text, background, lighting, crop. One request at a time. Lock what already works.

4. **Brand check**  
   - Spelling of on-image text  
   - Color vs. brand hex  
   - Logo clearspace / no fake logos  
   - Claims compliant  
   - No artifacts at 100% zoom  

5. **Export**  
   Correct ratio → 2K review → 4K final if needed → platform-compressed derivatives → archive prompt + seed/ref notes in your kit.

### Team tip

Store winning prompts in `banana-prompt-kit/prompts/` with variables documented. Treat prompts like ad copy: version them.

---

## 9. Resources

| Resource | Link / path |
|----------|-------------|
| **Banana Pro AI** (app) | https://bananaproai.app/ |
| **Support** | support@bananaproai.app |
| **This playbook (PDF)** | `banana-pro-ai-image-prompt-playbook.pdf` |
| **GitHub kit** | `banana-prompt-kit/` — README, `docs/playbook.md`, `prompts/*`, `examples/` |
| **Prompt packs** | `prompts/ecommerce.md`, `thumbnails.md`, `characters.md`, `ads-social.md`, `negatives.md` |
| **Iteration notes** | `examples/before-after-notes.md` |

### About Banana Pro AI

Banana Pro AI is an AI image generator and photo editor for creators and marketers: text-to-image, conversational editing, 2K/4K output, typography in images, character consistency, and multi-reference workflows.

---

*© 2026 Banana Pro AI playbook for educational distribution. Product names are for identification. Always verify commercial usage rights in the product Terms.*

*Generated for SEO & creator education — bananaproai.app*
