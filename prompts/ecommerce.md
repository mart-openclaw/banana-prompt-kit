# E-commerce prompts

High-fidelity product imagery for marketplaces, DTC sites, and catalogs.  
**Recommended ratios:** 1:1 or 4:5 · **Export:** 2K review → 4K final when zoom/detail matters  
**Tool:** [Banana Pro AI](https://bananaproai.app/)

Variables to swap are in `[BRACKETS]`. After generation, use conversational edits for color match and cleanup (see `../examples/before-after-notes.md`).

---

## 1. Pure white packshot (beauty / CPG)

```
[PRODUCT: frosted glass serum bottle 30ml with white pump], label area blank,
centered on pure white seamless background (#FFFFFF), soft dual softbox lighting,
subtle contact shadow directly under base, commercial beauty product photo,
accurate [MATERIAL: frosted glass] texture, true-to-life color, no text, no hand,
no logo, no reflection of photographer, square 1:1 composition with safe margin.
```

**Why it works:** Subject-first + material cue + lighting + hard constraints. Blank label avoids invented brand marks.  
**Swap:** product name, material, bottle size, add “subtle logo only if provided in reference.”

---

## 2. Soft shadow packshot (electronics)

```
[PRODUCT: compact USB-C hub in space-gray aluminum], angled 30 degrees hero view,
pure light-gray seamless (#F2F2F2), softbox key from camera-left, gentle fill,
crisp edge definition on ports, commercial tech catalog photo, accurate metal finish,
no cables unless specified, no text, no watermark, 1:1.
```

**Why it works:** Angle + finish accuracy matters more than “8K” adjectives. Gray seamless reads premium vs pure white for metal.  
**Swap:** product, finish color hex, angle (top-down vs 45°).

---

## 3. Lifestyle kitchen (food / housewares)

```
[PRODUCT: stainless steel chef’s knife with black pakkawood handle] resting on
[SURFACE: white marble counter], shallow depth of field, morning window light from left,
lifestyle product photography, [PROPS: soft-focus herbs] in background only,
appetizing but uncluttered, no people, no logos, natural color, 4:5 portrait crop.
```

**Why it works:** One hero + controlled props + light direction. Avoids busy flat-lays that bury the SKU.  
**Swap:** product, surface, one prop max, ratio.

---

## 4. Apparel — invisible mannequin feel

```
[GARMENT: navy merino wool crewneck sweater], invisible mannequin / ghost mannequin
product shot, even studio lighting, true [COLOR: navy #001F3F], visible knit texture,
light gray background, e-commerce catalog style, sleeves natural drape, no hanger,
no model head, no mannequin seams, 1:1.
```

**Why it works:** Color hex + fabric detail + ghost-mannequin convention = marketplace-ready.  
**Swap:** garment, hex, background (white vs gray).

---

## 5. Footwear three-quarter hero

```
Single [PRODUCT: white leather low-top sneaker] on seamless light studio floor,
three-quarter front hero angle, soft overhead softbox with gentle rim,
accurate stitching and sole tread, commercial footwear photo, slight reflection
on floor (10% opacity feel), no props, no socks, no text, 1:1.
```

**Why it works:** Classic shoe angle buyers expect; constrained reflection prevents chrome chaos.  
**Swap:** shoe model, colorway, floor tone.

---

## 6. Jewelry macro on stone

```
Macro product photo of [PRODUCT: 14k gold thin hoop earrings], resting on
[SURFACE: raw beige stone], soft diffused daylight, shallow DOF with sharp metal highlights,
luxury jewelry catalog style, warm neutral palette, no hands, no model, no text, 1:1.
```

**Why it works:** Macro + luxury surface cues scale; “no hands” prevents anatomy artifacts.  
**Swap:** jewelry type, metal, surface.

---

## 7. Multi-SKU group (same family)

```
Family packshot: [COUNT: three] [PRODUCT LINE: matte ceramic mugs] in [COLORS: cream, sand, charcoal],
arranged in a gentle arc on pure white, even softbox lighting, equal scale,
commercial catalog group shot, consistent style across items, subtle contact shadows,
no text, no props, 1:1.
```

**Why it works:** Explicit count + equal scale reduces “extra mug” hallucinations.  
**Swap:** count, products, colors; for consistency, attach multi-reference of each SKU.

---

## 8. Subscription box unboxing flat-lay

```
Top-down flat lay of [BOX BRAND STYLE: kraft subscription box] opened with tissue,
contents: [ITEMS: candle, matchbox, card], neat geometric arrangement on linen,
soft overhead daylight, cozy DTC unboxing aesthetic, muted warm palette,
space at top for later badge overlay, no readable fake logos, 1:1.
```

**Why it works:** Named contents prevent random clutter; “no fake logos” is critical for packaging.  
**Swap:** items list, fabric, palette.

---

## 9. Furniture room vignette

```
[PRODUCT: oak mid-century side table] in a bright minimal living room corner,
natural window light, Scandinavian interior photography, soft neutral walls,
one plant in background for scale, product sharp and primary, no people,
true wood grain, 4:5, commercial furniture lifestyle.
```

**Why it works:** Context sells furniture better than pure white; one plant = scale without chaos.  
**Swap:** furniture, interior style, plant on/off.

---

## 10. Color-accurate food pack (jar / pouch)

```
[PRODUCT: glass jar of tomato sauce with blank label band], 45-degree hero,
pure white background, softbox lighting optimized for glass and liquid accuracy,
true red sauce color, commercial CPG photo, condensation optional but light,
no hand, no spoon, no text glyphs, 1:1.
```

**Why it works:** Food color drift is a top failure mode—call out “true” color + glass handling.  
**Swap:** food product, liquid/solid, condensation.

---

## 11. Detailing / texture crop (secondary image)

```
Extreme detail crop of [MATERIAL REGION: woven wool fabric of overcoat],
angled raking light to show texture, soft gradient background, material swatch
photography for PDP zoom, no full garment, no mannequin, accurate color [HEX],
commercial textile photo, 1:1.
```

**Why it works:** PDPs need texture shots; framing as “swatch” avoids weird half-body crops.  
**Swap:** material region, hex.

---

## 12. “In hand” scale shot (careful)

```
[PRODUCT: 500ml matte black water bottle] held by one adult hand for scale,
clean manicure, neutral sleeve cuff, soft studio light, light gray background,
e-commerce scale reference photo, natural hand anatomy, five fingers visible,
product label area blank, no extra jewelry, 1:1.
```

**Why it works:** Hands are hard—explicit anatomy constraints + “one hand” reduce extras. Prefer conversational fix if fingers break.  
**Swap:** product, hand/skin tone guidance, cuff color.

---

## Tips for this channel

- Match **marketplace background rules** (Amazon-style pure white vs lifestyle).  
- Use **multi-reference** when SKU color must match a photo.  
- Put **exact hex** in the prompt *and* verify in conversation (“reduce blue cast”).  
- Keep on-image text out of packshots; add price badges in your design tool.
