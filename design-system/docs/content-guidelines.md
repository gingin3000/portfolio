---
title: UX Content Guidelines
description: Principles and practices for writing accessible, clear UX content
version: 1.0.0
category: content
last_updated: 2026-07-19
---

# UX Content Guidelines

Clear, accessible UX content built on five core principles. Use these guidelines when writing copy for your portfolio or any public-facing UX content.

---

## Core Principles

### Principle 1: Lead with the problem, not the solution
**Description:** Describe what was broken first, then show how you fixed it. This anchors the reader in *why* the work mattered.

**Tags:** `problem-first` `clarity` `context`

**Do:**
```
Users thought they were answering a security question—but were actually signing up for an account. 
I rewrote the copy to make it clear.
```

**Don't:**
```
We improved clarity by reworking the signup flow.
```

---

### Principle 2: Be specific and concrete
**Description:** Use real examples, numbers, and actual user behaviors instead of abstract statements. Show, don't tell.

**Tags:** `specificity` `data-driven` `examples`

**Do:**
```
40% of pages were buried 5–6 levels deep and rarely found.
```

**Don't:**
```
The information architecture was disorganized.
```

---

### Principle 3: Write for mixed audiences
**Description:** Your reader might be a fellow designer, a hiring manager, a developer, or someone unfamiliar with your domain. Assume no shared jargon; define terms upfront if they're necessary.

**Tags:** `accessibility` `clarity` `audience-aware`

**Do:**
```
I wrote a spec first—defining what the feature should do before building—to prevent scope creep.
```

**Don't:**
```
I employed SDD principles to optimize the delivery pipeline.
```

---

### Principle 4: Explain the "why," not just the "what"
**Description:** Don't just say what you did. Say why it mattered to the user, the business, or the team.

**Tags:** `context` `impact` `reasoning`

**Do:**
```
I reduced onboarding from four screens to one, which cut support requests about the feature.
```

**Don't:**
```
We consolidated the onboarding screens.
```

---

### Principle 5: Use positive framing
**Description:** Describe what users *can* or *will* do, not what they can't. This is especially important in error states or limitations.

**Tags:** `tone` `user-empathy` `framing`

**Do:**
```
Users can now verify the site's legitimacy before entering payment information.
```

**Don't:**
```
Users won't get scammed or Users can't be fooled by fake sites.
```

---

## Voice & Tone

### Be direct and concise
**Description:** Use short sentences mixed with slightly longer explanatory ones. Cut redundancy ruthlessly. If you've said it twice, delete one.

**Tags:** `conciseness` `clarity` `brevity`

**Do:**
```
The flow packed three tasks into one screen. I separated them: one task per screen.
```

**Don't:**
```
The user flow was attempting to accomplish multiple objectives concurrently, which created cognitive overload. 
We distributed information across multiple screens.
```

**Guidelines:**
- Aim for average sentence length of 12–15 words
- Use one idea per sentence
- Delete words that don't add meaning

---

### Avoid hedging language
**Description:** Say "this caused X" not "this may have possibly caused X." You're describing your own work; you know what you did.

**Tags:** `confidence` `clarity` `directness`

**Do:**
```
Shorter copy made the call-to-action stand out.
```

**Don't:**
```
The shortened copy potentially might have helped reduce visual weight.
```

---

### Use active voice
**Description:** Keep the focus on actions and people, not abstract nouns.

**Tags:** `active-voice` `clarity` `human-centered`

**Do:**
```
I worked with legal to find compliant, user-friendly wording.
```

**Don't:**
```
Collaboration with legal resulted in compliant language that maintained usability.
```

---

## Structure

### Start with context, not details
**Description:** Give the reader just enough background to understand what mattered.

**Tags:** `context` `scoping` `clarity`

**Do:**
```
Users wanted a way to verify site legitimacy, but our first design was confusing about what they were creating and why. So I...
```

**Don't:**
```
We discovered through extensive user research conducted across three regions using mixed methods...
```

---

### Use lists and hierarchies liberally
**Description:** When you have multiple points, use bullets or structured sections. Prose walls are harder to scan.

**Tags:** `scannability` `structure` `accessibility`

**Do:**
- Point A and the reasoning
- Point B and the reasoning  
- Point C and the reasoning

**Don't:**
```
A paragraph where all three points are tangled together.
```

---

### Break long sections with subheadings
**Description:** If your case study section is more than 3–4 paragraphs, add a subheading to help the reader navigate.

**Tags:** `structure` `navigation` `accessibility`

**Guidelines:**
- Use heading hierarchy consistently (H2 for sections, H3 for subsections)
- Keep heading text under 60 characters
- Use imperative verbs when possible ("Build," "Analyze," "Test")

---

## Accessibility & Cognitive Load

Some people process information better when it's structured, explicit, and doesn't demand extra cognitive effort. Many of the principles above already support this. Here's how to go further.

