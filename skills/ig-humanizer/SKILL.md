---
name: ig-humanizer
description: "Removes the patterns that make an Instagram caption or carousel slide read machine-written — clusters of AI words, reveal bridges, fragment stacks, emoji storms, performed honesty — without sanding off the writer's voice. Three modes: Rewrite (default), Audit (pre-post pass/fail on hook, length, hashtags, emoji and call to action) and Profile (learn your voice from 3–6 past captions). Use this skill whenever the user says things like \"humanize this caption\", \"this sounds like AI\", \"check my caption before I post\", \"audit this carousel\", \"make my slides sound like me\", or \"learn how I write captions\". Not for writing from scratch (use ig-caption-writer or ig-carousel-planner), and not a tool for beating AI detectors."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Humanizer

You paste a caption, a set of slide texts, or both. I hand back the clean version, a short list of what changed and why, and a reader verdict: **reads human / mixed / reads AI**.

This fixes what people notice when they read. It doesn't promise anything about AI detectors — on 150 words of caption, their scores are noise.

---

## The core discovery: Instagram's AI tells are louder because captions are short

In a 1,500-word article, one "elevate" disappears. In a 60-word caption it's 2% of the text. And on carousel slides, where every slide is 8–15 words, one templated phrase can be the whole slide.

Instagram also has its own tells: emoji at the start of every line, "✨" sprinkled for mood, "POV:" on things that aren't a point of view, three-word fragment slides.

**Rule: judge each caption paragraph and each slide on its own. One marker can be fine. Two on one slide is a rewrite.**

---

## The three modes

### Mode 1 — Rewrite (default)
**When:** you want it ready to post. **How:** the four passes below.

### Mode 2 — Audit
**When:** "check this before I post". **How:** the audit checklist. Return Blockers, Warnings and one fix per item. Change nothing.

### Mode 3 — Profile
**When:** "learn how I write". You paste 3–6 captions you wrote and liked. **How:** pull checkable habits (how you open, line length, emoji use, how you ask for action, words you never use). Output rules with a real example each. Hand them to `voice-profile-bank`. Never invent a rule you can't show in their captions.

---

## The four passes (Rewrite mode)

### Pass 1 — Scrub
Count markers per paragraph (caption) or per slide.

**Vocabulary markers:** elevate, unlock, level up, game-changer, dive in, delve, journey (as metaphor), seamless, empower, transformative, crucial, leverage, curated, vibes (as filler), next level.

**Single-hit fixes:**
1. "It's not X, it's Y."
   - Bad → "It's not about the gear. It's about the light."
   - Good → "My best Reel was filmed on a 2019 phone next to a window."
2. Reveal bridges: "The result?", "The secret?", "Here's the thing", "Plot twist:".
3. "Let's talk about…", "Let me tell you…" openers.
4. "POV:" when the caption isn't a scene from someone's point of view.
5. Closers: "What do you think?", "Double tap if you agree", "Comment YES".

**Emoji:**
- An emoji opening every line → keep at most one or two, where they mark something.
- Mood emoji ("✨🙌🔥") with no job → cut.
- 0–3 per caption is normal. Ten is a storm.

**Punctuation:** at most one em dash per slide; about one per 100 words in a caption. Replace extras with a comma, colon or brackets — never a full stop.

### Pass 2 — Rhythm
1. **No fragment stacks.**
   - Bad slide → "Simple. Fast. Free."
   - Good slide → "Takes 10 minutes, costs nothing."
2. **No "No X. No Y. Just Z."**
3. **Max two standalone fragments per caption.**
4. **Short lines and blank lines are fine** — that's how Instagram captions look. Fix fragments-for-drama, not layout.
5. **Slides are short by design.** Never pad a slide to make it "flow", never chop one for punch.

### Pass 3 — Add (only what the writer gives you)
A caption that reads human usually has one of:
- A number with a referent ("4 seconds → 7 seconds average watch time").
- A named thing (tool, place, person, date).
- A moment you saw or did.

If missing, **ask**. Never insert a number, story, confession or hedge the writer didn't give you. Banned insertions: "real talk", "not gonna lie", "I'll be honest".

### Pass 4 — Self-check
1. Did I create fragment slides or reveal bridges? → merge.
2. Did I add a framed confession or hedge? → remove.
3. Did I strip the writer's real quirks (their one emoji habit, lowercase style, slang)? → restore.

---

## Audit checklist (Mode 2)

**Blockers:**
- Hook doesn't work within the first ~125 characters (caption) or slide 1 is a bare title (carousel).
- More hashtags than Instagram's current cap (verify), or a hashtag wall.
- Engagement bait ("comment YES", "double tap").
- 2+ markers on one slide or in one caption paragraph.
- An unsourced stat or invented-sounding result.

**Warnings:**
- More than 3 emoji, or emoji opening every line.
- Generic call to action, or more than one.
- No specific detail anywhere.
- Over 2,200 characters (verify current limit).
- Media not mentioned (caption with no image/Reel reminder).

---

## Worked example (Rewrite)

**Input caption:**
"✨ Let's talk about elevating your content game ✨
The secret? Consistency. 🔥
It's not about posting more. It's about posting smarter. 🙌
Unlock your potential today! 💯
What do you think? 👇"

**Output:**
```
I posted every day in March. 31 Reels.

Average views went down.

In April I posted 3 times a week and spent the saved hours on the first 2 seconds of each one. Average views tripled.

Which would you rather cut: posts or editing time?
```
Changes: removed "elevating", "unlock", reveal bridge "The secret?", "not X, it's Y", 7 mood emoji, generic closer · **asked the user** for March/April, 31 Reels and "tripled" before using them.
Verdict: reads human.

---

## Output format

```
MODE: [rewrite / audit / profile]
VERDICT: [reads human / mixed / reads AI] (reader estimate, not a detector score)

--- CLEAN VERSION (copy-ready) ---
[caption and/or slide texts]
--- END ---

CHANGES: [pattern → fix]
DENSITY: [per paragraph or per slide]
NEEDS FROM YOU: [numbers, names, moments]
KEPT ON PURPOSE: [quirks]
```

---

## Sibling skills

- `ig-caption-writer`, `ig-carousel-planner` — write it first.
- `voice-profile-bank` — store what Profile mode learns.
- `final-edit-modes` — edit into Mr V's own published voice.
- `linkedin-humanizer`, `threads-humanizer`, `x-humanizer` — other platforms.

---

## Pre-flight checklist

- [ ] Judged per slide and per paragraph?
- [ ] Single-hit phrases fixed, emoji storms cut?
- [ ] No fragment slides created, no dash turned into a full stop?
- [ ] Nothing inserted the writer didn't give?
- [ ] Self-check run?
- [ ] Verdict labelled as a reader estimate?
