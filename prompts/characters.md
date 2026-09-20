# Character & consistency prompts

For mascots, game protagonists, brand ambassadors, and turnaround sheets.  
**Recommended ratios:** 1:1 sheets · 16:9 scenes · **Features to use:** character consistency, multi-reference  
**Tool:** [Banana Pro AI](https://bananaproai.app/)

Lock identity details early (hair, age, marks, palette). Prefer neutral lighting for sheets; add drama only in scene prompts.

---

## 1. Brand mascot turnaround

```
Character design sheet of [MASCOT: friendly fox in a small blue scarf],
flat vector-inspired 3D, soft rounded shapes, front view + three-quarter + side view
on clean white background, consistent eye style and snout length, children's brand mascot,
even studio lighting, no text, high clarity outline, 16:9 sheet layout.
```

**Why it works:** Multiple views + “consistent [feature]” language + white void.  
**Swap:** species, scarf/colors, age vibe (kids vs premium).

---

## 2. Game protagonist full-body

```
Full-body character concept of [HERO: young explorer with copper short hair, teal jacket,
leather satchel], determined smile, neutral gray background, stylized game art,
consistent proportions, front view, soft studio light, no weapons, no text, 1:1.
```

**Why it works:** Outfit tokens are identity anchors; gray bg isolates for later compositing.  
**Swap:** hair, outfit colors, expression; keep the same string across scenes.

---

## 3. Semi-realistic portrait lock

```
Semi-realistic portrait of [PERSONA: woman mid-20s, silver bob haircut, light freckles,
calm expression, hazel eyes], soft beauty lighting, neutral backdrop, head-and-shoulders,
identity-sheet quality, no makeup brand logos, 1:1.
```

**Why it works:** Specific facial attributes beat “beautiful woman.” Use as reference for later poses.  
**Swap:** age, hair, freckles on/off, expression.

---

## 4. Multi-outfit variation sheet

```
Same female character, mid-20s, silver bob haircut, light freckles, calm expression,
outfit variation sheet with three panels: [1: casual tee], [2: winter coat], [3: formal blazer],
identical face and hair across panels, white background, fashion character sheet, 16:9.
```

**Why it works:** Explicit “identical face and hair” + panel structure.  
**Swap:** outfits; attach prior portrait as multi-reference.

---

## 5. Chibi / sticker set

```
Cute chibi sticker sheet of [CHARACTER: teal robot with one antenna], 6 poses
(wave, jump, think, cheer, sad, sleep), thick white sticker cut-out border,
pastel background, consistent robot design, kawaii product stickers, no tiny text, 1:1.
```

**Why it works:** Pose list + sticker border convention; limited palette reduces drift.  
**Swap:** character, pose list, border color.

---

## 6. Antagonist design (family-friendly)

```
Character concept of [FOE: sly raccoon in oversized coat with patched elbows],
smirking expression, storybook illustration style, full-body on kraft paper texture bg,
consistent proportions, no gore, no real-person likeness, 1:1.
```

**Why it works:** Personality via wardrobe + expression; style lock to storybook.  
**Swap:** animal, coat details, style (storybook vs comic).

---

## 7. Employee / team avatar set

```
Corporate avatar set: [COUNT: four] diverse professionals, consistent illustrated style
(flat vector with soft shading), circular crop friendly, friendly smile, solid
[BRAND BG: #0B3D91], matching line weight across all four, no logos, 1:1 grid.
```

**Why it works:** Style + line weight consistency called out for sets.  
**Swap:** count, brand hex, industry wardrobe.

---

## 8. Historical-inspired (fictionalized)

```
Fictional explorer character inspired by early aviation era (not a real historical person),
leather flight helmet, goggles on forehead, determined look, painterly concept art,
neutral museum-gray background, bust portrait, 1:1.
```

**Why it works:** “Not a real person” reduces lookalike risk while keeping era cues.  
**Swap:** era, wardrobe, medium.

---

## 9. Creature companion

```
Small companion creature: [CREATURE: round owl with knitted red scarf], perched,
cute but not baby-ish, consistent feather pattern, soft key light, plain backdrop,
game companion concept art, full body, no text, 1:1.
```

**Why it works:** Size/personality notes prevent “generic cute animal” mush.  
**Swap:** creature, scarf, game vs storybook style.

---

## 10. Expression sheet

```
Expression sheet of [LOCKED CHARACTER DESCRIPTION — paste exact prior identity string],
six panels: neutral, smile, laugh, angry, sad, surprised, identical hair and outfit,
white background, even lighting, concept art expression chart, 16:9.
```

**Why it works:** Reusing the **exact** identity string is the #1 consistency trick.  
**Swap:** expression list; always paste the lock string verbatim.

---

## 11. Action scene with locked hero

```
Action scene: [LOCKED HERO STRING] sprinting across a sunlit marketplace,
motion implied, camera at chest height, cinematic color grade matching brand teal,
keep face and outfit identical to reference, no new accessories, 16:9.
```

**Why it works:** Scene change only; “no new accessories” fights drift.  
**Swap:** environment, action verb; attach refs.

---

## 12. Age progression (same identity)

```
Age progression sheet of the same character: ages [12, 25, 50], identical core features
(eye shape, freckle pattern, hair color family), three bust panels, white background,
realistic illustrative style, consistent lighting, 16:9.
```

**Why it works:** Names which features must persist across ages.  
**Swap:** ages, which features are locked.

---

## Consistency workflow

1. Generate a **neutral portrait or turnaround** → save as reference  
2. Copy the **exact identity clause** into every later prompt  
3. Enable **character consistency / multi-reference** in Banana Pro AI  
4. Change **one** variable per iteration (pose *or* outfit *or* scene)  
5. Conversational edit: “Keep the same face and hairstyle; only change …”