### Keep paragraphs short
**Description:** Aim for 2–3 sentences per paragraph. Long blocks of text are harder to process for some people.

**Tags:** `accessibility` `cognitive-load` `readability`

**Do:**
```
I conducted five user interviews. Most users didn't understand the first screen. So I rewrote the copy and tested again.
```

**Don't:**
```
I conducted five user interviews which revealed that most users didn't understand the first screen, so I rewrote the copy and tested again with a second round of participants.
```

**Guidelines:**
- Max 3 sentences per paragraph
- One idea per paragraph
- White space between ideas

---

### Use explicit structure
**Description:** Don't make readers infer the organization. Use headings, lists, and white space to make the structure visible.

**Tags:** `accessibility` `structure` `clarity`

**Do:**
- Use a heading
- Use a bullet list
- Use clear section breaks

**Don't:**
- Write in flowing prose where the reader has to figure out where one idea ends and another begins

---

### Avoid double meanings and idioms
**Description:** Phrases like "the ball is in your court" or "thinking outside the box" are confusing for some people. Say what you mean directly.

**Tags:** `accessibility` `clarity` `directness`

**Do:**
```
I need your feedback by Friday.
```

**Don't:**
```
The ball is in your court—let's see what you think.
```

---

### Use high contrast between sections
**Description:** Add visual breaks (white space, dividers, or formatting changes) to signal that a new idea is starting. This helps some people track where they are.

**Tags:** `accessibility` `visual-hierarchy` `structure`

**Do:**
- Use spacing, subheadings, and visual hierarchy intentionally

**Don't:**
- Run everything together without visual markers

---

### Be explicit about what comes next
**Description:** Don't assume readers will infer the next step. Say it.

**Tags:** `clarity` `guidance` `structure`

**Do:**
```
Here's what I found. Next, I tested my fix with five more users.
```

**Don't:**
```
Here's what I found.
```

---

### Avoid ambiguous pronouns
**Description:** When you use "it," "this," or "they," make sure it's crystal clear what you're referring to. Don't make readers scroll back to figure it out.

**Tags:** `clarity` `accessibility` `reference`

**Do:**
```
The signup flow was confusing. I simplified it by splitting the form into two screens.
```

**Don't:**
```
The signup flow was confusing. I simplified it.
```

---

### Define acronyms every time
**Description:** Even if you've used an acronym before, define it again in a new section or paragraph. Readers don't retain acronyms well, and context-switching costs cognitive energy.

**Tags:** `accessibility` `clarity` `reference`

**Do:**
```
I used spec-driven development (SDD—writing a spec before building) to prevent scope creep.
```

**Don't:**
```
As discussed earlier, I used SDD to prevent scope creep.
```

---

### Break up lists of more than three items
**Description:** Long lists are hard to scan. If you have more than 3–4 bullet points, consider grouping them under subheadings or breaking them into multiple lists.

**Tags:** `scannability` `accessibility` `structure`

**Do:**
```
**What I tested:** Copy clarity, button placement, flow length.
```

**Don't:**
```
A 10-item bullet list in one block.
```

---

## Common Pitfalls to Avoid

| Pitfall | Why it's a problem | Fix |
|---------|-------------------|-----|
| **Overselling** | "Best-in-class" and "revolutionary" weaken your credibility | Let the specifics speak for themselves |
| **Hiding tradeoffs** | Readers can sense when you're leaving something out | Name the tradeoff you made and why |
| **Claiming unearned credit** | Taking credit for team work damages trust | Say "the team" or "I collaborated with X" |
| **Placeholder examples** | "For example, if a user..." is weaker than real data | Use actual quotes or numbers from your work |
| **Over-explaining process** | Readers don't care how you worked unless it's interesting | Focus on the outcome and the thinking |

---

## Pre-Publication Checklist

Use this checklist before publishing any content:

- [ ] **Problem is clear** in the first 1–2 sentences
- [ ] **"Why" is explained**, not just "what"
- [ ] **No jargon unexplained** or clearly defined
- [ ] **Specific example or number** included
- [ ] **No redundant phrases** or repeated ideas
- [ ] **Tone is direct, practical, thoughtful**—not formal or sales-y
- [ ] **Paragraphs are short** (2–3 sentences max)
- [ ] **Pronouns are clear** (no scrolling back needed)
- [ ] **Acronyms are defined** on first use in each section
- [ ] **Structure is visible** (headings, lists, white space)

---

## Example: Before & After

### Before
```
I conducted extensive user research which revealed pain points in the authentication flow. 
Subsequently, I redesigned the copy to improve comprehension and reduce user confusion. 
The implementation resulted in positive outcomes.
```

**Issues:** Vague, hedging, no specifics, passive voice, too formal

### After
```
Users were confused about what they were signing up for. 
I rewrote the copy to explain each step upfront and split the form into two stages. 
This reduced support requests by 30%.
```

**Improvements:** Specific problem, concrete solution, measurable outcome, active voice, direct tone


