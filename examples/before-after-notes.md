# Before / after iteration notes

Text-only case studies showing how a weak first prompt becomes a shippable asset via **conversational edits** in [Banana Pro AI](https://bananaproai.app/).  
No images embedded—focus is on the language you type.

---

## Case A — E-commerce serum bottle

### Before (weak prompt)

```
beautiful luxury skincare bottle, masterpiece, 8k, aesthetic, glowing
```

**Result (typical failure):** Invented gold logos, pink neon fog, bottle shape unstable, text gibberish on label, unusable for PDP.

### After (structured prompt)

```
Frosted glass serum bottle 30ml with white pump, blank label band, centered on
pure white seamless background, soft dual softbox, subtle contact shadow,
commercial beauty product photo, accurate frosted texture, no text, no hand, no logo, 1:1.
```

### Conversational edits (in order)

1. “Reduce blue color cast on the glass; keep frost opacity.”  
2. “Make the contact shadow softer and closer to the bottle base.”  
3. “Zoom out 10% for marketplace safe margin.”  

### Lesson

Keyword flattery ≠ product fidelity. Subject + material + lighting + constraints wins. Conversation handles micro color/crop.

---

## Case B — YouTube thumbnail text

### Before

```
excited guy pointing at something crazy for youtube
```

**Result:** Face OK-ish, but random glyphs where a title should be; low contrast bg; subject centered with no room for type.

### After

```
Close-up of a surprised creator facing camera, raised eyebrows, mouth open,
bright yellow background, high contrast, YouTube thumbnail, 16:9,
large empty space on the RIGHT for title, sharp eyes, dramatic rim light.
Text: "I WAS WRONG" in huge bold white letters with thick black outline.
```

### Conversational edits

1. “Replace all on-image text with exactly: I WAS WRONG. Same position, thicker outline.”  
2. “Push the face 10% more to the left; keep yellow background.”  
3. “Increase contrast on the eyes only; don’t darken the whole image.”  

### Lesson

Quote exact strings. Reserve negative space in the first prompt so edits don’t fight the crop.

---

## Case C — Character drift across scenes

### Before

```
cool anime girl in a city, then later: same girl in a forest
```

**Result:** Different face, hair length, and outfit each time—“same girl” was never specified.

### After (identity lock string)

```
Young woman, mid-20s, silver bob haircut, light freckles, hazel eyes, teal jacket,
calm expression — [reuse this exact clause every time]
```

Scene 1: `… standing in neon city street, night, 16:9`  
Scene 2: `… standing in sunlit forest path, morning, 16:9` + multi-reference to scene 1  

### Conversational edits

1. “Keep the same face and silver bob; only change the background to forest.”  
2. “Remove the extra scarf that appeared; outfit must stay teal jacket only.”  

### Lesson

Paste the **verbatim** identity clause. Change one variable per step. Multi-reference beats hope.

---

## Case D — Social ad claim compliance

### Before

```
skincare bottle that cures acne instantly, miracle glow
```

**Result:** Over-claim risk + medical implication + chaotic sparkles.

### After

```
9:16 vertical ad: skincare dropper bottle in foreground, soft bokeh bathroom,
subject in upper third, creamy light, clean aesthetic, lower third empty for CTA.
Text near top: "Glow in 7 days" bold. No medical imagery, no before/after skin disease photos.
```

### Conversational edits

1. “Remove sparkles and lens flares.”  
2. “Ensure text reads exactly: Glow in 7 days — no extra words.”  
3. “Leave lower third empty and clean for our swipe CTA.”  

### Lesson

Marketing claims belong in quoted, reviewable strings—not mystical adjectives.

---

## Case E — Hands on a scale shot

### Before

```
hand holding water bottle for scale
```

**Result:** Six fingers, melted thumb, second ghost hand.

### After

```
Matte black 500ml water bottle held by one adult hand for scale, clean manicure,
neutral sleeve cuff, soft studio light, light gray background, natural hand anatomy,
five fingers visible, product label blank, no extra jewelry, 1:1.
```

### Conversational edits

1. “Fix the hand: five fingers, natural grip, match existing lighting.”  
2. “Remove the second hand in the lower corner.”  
3. “Keep bottle graphics blank—no invented logo.”  

### Lesson

State finger count up front; still expect to fix hands in conversation. One issue per message.

---

## Case F — Educational diagram labels

### Before

```
infographic about making coffee
```

**Result:** Pretty icons, unreadable spaghetti labels, invented steps.

### After

```
Flat educational diagram of a 4-step coffee brewing process, numbered 1–4 left to right,
simple icons, pastel palette, large readable labels, white background, infographic style.
Labels exactly: "Grind", "Bloom", "Pour", "Serve".
```

### Conversational edits

1. “Replace any wrong labels with exactly: Grind, Bloom, Pour, Serve.”  
2. “Increase spacing between steps; no overlapping leader lines.”  
3. “Simplify icons to single-color line style.”  

### Lesson

Diagrams need **enumerated labels in quotes**. Beauty without legibility fails the brief.

---

## Iteration checklist (print this)

1. Did the **subject** match the brief on try #1? If not, rewrite the prompt—don’t only chat.  
2. Is the fix **local** (text, hand, bg)? → Conversation.  
3. Is the fix **identity** (wrong product/person)? → New prompt + references.  
4. One change per message.  
5. Say what to **keep**.  
6. Brand-check spelling and hex before 4K export.  

---

## See also

- Full playbook: [`../docs/playbook.md`](../docs/playbook.md)  
- Constraint packs: [`../prompts/negatives.md`](../prompts/negatives.md)  
- App: https://bananaproai.app/
