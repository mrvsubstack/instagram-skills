---
name: ig-hashtag-strategist
description: "Builds a small, sized Instagram hashtag set for one post — mostly niche tags you can actually rank in, one mid-size, at most one broad — matched to what the post is really about and rotated so it never looks automated. Use this skill whenever the user says things like \"what hashtags should I use\", \"give me hashtags for this post\", \"are 30 hashtags still worth it\", \"my hashtags don't work\", \"find niche hashtags\", or \"hashtag strategy for Instagram\". Not for writing the caption itself (use ig-caption-writer)."
metadata:
  author: Mr V
  version: "1.0"
  group: Instagram
---

# Instagram Hashtag Strategist

You give me the post (caption, carousel topic or Reel subject) and roughly how big your account is. I hand back 3–5 hashtags, each labelled by size and with a one-line reason, plus where to put them.

---

## The core discovery: hashtags are labels now, not lottery tickets

The old play was 30 tags and hope. Today, Instagram mostly uses hashtags to understand **what a post is about** — and has been cutting how many it allows per post. A wall of popular tags doesn't reach more people. It tells Instagram your post is about everything, which is the same as nothing.

The second half: in a tag with millions of posts, a small account's post is buried in minutes. In a tag with 20,000 posts, it can sit near the top for hours.

**Rule: choose a few tags you can actually be seen in, and every one must describe this exact post.**

Check the current hashtag limit with web search before delivering. At the time of writing Instagram caps posts at a handful of tags; label the cap as verified or unverified.

---

## Step 0 — Intake

1. **The post:** caption or a one-line description of the content.
2. **Account size:** under 5k, 5k–50k, or 50k+. Default: under 5k.
3. **Audience** in one line.
4. **Tags they use now**, if any — to spot the ones that are hurting.

---

## Step 1 — Pull the real topics

List 3–5 things the post is genuinely about:
- **The subject** ("pricing design work")
- **The community** ("freelance designers")
- **The format** ("before/after", "tutorial")
- **The outcome** ("earn more")

If a candidate tag doesn't map to one of these, it doesn't go in.

---

## Step 2 — Size each candidate

| Size | Posts using the tag | What it does for you | How many |
|---|---|---|---|
| **Niche** | under ~50k | Where small and mid accounts actually get seen | 2–3 |
| **Mid** | ~50k–500k | Bigger audience, still beatable | 1–2 |
| **Broad** | 500k+ | A category label; you'll be visible for minutes | 0–1 |

Instagram doesn't always show exact counts. Estimate from specificity, and tell the user to confirm by searching each tag in the app.
- Niche tags are specific and long: `#notionforfreelancers`, `#weddingphotographertips`.
- Broad tags are single common words: `#marketing`, `#design`.

**Adjust for account size:**
- Under 5k → lean niche (3 niche, 1 mid, 0 broad).
- 50k+ → can afford 1–2 mid and 1 broad.

---

## Step 3 — Drop the bad ones

Remove, and say why:
1. **Off-topic but popular.** `#love` on a pricing post confuses Instagram about who to show it to.
2. **Engagement-farm tags.** `#follow4follow`, `#like4like`, `#instagood` on a business post.
3. **Tags with signs of being restricted or spammy** — if searching the tag shows few or no recent posts, skip it. Tell the user to check.
4. **Brand tags you don't own**, unless the post is genuinely about that brand.

---

## Step 4 — Assemble and place

- **3–5 total.** Never more than the current cap.
- **Placement:** end of the caption or the first comment. Never mid-sentence.
- **Rotate.** Different niche tags for different topics. One copied block on every post reads as automation.

Rules:
1. **Every tag describes the post.**
   - Bad → `#entrepreneur #success #motivation #business #hustle`
   - Good → `#freelancedesigner #designpricing #brandingtips #freelancetips`
2. **A missing broad tag is fine.** Don't force one.
3. **Keywords in the caption matter too.** Instagram search reads captions. Make sure the main topic words appear naturally in the first lines.

---

## Worked example

**Input:** "Carousel: 4 changes that took my freelance design projects from $900 to $2,400 average. Account: 3,200 followers. Current tags: 28 generic ones like #design #art #creative #instagood."

**Output:**
```
SET (4 tags)
#designpricing          niche   exactly what the post teaches
#freelancedesigner      mid     the community this is for
#brandingtips           niche   adjacent topic your audience searches
#freelancetips          niche   outcome-focused, low churn

DROPPED FROM YOUR OLD SET
#art #creative — off-topic for a pricing post
#instagood — engagement-farm tag
24 others — too broad for a 3.2k account to be seen in

PLACEMENT: end of the caption. Next pricing post: swap #brandingtips for #proposaltips.
CAPTION KEYWORDS: make sure "freelance design" and "pricing" appear in the first 2 lines.
Verify: search each tag in the app and check the post counts and recent activity.
```
(Size labels are estimates until the user checks counts in the app.)

---

## Output format

```
POST: [one line] · ACCOUNT SIZE: [ ] · CAP: [n] (verified / unverified)

SET
[#tag] [niche/mid/broad] [one-line reason]

DROPPED: [tags and why]
PLACEMENT: [end of caption / first comment]
ROTATION NOTE: [what to swap next time]
CAPTION KEYWORDS: [words to include in the first lines]
VERIFY: search each tag in the app to confirm size and recent activity
```

---

## Sibling skills

- `ig-caption-writer` — the caption these tags attach to.
- `ig-carousel-planner` — carousel captions carry the set too.
- `ig-content-planner` — plan tag rotation across the week.

---

## Pre-flight checklist

- [ ] Current hashtag cap checked or labelled unverified?
- [ ] 3–5 tags, never over the cap?
- [ ] Every tag maps to a real topic of this post?
- [ ] Mix leans niche for small accounts?
- [ ] Bad tags dropped with a reason?
- [ ] Sizes labelled as estimates until checked in-app?
- [ ] Rotation note included?
