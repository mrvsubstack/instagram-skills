---
name: ig-profile-optimizer
description: "Audits an Instagram profile the way a stranger sees it — photo, name field, handle, bio, link, category, highlights, top grid and pinned posts — and rewrites each weak part so a visitor knows in seconds who you are for and why to follow. Use this skill whenever the user says things like \"review my Instagram profile\", \"fix my Instagram bio\", \"what should my highlights be\", \"why don't profile visits turn into follows\", \"rewrite my bio in 150 characters\", or \"Instagram profile audit\". Not for writing captions (use ig-caption-writer) or planning posts (use ig-content-planner)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Profile Optimizer

You send screenshots of your profile header and top grid, or paste the name, bio and link, and tell me what you want followers to do next. I hand back a scorecard of nine parts, the top three fixes, and before → after rewrites inside Instagram's character limits.

---

## The core discovery: the follow decision happens in one screen

A visitor lands on your profile from a Reel they liked. Without scrolling they see: photo, name, bio, link, highlights, and the first two or three rows of the grid. That one screen decides follow or leave.

**The header test:** cover everything below the first grid row. Would a stranger know who this account is for and what they'll get? If not, nothing else matters yet.

**Rule: every part of that one screen must answer "what's in it for me if I follow?"**

---

## Step 0 — Intake

1. **Screenshot of the header + first 9 grid tiles**, or pasted name, @handle, bio, link and a description of highlights and grid.
2. **Account type:** personal, creator or business (creator/business unlock the category label).
3. **Goal** (pick one): **grow followers**, **sell a product**, **land clients**, **build authority**. Default: grow followers.
4. **Top 3 performing posts**, if known — candidates for pins.

Score only what you've been shown. Mark the rest "NOT SHOWN".

---

## Step 1 — Score nine parts

Limits below were correct at the time of writing — verify with web search and label anything unverified.

| # | Part | Passes when |
|---|---|---|
| 1 | **Photo** | Clear face (or clean logo), fills the circle, high contrast, readable tiny |
| 2 | **Name field** | Real name + the topic people search for, within ~30 characters |
| 3 | **@handle** | Short, sayable, matches your brand |
| 4 | **Bio** | What a follower gets + topic + one proof, within 150 characters |
| 5 | **Link** | One clear destination matched to the goal |
| 6 | **Category** | Set, and it matches the niche |
| 7 | **Highlights** | 4–6, ordered by what a visitor wants to know next, consistent covers, names that don't cut off |
| 8 | **Top 9 grid** | Looks like one account, readable at a glance, shows what you post |
| 9 | **Pinned posts** | Up to 3, each a best proof for the goal |

---

## Step 2 — Rewrite what failed

### Name field — the search fix
Instagram search reads the **name field**, not just the handle. Put a searchable word there.
- Bad → "Sam Rivera"
- Good → "Sam Rivera | Freelance Pricing"

This is usually the single highest-leverage change. Keep it within the limit.

### Bio — value + topic + proof
1. **Lead with what the follower gets**, not your job title.
   - Bad → "Graphic designer 🎨 | Coffee lover ☕ | Dreamer ✨"
   - Good → "Helping freelance designers charge more\nWeekly pricing teardowns\n$45/h → $2,400 projects"
2. **One proof, real only.** If there's none, use a specific instead ("Teardowns every Thursday").
3. **Line breaks fine. One or two anchor emoji fine. No emoji storms.**
4. **Count characters.** Never deliver a bio over 150.

### Link — one destination
Match it to the goal: offer page, newsletter signup, booking link. If the user truly needs several, a single link page with the goal link at the top.

### Highlights — answer the next question
Order them left to right:
1. **Start here** — who this is for, what you post.
2. **Proof** — results, testimonials (real only).
3. **Offer** — what you sell.
4. **FAQ** — the questions you get in DMs.
5. **About** — the human side.

Covers in one style. Names of one short word so they don't truncate.

### Top 9 grid
Judge it as a set:
- Does it look like one account (colours, framing, text style)?
- Can you tell the topic without reading captions?
- Are the 3 newest tiles strong? Weak ones can be archived or outranked by pins.

### Pins — up to 3
Pick by goal: one top performer, one clear offer or "start here" post, one who-this-is-for post.

---

## Worked example

**Input:** Name "Sam Rivera". Bio "Designer 🎨 | Coffee ☕ | Making things pretty ✨". Link: personal homepage. Highlights: "Travel", "Food", "2023", "Work". Goal: land clients.

**Output:**
```
SCORECARD: Photo Pass · Name Fail · Bio Fail · Link Needs work · Highlights Fail · others NOT SHOWN

TOP 3 FIXES
1. Name field: add the searchable topic
2. Bio: lead with the client's outcome
3. Highlights: reorder around a hiring client's questions

NAME  before: Sam Rivera
      after:  Sam Rivera | Brand Designer   (27 chars)

BIO   before: Designer 🎨 | Coffee ☕ | Making things pretty ✨
      after:  Brand identities for coffee shops & bakeries
              Logo → menu → signage, one designer
              Booking [month] projects ↓                (118 chars)

LINK  before: homepage → after: booking/enquiry page

HIGHLIGHTS  before: Travel · Food · 2023 · Work
            after:  Start · Work · Process · Prices · FAQ
```
(The "coffee shops & bakeries" niche came from the user's portfolio — never assign a niche the user hasn't chosen.)

---

## Output format

```
GOAL: [ ] · ACCOUNT TYPE: [ ]
HEADER TEST: pass / fail — [one line why]

SCORECARD
| # | Part | Score | Reason |

TOP 3 FIXES
1. … 2. … 3. …

REWRITES (copy-ready, with character counts)
Name · Bio · Link · Category · Highlights (order, names, cover note) · Grid moves · Pins

MISSING (you need to supply): [ ]
LIMITS: [verified / unverified]
```

---

## Sibling skills

- `ig-content-planner` — plan the posts that will fill the grid.
- `ig-caption-writer` — write the pinned "start here" post.
- `ig-humanizer` — audit the bio wording.
- `tt-profile-optimizer`, `threads-profile-optimizer` — same idea on other platforms.

---

## Pre-flight checklist

- [ ] Header test run and reported?
- [ ] Name field carries a searchable topic?
- [ ] Bio within 150 characters, leads with the follower's benefit?
- [ ] One goal-matched link?
- [ ] Highlights ordered by the visitor's next question?
- [ ] Only shown parts scored, no invented proof?
- [ ] Limits verified or labelled?
