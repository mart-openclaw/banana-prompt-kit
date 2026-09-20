# Negatives, constraints & anti-patterns

Constraints are not an afterthought—they are how you keep marketplace compliance, brand safety, and anatomy under control.  
Use these as **suffix blocks** on prompts, or as conversational follow-ups in [Banana Pro AI](https://bananaproai.app/).

---

## Universal clean-product block

Append when you need a catalog-safe image:

```
Constraints: no watermark, no logo, no readable brand marks, no extra products,
no hands unless requested, no text overlays, no QR codes, no frames or borders,
no mannequin seams, pure seamless background as specified, accurate anatomy if people present.
```

---

## Marketplace / pure-white block

```
Constraints: pure white background #FFFFFF, no props, no drop shadows beyond a soft
contact shadow, no reflective floor, no lifestyle elements, no people, no animals,
product fully visible, no cropped edges, no glare covering labels.
```

---

## Typography-safe block

When you *do* want on-image text:

```
Constraints: render ONLY this exact text: "[YOUR COPY]"; no extra words, no misspellings,
no random glyphs, no lorem ipsum, high contrast against background, single font style
as specified, no watermark.
```

When you *do not* want text:

```
Constraints: no text, no letters, no numbers, no captions, no subtitles, no watermarks,
no signatures, no UI chrome.
```

---

## People / anatomy block

```
Constraints: natural adult anatomy, five fingers per hand, correct ear count,
no melted facial features, no extra limbs, no distorted eyes, age clearly adult 25–40
unless another age is specified, no celebrity lookalikes, no real private individuals.
```

---

## Character consistency block

```
Constraints: keep the same face, hair, eye color, and outfit as the reference;
do not change identity; do not add accessories; do not age or de-age the character;
no duplicate characters in frame unless requested.
```

---

## Brand-safety block (ads)

```
Constraints: no violence, no weapons, no hate symbols, no medical claims visuals,
no before/after body-shaming imagery, no shock gore, no political candidate likenesses,
no misleading UI that imitates system alerts, no fake review stars with invented numbers.
```

---

## Lighting / quality block (without keyword spam)

Prefer this over “8k uhd masterpiece best quality”:

```
Constraints: avoid muddy contrast, avoid oversharpen halos, avoid plastic skin,
avoid chromatic aberration, keep materials physically plausible, no heavy noise,
no artificial vignette unless requested.
```

---

## Anti-patterns library

| Don’t write | Write instead |
|-------------|---------------|
| `masterpiece, best quality, 8k, uhd, trending on artstation` | Softbox lighting, 45° hero, commercial catalog photo |
| `beautiful luxury vibe` | Brushed brass tray, marble surface, warm key light |
| `add some cool text` | Text exactly: “FREE SHIPPING” bold white sans, top-right |
| `anime photoreal oil paint` | Pick one: “clean product photo” *or* “anime cel shading” |
| `person like [celebrity]` | Original adult description + wardrobe; no lookalike |
| Endless paragraph of 200+ words | ≤ ~120 words; move fixes to conversation |

---

## Conversational negative recipes

Use after a first image—often more reliable than stuffing everything into prompt #1:

| Issue | Follow-up |
|-------|-----------|
| Extra object | “Remove the [object]. Keep everything else identical.” |
| Wrong bg | “Replace background with pure white #FFFFFF. Keep product unchanged.” |
| Fake logo | “Remove all logos and lettering from the product. Leave a blank label band.” |
| Bad hand | “Fix hands: five fingers, natural grip, match existing light.” |
| Oversharpen | “Reduce crunchy sharpening; keep natural material texture.” |
| Color cast | “Neutralize green cast; match product to hex [#……].” |
| Cropped product | “Zoom out 15% so the entire product is inside the frame with margin.” |
| Duplicate subject | “Keep only one [subject]; delete the duplicate.” |

---

## Channel quick-append cheats

**E-commerce**
```
…, commercial catalog photo, no text, no watermark, no props, accurate color.
```

**Thumbnail**
```
…, 16:9 YouTube thumbnail, high contrast, large title space, no tiny details,
text exactly: "[TITLE]".
```

**Character sheet**
```
…, clean white background, even lighting, consistent proportions, no text, no props.
```

**Social ad**
```
…, [1:1 or 9:16], room for headline, no fake logos, text exactly: "[CLAIM]".
```

---

## Versioning tip

Save constraint blocks as snippets (`neg-white.md`, `neg-anatomy.md`) and compose:

`[base prompt] + [channel block] + [safety block]`

That keeps the creative half readable and the compliance half reusable.
