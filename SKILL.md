---
name: seo-article
description: >
  Write SEO-optimized articles that rank on Google AND get cited by AI models
  (ChatGPT, Claude, Perplexity, Google AI Overview), while reading like a human
  wrote them for humans. Covers: definition engineering → article structure →
  narrative writing (Dan Shipper method) → on-page SEO → schema → GEO optimization.
  IMPORTANT: Always invoke /seo-research first to gather SERP data before writing.
  Use when asked to write blog posts, pillar articles, category definition pages,
  comparison articles, or any long-form SEO content.
  Triggers on: "write article", "SEO article", "blog post", "pillar article",
  "category definition", "write content for SEO", "品类定义文", "写 SEO 文章",
  "write a pillar page", "category education content".
user-invokable: true
argument-hint: "<topic or keyword>"
---

# SEO Article Writer

Write articles that satisfy three audiences simultaneously: Google (ranking), AI models (citation), and humans (reading).

## Workflow

### Step 1 — Research (MANDATORY)

Before writing, gather SERP data. Two paths:

- **No prior research:** Invoke `/seo-research [target keyword]` first. Wait for the Research Brief output before proceeding.
- **User provides research:** Accept the existing brief and skip to Step 2.

Never write an article without a Research Brief.

### Step 2 — Definition Engineering

The definition sentence is the single most important sentence in the article. It determines whether AI Overview, ChatGPT, and Perplexity will cite you.

**The formula (derived from highest-citation articles: AWS, NVIDIA, Google ML Glossary):**

```
[X] is a [category noun] that [verb1], [verb2], and [verb3] to [purpose] — [differentiating clause].
```

**Rules:**
- One sentence, 15-30 words
- Three-verb chain (perceive/understand + decide/reason + act/execute)
- End with "on behalf of [user]" or "to [achieve goal]" — highest AI citation rate
- No preamble. Definition IS the first sentence of the article (or paragraph 2 if using a hook opening)
- Include the primary keyword in its exact form

**The definition paragraph (not just the sentence):**

The definition sentence is the GEO citation anchor. But the definition *paragraph* does five jobs:

1. **Definition sentence** (15-30 words, `X is a Y that [verb1], [verb2], [verb3]`)
2. **Boundary line:** What it's NOT, in one contrast. Name the adjacent category and the technical dividing line. ("Not a chatbot that generates text about your tasks, but an agent that executes them: books the meeting, sends the email, writes code when no pre-built tool exists.")
3. **Modifier unpacking:** If the term is `[modifier] [noun]` (e.g., "personal agent"), unpack the modifier with 2-3 concrete specifics. Don't just say the modifier matters — show what it adds.
4. **Flywheel or mechanism:** One sentence naming the core value loop. This is what makes the reader think "oh, that's why this category exists."
5. **Verdict sentence** (2-5 words): crystallize the whole paragraph. ("That flywheel is the product.")

The definition sentence is for AI citation. The definition paragraph is for human conviction. Both matter.

**Disambiguation (if term has multiple meanings):**
- Within first 100 words, acknowledge other meanings in one sentence
- Use parenthetical: "(In entertainment, a personal agent is a talent rep. This guide covers the technology definition.)"

### Step 3 — Concept Precision Check (for technical categories)

When writing about a technology category (AI agents, cloud computing, blockchain, etc.), lock down the core terms before drafting. Imprecise terminology produces imprecise articles.

**For each core term in the article:**
1. **Write a 1-sentence technical definition** from first principles (e.g., "An agent is an LLM that can call tools and execute tasks in a loop, not just generate text")
2. **Identify the boundary:** What's the single thing that separates this term from its nearest neighbor? (Agent vs chatbot: tool calling. Personal agent vs AI agent: persistent user context.)
3. **Lock the usage rule:** Is the term a product name, a technical architecture, or a category label? These get used differently. ("Manus is a product. Agent is the engine behind it. Personal agent is the category.")

Run this check against every instance of the core terms in the draft. If a sentence uses the term in a way that contradicts the locked definition, fix it. This is especially critical for articles defining a category, where a single imprecise sentence can undermine the entire piece.

### Step 4 — Article Structure

Structure is for Google and AI systems. It determines what gets indexed, extracted, and appears as rich results.

**H1 (on-page heading):**
```
What Is [X]? Definition, Examples, and How It Works [Year]
```
- Primary keyword in exact form
- Can be longer than 60 characters — this is the visible page heading, not the SERP title
- Year tag for freshness signal (on time-sensitive topics)

