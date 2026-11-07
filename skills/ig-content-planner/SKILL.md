---
name: ig-content-planner
description: "Builds a 7-day Instagram plan: which days get a Reel, carousel, single image or story set, the pillar and hook for each, the reaction each post must earn, a daily story rhythm and a weekly saves-and-sends target. Use this skill whenever the user says things like \"plan my Instagram week\", \"what should I post on Instagram\", \"give me an Instagram content calendar\", \"how many Reels should I post\", \"plan my launch on Instagram\", or \"I post randomly on Instagram\". Not for writing a single caption (use ig-caption-writer) or one carousel (use ig-carousel-planner)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Content Planner

You give me your theme, audience, pillars and how much you can realistically make. I hand back a 7-day plan where every post has a format, a hook and a job — plus a story rhythm that runs underneath.

---

## The core discovery: each format has one job

Instagram formats aren't interchangeable. They do different work:
- **Reels** reach people who don't follow you yet.
- **Carousels** get saved, so they keep earning for weeks.
- **Single images** spark quick comments and reactions.
- **Stories** deepen the relationship with people who already follow you.

A week of only Reels gets views and no trust. A week of only stories talks to the same 200 people forever.

**Rule: pick the format by the job the post has to do, then pick the topic.**

---

## Step 0 — Intake

1. **Theme** for the week. Default: what the user is working on now.
2. **Audience** in one line.
3. **Capacity:** how many feed posts can they actually make? Default: 4. Be honest — 3 good posts beat 7 rushed ones.
4. **Pillars.** Default mix below.
5. **Raw material:** real stories, results, client questions, behind-the-scenes moments from this week.
6. **Any launch or promotion.** Default: none.

---

## Step 1 — Set the pillar mix

| Pillar | Share | Job |
|---|---|---|
| **Teach** | 40% | Tips, frameworks, how-tos — earns saves |
| **Story** | 30% | Your real experiences — earns follows and trust |
| **Conversation** | 20% | Relatable moments, questions, polls — earns comments |
| **Offer** | 10% (1–2 posts max) | What you sell, as the next step |

No pillar above 50% of feed posts.

---

## Step 2 — Assign format, hook and goal

| Goal | Formats | Hooks that fit |
|---|---|---|
| **Saves** | Carousel, how-I Reel | Numbered list · steal-this framework · before/after · number-first result |
| **Sends** | Reel, carousel | Contrarian truth · myth-buster · pattern-interrupt Reel |
| **Comments** | Single image, story poll | Relatable moment · mini confession |
| **Follows** | Before/after, story post | Mini confession · before/after |

Rules:
1. **At least 2 Reels and 2 carousels** in a 4–5 post week, if capacity allows.
2. **At least 3 save-earning posts and 2 send-earning posts.** Saves and sends are the headline numbers, not likes.
3. **No hook used more than twice a week.**
4. **At least one real first-person story.**
5. **Every angle comes from the raw material.** No invented results in the plan.
   - Bad → "Thu: Carousel — 10 productivity hacks"
   - Good → "Thu: Carousel — the 4 changes that took my average project from $900 to $2,400 (your note from Monday)"

---

## Step 3 — Plan the stories

Stories run every day, underneath the feed:
- **2–4 frames a day.**
- One **behind-the-scenes** frame (what you're making, a real moment).
- One **interactive** frame (poll, question box, quiz) — the replies become next week's content.
- One **reshare** of your newest feed post, so followers who missed it see it.
- On offer days: one frame with the link.

---

## Step 4 — Set the weekly target

Pick one number to watch: **saves + sends this week**. Compare with last week if the user has it. Don't promise numbers — set a target they can check.

Posting times: use the user's own Insights (Professional dashboard → audience → most active times). If they don't have them, write "check your Insights" rather than quoting generic times as fact.

---

## Worked example

**Input:** "Freelance designer, audience = junior designers, capacity 4 posts, material: moved from hourly to project pricing; a client asked for 14 revisions; I redesigned my portfolio homepage this week."

**Output:**
| Day | Format | Pillar | Hook | Goal | Angle |
|---|---|---|---|---|---|
| Mon | Reel | Teach | Pattern interrupt | Sends | "You're charging hourly. Here's why that caps you." (15s talking head) |
| Tue | Carousel | Story | Before/after | Saves | $45/h → $2,400 projects: the 4 changes |
| Thu | Single image | Conversation | Relatable moment | Comments | Screenshot of revision #14 request (name blurred) — "where's your line?" |
| Sat | Carousel | Teach | Steal-this framework | Saves | The 5-section portfolio homepage I just rebuilt |
Stories daily: BTS of the portfolio redesign · poll "hourly or project?" · reshare each feed post.
Target: saves + sends. Offer: none this week.

---

## Output format

```
WEEK OF [date] · Theme: [ ] · Audience: [ ] · Capacity: [n] feed posts
Pillar mix: Teach [ ]% · Story [ ]% · Conversation [ ]% · Offer [ ]%

| Day | Format | Pillar | Hook | Goal | Angle (source) | Time |

STORIES (daily): [BTS / interactive / reshare / link days]

BALANCE CHECK
- [ ] 2+ Reels, 2+ carousels (if capacity allows)
- [ ] 3+ save posts, 2+ send posts
- [ ] 1+ real story post
- [ ] No pillar over 50%, offer 1–2 max
- [ ] No hook more than twice

WEEKLY TARGET: saves + sends = [ ] (last week: [ ] if known)
MISSING MATERIAL: [what to ask for]
```

---

## Sibling skills

- `ig-caption-writer` — write each Reel or image caption.
- `ig-carousel-planner` — script each carousel.
- `ig-hashtag-strategist` — rotate tag sets across the week.
- `ig-profile-optimizer` — make sure the profile converts the new visitors.

---

## Pre-flight checklist

- [ ] Plan fits the user's real capacity?
- [ ] Every post has a format chosen by job, and a goal?
- [ ] Saves and sends targets met?
- [ ] Every angle traces to real material, no invented results?
- [ ] Story rhythm included?
- [ ] Posting times from Insights, or labelled "check your Insights"?
