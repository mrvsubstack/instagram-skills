---
name: ig-caption-writer
description: "Writes an Instagram caption for a single image or a Reel: a hook that works in the first ~125 characters before \"more\", a skimmable body, one specific call to action and a small sized hashtag set, delivered as a copy-ready block. Use this skill whenever the user says things like \"write an Instagram caption\", \"caption this Reel\", \"I need a hook for this post\", \"make this caption get saves\", \"rewrite my caption\", or \"what should I write under this photo\". Not for multi-slide carousels (use ig-carousel-planner) or checking a finished caption (use ig-humanizer in audit mode)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Caption Writer

You tell me what the image or Reel is, who it's for and what you want it to earn. I hand back one caption, ready to paste, with the hook chosen by goal and a 3–5 tag hashtag set.

---

## The core discovery: Instagram is judged on sends and saves

A like costs the viewer nothing. A **save** means "I'll need this later". A **send** means "you need to see this". Those are the two actions that tell Instagram a post is worth showing to more people — and they're the ones your caption can actually cause.

And the caption only gets read if the first line earns the tap on "more". Instagram cuts captions at roughly 125 characters.

**Rule: the first 125 characters must work alone, and the last line must ask for one specific action — usually a save or a send.**

---

## Step 0 — Intake

1. **The media.** What's in the image or Reel, in one or two lines. If it's a Reel, what happens in the first 3 seconds.
2. **Goal:** saves, sends, comments or follows. Default: saves.
3. **Audience** in one line.
4. **One real detail:** a number, a date, a named tool or person. If there's nothing, ask once. If still nothing, drop the claim — never invent one.
5. **Voice samples or a stored voice profile**, if available.

---

## Step 1 — Pick the caption hook by goal

| Goal | Hook | Shape |
|---|---|---|
| **Saves** | Number-first result | "[Exact result] in [time]. The [n]-step version you can copy:" |
| **Sends** | Contrarian truth | "[Common advice] is why [audience] stays stuck." |
| **Comments** | Relatable moment | Drop into a specific shared moment, no setup. "Opening Canva to make one graphic. Closing it 2 hours later." |
| **Follows** | Mini confession | A first-person story with a real cost. "I spent $1,900 on a course I never opened past lesson 3." |

Offer 2–3 hook options. Let the user pick.

### Hook rules
1. **It makes sense with nothing after it.**
   - Bad → "So this happened…"
   - Good → "My Reel got 41,000 views. The caption was 9 words."
2. **Payoff, tension or number before the cut.** Not after.
3. **No throat-clearing openers:** "Let's talk about…", "Here's the thing…", "POV:" on something that isn't a point of view.
4. **No announced honesty:** "Real talk", "Not gonna lie". The fact does the work.

---

## Step 2 — Write the body

1. **Short lines. A blank line between beats.** People read captions on a phone with their thumb.
2. **Deliver what the hook promised** — the steps, the story or the reason.
3. **One idea per caption.** Two ideas is two posts.
4. **One specific detail per beat.**
   - Bad → "Lighting really matters for Reels."
   - Good → "I moved my desk 1 metre toward the window. Watch time went from 4 to 7 seconds."
5. **Length:** whatever the idea needs. Instagram allows 2,200 characters (verify current limit). A story can run long; a tip shouldn't.
6. **0–3 emoji, each with a job.** No emoji storms.

---

## Step 3 — Write one call to action

One. Specific. Matched to the goal.

| Goal | Bad | Good |
|---|---|---|
| Saves | "Save this!" | "Save this for the next time a Reel flops in the first hour." |
| Sends | "Share with friends" | "Send this to the friend who still posts at midnight." |
| Comments | "What do you think?" | "Which of the 4 do you skip? Mine's #3." |
| Follows | "Follow for more" | "I post one teardown like this every Thursday." |

No "comment YES and I'll DM you" gates. No "double tap if you agree".

---

## Step 4 — Hashtags

Hand the post to `ig-hashtag-strategist`, or apply its rule directly: **3–5 tags, sized** — mostly small niche tags, one mid, at most one broad. Instagram has been tightening hashtag limits; check the current cap with web search before going above 5. Put them at the end or in the first comment.

---

## Step 5 — Quick scrub

Run the fast `ig-humanizer` check: no clusters of AI words (elevate, unlock, game-changer, level up, dive in), no "The result?" reveals, no "No X. No Y. Just Z." stacks, no invented numbers.

---

## Worked example

**Input:** "Reel: me reorganising my desk for filming, before/after. Goal: saves. Audience: new creators filming at home. Detail: watch time went from 4s to 7s average after moving to window light."

**Output:**
```
Average watch time: 4 seconds → 7 seconds. I didn't buy a single light.

Here's the whole change:

1. Desk 1 metre closer to the window, facing it
2. Window light hits your face from the front, not the side
3. Phone at eye level on a stack of books
4. Film between 10am and 2pm, nothing after 4

That's it. The ring light is still in its box.

Save this for the next time you film and think "why do I look tired?"

#homestudiosetup #smallcreatortips #filmingtips #reelstips
```
Hook: number-first result → saves. 389 characters.

---

## Output format

```
GOAL: [saves / sends / comments / follows]
HOOK OPTIONS: A) [ ] B) [ ] C) [ ]

--- CAPTION (copy-ready) ---
[caption]
[hashtags]
--- END ---

Hook length: [n] chars (target ≤125) · Total: [n] chars
Media you need to attach: [image / Reel — and cover frame suggestion]
Placeholders to fill: [ ]
```

---

## Sibling skills

- `ig-postiz-publisher` — schedule the finished post through Postiz after you approve it.
- `ig-carousel-planner` — the idea needs several slides.
- `ig-hashtag-strategist` — build the sized tag set.
- `ig-hook-extractor` — study a post you admire first.
- `ig-humanizer` — audit or scrub the final caption.

---

## Pre-flight checklist

- [ ] First ~125 characters work alone?
- [ ] Hook matches the goal?
- [ ] Every number came from the user?
- [ ] One idea, short lines, blank lines between beats?
- [ ] One specific call to action — no bait?
- [ ] 3–5 sized hashtags at the end, cap verified if going higher?
- [ ] Reminder to attach the media included?
