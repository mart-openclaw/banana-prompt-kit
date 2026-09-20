# Banana Prompt Kit

**Production-ready prompt packs and a full Image Prompt Playbook for [Banana Pro AI](https://bananaproai.app/).**

This kit is for creators, marketers, and product teams who need repeatable text-to-image results—not one-off “magic words.” Use it with Banana Pro AI’s text-to-image, conversational editing, 2K/4K export, typography-in-image, character consistency, and multi-reference features.

> **App:** https://bananaproai.app/  
> **Support:** support@bananaproai.app  
> **Playbook PDF:** `banana-pro-ai-image-prompt-playbook.pdf` (companion release)

---

## Why this repo exists

Most “prompt lists” online are keyword soup. This kit instead documents:

1. A **reusable prompt formula** (subject → attributes → composition → style → constraints)
2. **Channel playbooks** (e-commerce, thumbnails, ads, characters, diagrams)
3. **Conversational edit recipes** for fixing hands, text, lighting, and backgrounds
4. **Copy-paste prompts** with notes on *why they work* and which variables to swap
5. A **workflow** from brief → export that teams can adopt

If you only want the narrative guide, start with [`docs/playbook.md`](docs/playbook.md). If you want to ship assets today, jump into `prompts/`.

---

## Repository structure

```
banana-prompt-kit/
├── README.md                 ← you are here
├── LICENSE                   ← MIT
├── docs/
│   └── playbook.md           ← full Image Prompt Playbook (2026)
├── prompts/
│   ├── ecommerce.md          ← packshots, lifestyle, apparel, electronics
│   ├── thumbnails.md         ← YouTube / video covers
│   ├── characters.md         ← mascots, sheets, consistency locks
│   ├── ads-social.md         ← feed, stories, B2B, sale creatives
│   └── negatives.md          ← constraint libraries & anti-patterns
└── examples/
    └── before-after-notes.md ← iteration stories (text before/after)
```

---

## How to use

### 1. Skim the playbook once

Read [`docs/playbook.md`](docs/playbook.md) sections 1–2 (how prompts work + formula). That alone will improve first-generation hit rate.

### 2. Pick a channel pack

| If you are making… | Open |
|--------------------|------|
| Marketplace / DTC product shots | [`prompts/ecommerce.md`](prompts/ecommerce.md) |
| YouTube or course thumbnails | [`prompts/thumbnails.md`](prompts/thumbnails.md) |
| Mascots / game / brand characters | [`prompts/characters.md`](prompts/characters.md) |
| Meta / TikTok / LinkedIn ads | [`prompts/ads-social.md`](prompts/ads-social.md) |
| Cleanup & brand safety constraints | [`prompts/negatives.md`](prompts/negatives.md) |

### 3. Swap the bracketed variables

Every prompt uses `[BRACKETS]` for the pieces you should change: product name, color hex, emotion, exact on-image copy, etc.

### 4. Generate, then converse

In [Banana Pro AI](https://bananaproai.app/):

1. Paste the adapted prompt → generate  
2. Apply **one** conversational edit at a time (see playbook §4 and `examples/before-after-notes.md`)  
3. Brand-check spelling, hex colors, and claims  
4. Export **2K** for review, **4K** for final paid placements when detail matters  

### 5. Version your winners

Copy a winning prompt into your team wiki or a private fork. Treat prompts like ad copy: name versions (`packshot-serum-v3`).

---

## Prompt formula (cheat sheet)

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

**Compact form:**

```
[SUBJECT], [2–4 attributes], [setting],
shot as [composition], [lighting],
in the style of [style], [mood/palette],
[constraints].
```

---

## Aspect ratios quick reference

| Ratio | Use |
|-------|-----|
| 1:1 | Feed posts, marketplace tiles |
| 4:5 | Instagram portrait feed |
| 16:9 | YouTube, blogs, decks |
| 9:16 | Stories, Reels, TikTok, Shorts |

Full export guidance (including 2K/4K) lives in the playbook §5.

---

## Design principles behind the packs

- **Subject first** — models overweight early tokens  
- **Concrete over flattering** — “soft key light from camera-left” beats “masterpiece”  
- **Exact strings for typography** — quote the headline you want rendered  
- **Constraints are part of the prompt** — white background, no watermark, no extra props  
- **Conversation for surgery** — don’t regenerate the universe to fix a hand  

---

## About Banana Pro AI

[Banana Pro AI](https://bananaproai.app/) is an AI image generator and photo editor:

- Text-to-image  
- Conversational editing  
- 2K / 4K output  
- Typography in images  
- Character consistency  
- Multi-reference workflows  

Contact: **support@bananaproai.app**

---

## Contributing

PRs that add **tested** prompts with notes (why it works + variables) are welcome. Please:

- Keep one prompt per fenced block  
- Include channel + recommended aspect ratio  
- Avoid trademarked character likenesses and celebrity names  
- Do not add affiliate spam or “top 50 tools” listicles  

---

## License

MIT — see [`LICENSE`](LICENSE).

Prompts are provided for educational and commercial creative use with your own tools and accounts. Always verify the product Terms of Service for image licensing on your intended channel.

---

## Related assets

| Asset | Location |
|-------|----------|
| Full playbook (Markdown) | [`docs/playbook.md`](docs/playbook.md) |
| Full playbook (PDF) | `banana-pro-ai-image-prompt-playbook.pdf` (sibling release) |
| Product | https://bananaproai.app/ |
