---
name: ig-carousel-planner
description: "Plans an Instagram carousel slide by slide — a hook slide that earns the swipe, the best value up front, one point per slide, and a final slide worth saving — plus the caption, delivered as a slide-by-slide script you can drop into Canva or any design tool. Use this skill whenever the user says things like \"plan a carousel\", \"turn this into an Instagram carousel\", \"write my slides\", \"make a carousel that gets saves\", \"how many slides should this be\", or \"carousel about X\". Not for a single image or Reel caption (use ig-caption-writer) and not for designing the visuals themselves (use carousel-generator)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Carousel Planner

You give me a topic, a list, a framework or a before/after. I hand back the slide script — the exact words on every slide, in order — plus the caption and what each slide is there to do.

---

## The core discovery: slide 1 sells the swipe, the last slide sells the save

People decide in under a second whether to swipe. Then interest drops with every slide. So two slides do almost all the work:

- **Slide 1** opens a loop the reader needs closed.
- **The last slide** gives them something worth keeping — a one-slide summary they'll come back to.

Everything in between exists to get them from one to the other without bailing.

**Rule: write the last slide first, then slide 1, then the middle. Put your strongest point on slide 2 or 3, never at the end.**

---

## Step 0 — Intake

1. **The material:** topic, list, framework, steps or transformation.
2. **Goal:** saves (default), sends or follows.
3. **Audience** in one line.
4. **Real proof**, if any: your result, a number, a before/after. Never invented.
5. **Brand style notes** for the on-slide text (all caps headers? lowercase? one colour?). Default: plain.

---

## Step 1 — Pick the carousel shape

| Shape | Goal | When | Spine |
|---|---|---|---|
| **Numbered list** | Saves | You have 5–9 distinct tips | Hook → item per slide → recap |
| **Before / after** | Saves, follows | You have a real result | Before → turning point → steps → after → how to start |
| **Myth-buster** | Sends | Your niche believes something wrong | Myth → why it's wrong → truth, repeat → summary |
| **Steal-this framework** | Saves | You have a named, repeatable method | Name + promise → each part → one-slide cheat sheet |

---

## Step 2 — Set the slide count

Match it to the material. Typical teaching carousel: **6–10 slides**. Instagram allows up to 20 now (verify current limit), but most ideas don't deserve that.

1. **Never pad.** A 4-point idea is a 6-slide carousel (hook + 4 + payoff), not 10.
2. **Fewer than 4 slides?** It's probably a single image. Say so.

---

## Step 3 — Write the slides

### Slide 1 — the hook
A promise plus an open loop. Big text. One idea. A number if one fits.
- Bad → "Portfolio Tips"
- Good → "7 portfolio mistakes that get designers ghosted (#4 is on almost every one I review)"

### Slides 2–3 — front-load the best
Your strongest point goes here. Readers who stop at slide 3 should still leave with something.

### Middle slides — one point each
1. **Readable in 2 seconds.** Headline + at most 1–2 short lines.
2. **Each slide stands alone.** Someone screenshotting slide 5 should understand it.
3. **Concrete over abstract.**
   - Bad → "Be consistent with your branding"
   - Good → "Same 2 fonts on every slide. Not 5."

### Last slide — the payoff
1. **A one-slide summary** worth saving on its own: the checklist, the formula, the cheat sheet.
2. **One ask.** Save, send or follow. Not all three.
   - Bad → "Like, comment, share, save and follow for more!!"
   - Good → "Save this. Check it before your next portfolio update."

---

## Step 4 — Write the caption

The carousel carries the content, so the caption can be short:
1. Restate the hook in the first ~125 characters.
2. One or two lines of context or a personal note.
3. The same single ask as the last slide.
4. 3–5 sized hashtags (from `ig-hashtag-strategist`).

---

## Step 5 — Scrub

Max one dash per slide. No "The result?" slides. No stacked "No X. No Y. Just Z." slides. No AI word clusters. Run `ig-humanizer` if in doubt.

---

## Worked example

**Input:** "Topic: pricing freelance design work. Goal: saves. Proof: I moved from hourly ($45/h) to project pricing and my average project went from $900 to $2,400."

**Output:**
```
SHAPE: Before / after · 7 slides · Goal: saves

S1  I charged $45 an hour for 3 years. Then I stopped. (What changed my average project from $900 → $2,400)
S2  Hourly punishes you for getting faster. The better you get, the less you earn.
S3  Step 1: Price the outcome, not the hours. "New homepage that converts" — not "20 hours of design".
S4  Step 2: Offer 3 packages. Most clients pick the middle one.
S5  Step 3: Put the price on page 1 of the proposal. Not hidden on the last page.
S6  Step 4: Say the number, then stop talking.
S7  CHEAT SHEET → Outcome, not hours · 3 packages · Price on page 1 · Say it, then silence. Save this for your next proposal.

CAPTION
$45 an hour for 3 years. Average project now: $2,400.
The 4 changes are in the slides. Number 4 is the hardest.
Save this for your next proposal.
#freelancedesigner #designpricing #freelancetips #designbusiness
```
("Most clients pick the middle one" is a common pattern, not a stat — keep it phrased as the user's experience or cut it.)

---

## Output format

```
SHAPE: [ ] · SLIDES: [n] · GOAL: [ ]

| Slide | Job | On-slide text | Visual note |
|-------|-----|---------------|-------------|
| 1 | Hook + loop | | |
| … | | | |
| N | Payoff + one ask | | |

--- CAPTION (copy-ready) ---
[caption + hashtags]
--- END ---

Image format: portrait 4:5 recommended (verify current specs) · all images, keep the look consistent
Placeholders to fill: [ ]
```

---

## Sibling skills

- `ig-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `ig-caption-writer` — a single image or a Reel.
- `carousel-generator` — turn this script into designed slides.
- `ig-hashtag-strategist` — the tag set for the caption.
- `ig-hook-extractor` — reverse-engineer a carousel you admire.

---

## Pre-flight checklist

- [ ] Last slide written first and worth saving alone?
- [ ] Slide 1 has a promise and an open loop, not a bare title?
- [ ] Best point on slide 2 or 3?
- [ ] One point per slide, readable in 2 seconds?
- [ ] No padding to reach a round number?
- [ ] One ask only?
- [ ] Every result is the user's own?