**Title Psychology (derived from Every.to's highest-performing patterns):**

Before optimizing for character count, nail the *psychology* of the title:

| Pattern | Formula | Example |
|---------|---------|---------|
| **Contrarian hook** | [Popular belief as premise] + [flip] | "If SaaS Is Dead, Linear Didn't Get the Memo" |
| **Qualified verdict** | [Strong judgment] + [limitation in parens] | "The Best Coding Model We've Tested (With Some Maddening Habits)" |
| **Personal narrative hook** | "What I Learned/Stopped/Discovered" + [doing X] | "What I Learned Onboarding Our AI Project Manager" |
| **Provocative reframe** | [Familiar concept] + [unexpected new frame] | "The Knowledge Economy Is Over. Welcome to the Allocation Economy." |

**`<title>` tag (SERP title) — DIFFERENT from H1:**

- **Under 55-60 characters** (Google truncates at ~580px)
- **NO brand suffix** — wastes 8-15 characters that should be keywords
- **Primary keyword as close to beginning as possible**

| Article Type | Formula | Example |
|-------------|---------|---------|
| Definition / Pillar | `What Is [X]? [Value Hook] [Year]` | `What Is a Personal Agent? Definition & Guide [2026]` |
| Comparison | `[X] vs [Y]: [Core Difference] [Year]` | `Personal Agent vs AI Browser: Key Differences` |
| Educational | `How [X] Works: [Hook]` | `How Personal Agents Work: Architecture Explained` |
| History / Trend | `[Topic]: [Narrative Hook] [Year]` | `History of Personal Agents: 1995 Vision to 2026 Reality` |
| Review / Roundup | `Best [X] in [Year]: [Qualifier]` | `Best Personal Agents in 2026: Tested & Compared` |

**Meta description:**
- **120-155 characters**, complete sentence, includes primary keyword
- Functions as click-through pitch: "why should I read this over the 9 other results?"
- Formula: `[Definition or core answer, ~80 chars] + [Value differentiator, ~60 chars]`
- No brand name unless brand IS the topic. No quotes or special characters.

**H2 headings — ALL as questions:**
```
## What is [X]?
## Why does [X] matter?
## How does [X] work?
## What are the core capabilities of [X]?
## How is [X] different from [Y]?
## What can [X] actually do?
## Who is building [X] in [Year]?
## What are the challenges and limitations?
## How do you choose [X]?
## What is the future of [X]?
## FAQ
```

Question-format H2s align with highest-cited articles in AI Overview (AWS, NVIDIA, Google Cloud) and match "People Also Ask" queries directly.

**Mandatory structural elements:**
- Table of Contents with anchor links (before first H2)
- At least 2 comparison tables (against competitors/adjacent categories)
- At least 1 evaluation/criteria table
- **Table humanization rule:** Never drop a table cold. Every table needs a 1-2 sentence narrative intro that tells the reader *what to look for* and *why it matters*. The table delivers data; the intro delivers meaning.
- **Comparison table precision rule:** For each column in a comparison table, state both what the category CAN do and what it CANNOT do. "Answers questions in a conversation" is incomplete. "Answers questions in a conversation. No tool access, no task execution" draws a boundary. The absence is often more informative than the presence.
- **Product list framing rule:** Before any list of products, companies, or examples, establish the conceptual framework that organizes them. Never drop a bullet list cold. One sentence that teaches the reader the organizing principle. ("The products below are built on agents: LLMs that call tools, execute tasks, and operate in loops. The product is the interface. The agent is the engine.")
- FAQ section with 10+ Q&As
- "Challenges and Limitations" section (E-E-A-T signal — 7 of 8 top-ranking definition articles have this)
- Related Reading links (3-5 internal links at bottom)

**Schema markup:**
- `Article` (author, datePublished, dateModified, publisher, wordCount)
- `BreadcrumbList`
- `Organization`
- **NOT** `FAQPage` (restricted to government/healthcare since Aug 2023 — keep FAQ content for AI citation value)

**Progressive Disclosure Principle:**

| Reader time | What they get | How to achieve it |
|-------------|--------------|-------------------|
| 5 seconds | Core conclusion | H1 + subtitle tell the full story |
| 30 seconds | Nuanced judgment | First paragraph gives qualified verdict |
| 2 minutes | One complete perspective | Each H2 section is independently valuable |
| 5 minutes | Key comparisons + data | Tables, bullets, verdict sentences are scannable |
| 15 minutes | Full deep analysis | Complete article with narrative arc |

Never bury the conclusion. Lead with the verdict. Let the article *justify* the opening claim.

### Step 5 — Writing Style (Dan Shipper Method)

Load `references/writing-style.md` for the complete style guide.

**Core principle:** Write like a builder who just came back from the front line — with data, with scars, with thoughts about the bigger picture.

**Key rules (always in memory — no need to load reference for these):**
- First paragraph: 3 sentences max, personal micro-scene preferred
- Definition sentence goes in paragraph 2
- 30%+ of all paragraphs should be single-sentence paragraphs
- Every analytical passage ends with a verdict sentence (2-5 words)
- Conversational transitions only ("Here's what I mean." not "Furthermore")
- Max 2-3 em-dashes per 1000 words — overuse is the #1 AI writing tell
- At least 2 vivid verbs per section (not generic be/have/get/make/do)
- Person switching: narrative "I" → analytical "You/We" → conclusion "I"

**Load `references/writing-style.md`** for: the three opening moves, sentence rhythm targets, paragraph patterns, transitions list, voice toolkit, metaphor rules, section opening techniques, narrative arc, endings, and the full blacklist.

### Step 6 — On-Page SEO

**Keyword placement (primary keyword):**
- Title tag: exact match
- H1: exact match or close variant
- URL slug: exact match, hyphenated
- First paragraph: within first 100 words
- Multiple H2 headings: natural inclusion
- Image alt text: at least 2 images
- Last paragraph / conclusion

**Keyword density:** 1-2% natural occurrence. Never force it.

**Internal links:** 3-5 per 1000 words. Anchor text uses primary or related keywords. Every article links to its topic cluster pillar page.

**External links:** 5-10 to authoritative sources (Wikipedia, official docs, research papers). Opens in new tab. Establishes E-E-A-T.

**CTA strategy:**
- 3-4 inline CTAs per article, spaced every 800-1200 words
- Placement: always AFTER a "problem → solution" passage, never random
- Progressive commitment: "Learn more" → "Try it" → "Sign up"
- All CTA URLs: `?from=blog-[slug]`
- Category education phase: emphasize category word, not brand ("See how a personal agent handles this" > "Try [Brand] for free")

**Open Graph tags:** `og:title`, `og:description` (up to 200 chars), `og:image`, `og:url`

### Step 7 — GEO (Generative Engine Optimization)

GEO determines whether AI models (ChatGPT, Claude, Perplexity, Google AI Overview) cite your article when answering user questions. SEO gets you ranked. GEO gets you quoted.

**GEO citation priority (what AI models extract, in order):**

| Priority | Element | How to optimize |
|----------|---------|-----------------|
| 1 | Definition paragraph | Follow the 5-step definition paragraph architecture (Step 2). Self-contained, precise, quotable. This is what gets cited when someone asks "what is X?" |
| 2 | FAQ answers | First sentence IS the answer, restating the question's core terms. Include current data (dates, numbers, product names). Keep to 2-4 sentences for citation-friendly length. |
| 3 | Comparison tables | Column headers should mirror search intent phrasing ("What it does" beats "Core function"). Each cell states both what the category CAN and CANNOT do. |
| 4 | Verdict sentences | Sentences under 15 words with a specific name, number, or date get cited far more than general statements. |
| 5 | H2 section openers | First sentence of every H2 section should pass the "standalone quote" test: meaningful without surrounding context. |

**Self-contained blocks:**
- Every H2 section must be independently understandable and citable without context from other sections
- **GEO atomic test:** Take any section out of context. Can it be cited as a standalone answer? If not, add a framing sentence at the top.

**Citable patterns (what AI models cite most):**
1. Definition sentence in `X is a Y that does Z` format
2. Comparison tables with clear, search-intent-aligned column headers
3. Short declarative statements with specific facts/numbers
4. FAQ answers that start with the question's keywords
5. "Not X, but Y" contrast statements that draw category boundaries

**FAQ as GEO weapon:**
FAQ answers are the second-highest citation target after the definition. Optimize each one:
- First sentence directly answers the question (zero preamble)
- Include the most recent verifiable data point (date, price, market size, product launch)
- Keep answers to 2-4 sentences for citation-friendly length
- Link to authoritative sources within answers for E-E-A-T

### Step 8 — Meta Output Block (MANDATORY)

Every article ends with a `<!-- SEO Meta -->` block after Related Reading:

```
<!-- SEO Meta
meta_title: "[under 60 chars, no brand suffix]"
meta_description: "[120-155 chars, includes primary keyword, compelling sentence]"
h1: "[on-page heading, can be longer than title tag]"
og_title: "[same as meta_title or slightly adapted for social]"
og_description: "[same as meta_description or adapted, up to 200 chars]"
canonical_url: "https://ego.app/blog/[slug]"
primary_keyword: "[exact match keyword]"
secondary_keywords: "[comma-separated list]"
date_published: "[YYYY-MM-DD]"
date_modified: "[YYYY-MM-DD]"
-->
```

**Hard rules:**
1. `meta_title` ≠ `h1` (title is SERP-optimized, H1 is page-optimized)
2. `meta_title` must NOT contain brand name, "| ego", "- ego Blog", or any suffix. Zero exceptions.
3. `meta_description` must be complete sentence, 120-155 characters, includes primary keyword.

### Step 9 — Anti-AI-Slop Check

Load `references/anti-ai-slop.md`. Scan every draft against all 14 tells before delivery.

**Quick-check (always in memory):**
- Em-dashes: max 2-3 per 1000 words
- Zero banned AI vocabulary (delve, unpack, tapestry, leverage, holistic, robust, comprehensive, foster, harness, pivotal, embark, synergy, paradigm...)
- Contractions used naturally throughout
- Every claim has a specific name, number, or date
- At least 1 real failure/mistake/uncomfortable truth per article
- Read aloud test: must sound like a person, not a news anchor

---

## Word Count Guidelines

| Article Type | Target | Principle |
|-------------|--------|-----------|
| Pillar / category definition | 3,500-5,000 | Only type that justifies 3,500+. Most comprehensive resource. |
| Comparison ("X vs Y") | 1,800-2,500 | One comparison per article. |
| "Third road" ("X vs Y: Why Z") | 2,000-2,500 | 60% fair comparison, 40% introducing third option |
| Educational / how-to | 2,000-2,500 | One core insight. Split if exceeding 2,500. |
| Review / roundup | 2,500-3,500 | 300-400 words per product reviewed |
| Trend / landscape | 2,000-2,500 | Sharp opinions, specific signals |
| Scenario / narrative | 1,800-2,500 | Story drives structure |

**Split rule:** Any article (except pillar) exceeding 3,000 words with 2+ core arguments → split and interlink.

## Education:Promotion Ratio

| Stage | Ratio | When |
|-------|-------|------|
| New category (no definition exists) | 80:20 | First 20 articles |
| Growing category (definition established) | 70:30 | Articles 20-50 |
| Mature category (competitive SERP) | 65:35 | 50+ articles |

## Article Type Templates

### Pillar / Definition Article
```
[Hook paragraph — scenario the reader recognizes]
[Definition paragraph — formal definition + boundary-setting]

## Table of Contents
## Why does [X] matter?
## How does [X] work?
  [Scene opening → technical explanation wrapped in analogy]
  [Comparison table: your approach vs standard approach]
## What are the core capabilities?
  [Table: capability | meaning | without it you get...]
## How is [X] different from [adjacent categories]?
  [Full comparison table]
## What can [X] do? [Examples]
## Who is building [X]?
## Challenges and limitations
## How to choose
  [Evaluation table]
## Future
## FAQ (10-12 Q&As)
[Related Reading: 3-5 internal links]
<!-- SEO Meta ... -->
```

### Comparison Article ("X vs Y")
```
[Hook — the confusion most people have]
[One-line thesis: the core difference]

## What is [X]?
## What is [Y]?
## [X] vs [Y]: key differences
  [Comparison table + subsections by dimension]
## When to use [X] vs [Y]
## FAQ
[Related Reading]
<!-- SEO Meta ... -->
```

### Third-Road Article ("X vs Y: Why You Need Z")
```
[Hook — the false dilemma]

## What is [X]?
## What is [Y]?
## [X] vs [Y] compared [Fair, thorough comparison]
## The shared limitation
  [Both fail at the same thing — set up the pivot]
## A different approach: [Z]
  [Your category/product enters as the resolution]
## FAQ
[Related Reading]
<!-- SEO Meta ... -->
```

---

## Checklist (Run Before Publishing)

### Content Quality
- [ ] Hook in first paragraph — not a summary, not a definition-first opening
- [ ] Definition sentence follows `X is a Y that [verb1], [verb2], [verb3]` pattern
- [ ] Definition paragraph covers all 5 jobs: definition sentence, boundary line, modifier unpacking, flywheel, verdict
- [ ] Concept Precision Check passed (for technical categories): core terms locked with 1-sentence definition, boundary, and usage rule
- [ ] Disambiguation within first 100 words (if term has multiple meanings)
- [ ] All H2s are questions
- [ ] At least 2 comparison tables, each with narrative intro
- [ ] Comparison tables state both CAN and CANNOT for each column
- [ ] Product lists/examples prefaced with a conceptual framework sentence
- [ ] "Challenges and Limitations" section present
- [ ] FAQ with 10+ Q&As
- [ ] Each section passes GEO atomic test (citable independently)
- [ ] No "In today's rapidly evolving..." or similar AI-sounding phrases
- [ ] Short verdict sentences present (2-5 words after longer passages)

### SEO
- [ ] Primary keyword in: title tag, H1, URL, first 100 words, 3+ H2s, alt text
- [ ] `<title>` tag under 60 characters, NO brand suffix, keyword front-loaded
- [ ] `<title>` tag is DIFFERENT from H1
- [ ] Meta description: 120-155 characters, complete sentence, includes primary keyword
- [ ] Meta description is NOT a repeat of the title tag
- [ ] TOC with anchor links
- [ ] 3-5 internal links per 1000 words
- [ ] 5-10 external links to authoritative sources
- [ ] 3-4 inline CTAs with tracking parameters
- [ ] Related Reading (3-5 links) at bottom
- [ ] `datePublished` and `dateModified` present
- [ ] **Meta Output Block** appended after Related Reading (Step 7)

### Schema
- [ ] Article schema (author, dates, publisher, wordCount)
- [ ] BreadcrumbList schema
- [ ] Organization schema

### Style (The Dan Shipper Test)
- [ ] First paragraph: 3 sentences max, uses personal micro-scene / poetic abstraction / provocative assertion
- [ ] 30%+ of paragraphs are single-sentence paragraphs
- [ ] Every analytical passage ends with a verdict sentence (2-5 words)
- [ ] At least 3 parenthetical asides with self-deprecating humor
- [ ] At most 2-3 em-dashes per 1000 words
- [ ] All data expressed as precise numbers — zero vague adjectives
- [ ] At least 3 analogies from everyday domains (food, body, school, relationships)
- [ ] Technical concepts: everyday analogy → parenthetical definition → immediate example
- [ ] At least 2 vivid verbs per section (not generic be/have/get/make/do)
- [ ] Zero academic transition words (Furthermore/Moreover/In addition/Additionally)
- [ ] Zero "You should..." sentences
- [ ] Ending: circles back to opening scene or lands a quotable gold sentence
- [ ] Person switching: narrative "I" → analytical "You/We" → conclusion "I"

### Anti-AI-Slop (run after every draft)
- [ ] Em-dash count: max 2-3 per 1000 words **in prose only** (exclude tables, bullet labels, meta lines)
- [ ] Zero banned AI vocabulary (delve, unpack, multifaceted, myriad, tapestry, leverage, utilize, holistic, robust, comprehensive, foster, facilitate, harness, underscore, pivotal, paramount, embark, realm, intricate, cutting-edge, groundbreaking, navigate, synergy, paradigm)
- [ ] Contractions used naturally throughout ("it's" not "it is", "don't" not "do not")
- [ ] Every claim has a specific name, number, or date — no confident generalities
- [ ] Max 1 "It's not about X, it's about Y" construction per article
- [ ] Lists/bullets only for genuinely parallel items — narrative ideas stay in prose
- [ ] Every section has clear point of view / verdict — not a neutral overview
- [ ] Zero emojis
- [ ] Zero hedge stacks ("may potentially help to possibly...")
- [ ] At least 1 real failure/mistake/uncomfortable truth per article
- [ ] Sentence length varies wildly (3-word punches mixed with 30-word explorations)
- [ ] Symmetric triplet check: no more than 3 "X, Y, and Z" three-element lists in the article
- [ ] Read the draft aloud — if it sounds like a news anchor, rewrite
