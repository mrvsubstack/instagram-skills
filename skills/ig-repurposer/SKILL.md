---
name: ig-repurposer
description: "Rebuilds content you already made — a LinkedIn post, blog, newsletter, YouTube script, tweet or thread — into a native Instagram post: a carousel when the idea has steps, a caption post or Reel caption when it's one sharp point, re-hooked for the 125-character cut with off-platform leftovers removed. Use this skill whenever the user says things like \"turn this into an Instagram post\", \"repurpose my newsletter for Instagram\", \"make a carousel from this blog\", \"adapt my LinkedIn post for Instagram\", \"cross-post this to Instagram\", or \"this thread would make a good carousel\". Not for writing from scratch (use ig-caption-writer or ig-carousel-planner)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Repurposer

You paste something you've already made. I decide whether it wants to be a carousel, a caption post or a Reel caption, and hand back the Instagram version — slides and caption, ready to build.

This transforms. It doesn't generate. Your claims, numbers and names stay exactly as they were.

---

## The core discovery: pick the format from the shape of the idea

The biggest repurposing mistake on Instagram isn't wording. It's the wrong container.

- An idea with **steps, a list or a before/after** wants to be a **carousel** — it'll get saved.
- An idea that is **one sharp point or one story** wants to be a **caption post** or a **Reel**.
- An idea that needs **showing, not telling** wants to be a **Reel**.

Paste a 1,200-word newsletter into a caption and nobody reads it. Turn its 6 steps into 8 slides and it gets saved.

**Rule: decide the container before you write a single word.**

---

## Step 0 — Intake

1. **The source.** Paste the text, transcript or script. If it's a link, ask for the text (or read it with web search if available, and say so).
2. **Goal:** saves (default), sends, comments or follows.
3. **Any visuals you already have** (photos, screen recordings, slides).
4. **Account voice notes** or a stored voice profile, if available.

---

## Step 1 — Extract the spine

One sentence before anything else:
`SPINE: [the claim] — proved by [the story, steps or number].`

If the source holds several ideas, pick one per post and list the others as spin-offs.

---

## Step 2 — Choose the container

| The spine is… | Container | Hand-off |
|---|---|---|
| A list of 4+ tips or steps | Carousel (numbered list) | `ig-carousel-planner` method |
| A transformation with a result | Carousel (before/after) | `ig-carousel-planner` method |
| A myth your niche believes | Carousel (myth-buster) or Reel | — |
| One sharp opinion | Caption post or Reel | `ig-caption-writer` method |
| One story with a lesson | Caption post | `ig-caption-writer` method |
| Something you do on screen | Reel (how-I) | `tt-hook-scripter` method works for Reels too |

Say which container you picked and why in one line.

---

## Step 3 — Rebuild by source type

| Source | What to do |
|---|---|
| **LinkedIn post** | Cut the professional throat-clearing. Turn the paragraphs into slides or tighten into a short caption. Add the save/send ask LinkedIn posts don't have. |
| **Blog / newsletter** | Take the steps or the one story. Never summarise the whole piece. |
| **YouTube script** | Lift the strongest 30 seconds for a Reel, or the steps for a carousel. |
| **Tweet / X thread** | A thread is usually already a carousel: one tweet per slide, best tweet becomes slide 1. A single tweet becomes a caption hook. |

---

## Step 4 — Re-hook for Instagram

- **Caption post:** new first line that works inside ~125 characters.
- **Carousel:** slide 1 gets a promise and an open loop.
- **Reel:** first 1–3 seconds — on-screen text plus first spoken line.

The source's hook rarely survives the move. Write a new one.

---

## Step 5 — Strip and add

**Strip:**
1. "Link in comments" (LinkedIn) / "link below" (YouTube) — links don't work in captions; point to "link in bio" only if there is one.
2. @-handles from other platforms.
3. "RT", "repost", "as I wrote on LinkedIn".
4. Long paragraphs — break them.

**Add:**
1. One specific save or send ask.
2. 3–5 sized hashtags (`ig-hashtag-strategist`).
3. A visual note for each slide or the Reel's first frame.

---

## Worked example

**Source (LinkedIn post, condensed):** "I stopped hourly billing in 2023. Four changes: price outcomes not hours, offer 3 packages, put the price on page one, say the number and stop talking. Average project went from $900 to $2,400."

**Output:**
```
SPINE: Project pricing beats hourly — proved by $900 → $2,400 average.
CONTAINER: Carousel (before/after) — 4 clear steps + a real result = saves.

S1  $900 → $2,400 per project. Same skills. 4 changes. (The 4th is the hardest.)
S2  Before: $45/hour. Faster work = less money.
S3  1. Price the outcome, not the hours
S4  2. Offer 3 packages
S5  3. Price on page 1 of the proposal
S6  4. Say the number. Then stop talking.
S7  Cheat sheet — save this for your next proposal.

CAPTION
$900 → $2,400 average project. Nothing changed but how I priced.
All 4 steps in the slides.
Save this before your next proposal.
#freelancedesigner #designpricing #freelancetips #proposaltips

STRIPPED: "link in comments", LinkedIn framing
SPIN-OFFS: "Say the number and stop talking" as its own Reel
```

---

## Output format

```
SPINE: [ ]
CONTAINER: [carousel / caption post / Reel] — why: [ ]

[Slides table, or caption, or Reel beat sheet — copy-ready]

--- CAPTION (copy-ready) ---
[caption + hashtags]
--- END ---

SOURCE → INSTAGRAM MAP: [kept / cut / added]
SPIN-OFFS: [ ]
Placeholders to fill: [ ]
```

---

## Sibling skills

- `ig-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `ig-caption-writer`, `ig-carousel-planner` — start from scratch instead.
- `ig-hashtag-strategist` — the tag set.
- `linkedin-repurposer`, `threads-repurposer` — take the same spine elsewhere.
- `content-repurposer` — plan one piece across every platform at once.

---

## Pre-flight checklist

- [ ] Spine written first?
- [ ] Container chosen from the shape of the idea, with a reason?
- [ ] New hook in the right place for the container?
- [ ] Other-platform leftovers stripped?
- [ ] Source facts unchanged, nothing added the user didn't confirm?
- [ ] One save or send ask, 3–5 sized tags?
