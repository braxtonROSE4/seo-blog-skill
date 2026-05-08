# Anti-AI-Slop Protocol

AI-generated text has recognizable fingerprints. Readers, editors, and increasingly Google can spot them. This file lists every known AI writing tell and the specific fix.

**Load this file during the final self-check phase (before delivering any draft). Scan every draft against every tell below.**

---

## The 14 AI Writing Tells

**Tell #1: Em-dash overuse (the #1 AI signature)**
- AI models scatter em-dashes everywhere because training data from NYT/Atlantic/Wired overrepresented them
- **Rule:** Max 2-3 em-dashes per 1000 words **in prose paragraphs**. Em-dashes inside tables, bullet lists, and metadata lines don't count — they're structural, not stylistic. When you reach for one in body text, try a period, comma, colon, or parentheses first. Most em-dashes should become periods (for short punchy sentences) or commas (for natural flow).
- **Self-test:** Search the draft for "—". Ignore occurrences inside `| table |` rows and `- bullet` items. If prose count > 3 per 1000 words, rewrite.
- **Common mistake:** An article might have 40 total em-dashes but only 15 in prose, because comparison tables use em-dashes as separator convention. Don't panic at the raw count — count only prose occurrences.

**Tell #2: "Delve" and the AI vocabulary**
- AI models overuse specific words that real writers rarely choose. These words instantly flag content as machine-generated.
- **Banned words:** delve, unpack, multifaceted, myriad, plethora, tapestry, landscape (as metaphor), leverage (as verb), utilize (use "use"), holistic, robust, nuanced (as adjective for nouns), comprehensive, foster, facilitate, harness, underscore, pivotal, paramount, embark, realm, intricate, cutting-edge, groundbreaking, navigate (metaphorical), synergy, paradigm
- **Self-test:** Search the draft for each word. If found, replace with a simpler, more common word.

**Tell #3: Formulaic paragraph structure**
- AI writes paragraphs in a predictable pattern: topic sentence → explanation → example → transition. Every paragraph follows the same shape.
- **Fix:** Vary paragraph structure deliberately. Some paragraphs are just a question. Some are a single sentence. Some start with the example, then give the point. Some are dialogue. Break the pattern every 3-4 paragraphs.

**Tell #4: Perfect grammar and zero contractions**
- AI writing is unnaturally polished. Real humans write "it's" not "it is", "don't" not "do not", "can't" not "cannot".
- **Rule:** Use contractions everywhere a native English speaker would in speech. "It is important" → "It's important". "You should not" → "You shouldn't". The only exception: when the uncontracted form adds deliberate emphasis ("This is *not* a chatbot.").

**Tell #5: Lack of specifics — confident generalities**
- AI makes broad claims that sound authoritative but contain no verifiable details. "Many companies are adopting AI" vs. "Shopify's CEO told employees in April 2025 that teams must prove a task can't be done by AI before requesting new headcount."
- **Rule:** Every claim needs a specific example, a name, a number, or a date. If you can't provide one, cut the sentence.

**Tell #6: Rhetorical mirroring — "It's not about X, it's about Y"**
- AI loves this construction and repeats it multiple times per article. Once is fine. Twice is a pattern. Three times is a tell.
- **Rule:** Max 1 per article. Vary your rhetorical structures.

**Tell #7: List addiction — everything becomes bullets**
- AI defaults to bullet points and numbered lists even when prose would be more readable and engaging.
- **Rule:** Use lists only for genuinely parallel items (feature comparisons, step-by-step instructions, FAQ). Never use bullets for ideas that deserve narrative development. If a point needs 2+ sentences of explanation, it's a paragraph, not a bullet.

**Tell #8: The "comprehensive overview" voice**
- AI writes like an encyclopedia: neutral, balanced, covering all angles equally. This produces content that is informative but has no *point of view*.
- **Fix:** Take a position. Every section should have a verdict. "Here are three approaches" is AI voice. "The third approach is the only one worth your time — here's why" is human voice.

**Tell #9: Emoji bullets in professional content**
- Using emojis as section markers or list bullets, like "key takeaways: ..." or "warning:", or using emojis as list markers. This is a GPT-4o fingerprint.
- **Rule:** Zero emojis in SEO articles. Period.

**Tell #10: Hedging stacks — "may potentially help to possibly..."**
- AI stacks hedge words to avoid making commitments. "This could potentially be useful for some users in certain contexts."
- **Fix:** Be direct. "This works for [specific use case]." If you're genuinely uncertain, say why: "The research is mixed — two studies support this, one contradicts it."

**Tell #11: Missing personal stakes — no skin in the game**
- AI can't share what it lost, risked, or learned the hard way. This absence is the deepest tell.
- **Fix (the Dan Shipper method):** Include at least one real failure, mistake, or uncomfortable truth per article. "We tried this approach for three months. It didn't work." This is the one thing AI genuinely cannot fake.

**Tell #12: Uniform sentence length**
- AI tends to write sentences of similar length (15-20 words), creating a monotonous rhythm. Human writing has wild variation — from 3-word punches to 40-word explorations.
- **Fix:** After writing a draft, check sentence length variation. If most sentences fall in the 12-20 word range, manually add very short sentences (3-7 words) and allow some longer ones (25-35 words).

**Tell #13: The summary conclusion**
- AI always ends with a recap: "In conclusion, we've explored X, Y, and Z. The key takeaway is..."
- **Fix:** Already covered in writing-style.md §4.10 — circle back to the opening scene, or land a gold sentence. Never summarize.

**Tell #14: Symmetric triplets — "X, Y, and Z" on repeat**
- AI loves three-element lists of abstract nouns: "efficiency, scalability, and reliability." "speed, accuracy, and consistency." Twice in an article is fine. Five times is a fingerprint.
- **Rule:** After drafting, search for "`, and`" patterns. If three-element lists appear more than 3 times in the article, break at least half of them: drop to two items, expand one into its own sentence, or replace the list with a single vivid verb.
- **The deeper tell:** The triplets aren't just repetitive — they're vague. "It improves speed, accuracy, and reliability" says nothing. "It cut our pipeline from 45 minutes to 3" says everything.

---

## The Ultimate Anti-AI Test

Read your draft aloud. If it sounds like a news anchor reading a teleprompter — smooth, balanced, authoritative, forgettable — it has AI voice. It should sound like a person talking to a friend, with pauses, emphases, asides, and the occasional rough edge.
