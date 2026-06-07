---
name: microsoft-writing-style
description: >
  Review and rewrite content for compliance with the Microsoft Writing Style Guide.
  Enforces voice principles (warm, crisp, ready to help), bias-free language,
  sentence-style capitalization, Oxford commas, scannable structure, and global-ready
  writing. Use when reviewing docs, UI text, blog posts, release notes, or any
  technical communication that should follow Microsoft style.
license: Apache-2.0
metadata:
  author: iemejia
  version: "1.0"
  source: https://learn.microsoft.com/en-us/style-guide/welcome/
---

# Microsoft Writing Style Guide compliance

Use this skill to review, edit, or write content that follows the
[Microsoft Writing Style Guide](https://learn.microsoft.com/en-us/style-guide/welcome/).

## When to activate

- User asks to "review for Microsoft style" or "apply Microsoft style guide"
- Content is destined for Microsoft documentation, UI, blog, or marketing
- User asks for writing feedback referencing voice, tone, capitalization, or inclusive language

## Review workflow

1. Read the content provided by the user.
2. Evaluate against each rule category below (voice, word choice, capitalization, punctuation, structure, bias-free, global readiness).
3. For each violation found, output:
   - The original text (quoted)
   - The rule violated (with a short explanation)
   - A suggested rewrite
4. After all violations, provide a clean rewritten version if the user requests one.

## Top 10 rules (quick reference)

1. **Use bigger ideas, fewer words.** Shorter is always better.
2. **Write like you speak.** Read your text aloud. If it sounds stilted, rewrite it.
3. **Project friendliness.** Use contractions: *it's, you'll, you're, we're, let's.*
4. **Get to the point fast.** Lead with the key takeaway. Front-load keywords.
5. **Be brief.** Give customers just enough info to decide confidently. Prune excess words.
6. **When in doubt, don't capitalize.** Use sentence-style capitalization everywhere except proper nouns and product names.
7. **Skip periods on headings and short list items.** Save periods for body copy.
8. **Use the Oxford comma.** In a list of three or more, include a comma before the conjunction.
9. **Don't be spacey.** One space after periods. No spaces around em dashes.
10. **Revise weak writing.** Start with a verb. Edit out *you can* and *there is/are/were.*

## Voice principles

The Microsoft voice is **warm and relaxed**, **crisp and clear**, and **ready to lend a hand**.

- Be natural and conversational, not formal or stiff.
- Adapt tone to context (serious for errors, celebratory for success) while keeping voice constant.
- Focus on the customer: anticipate needs, offer information at the right time, get out of the way.

For detailed guidance, see [references/voice-and-tone.md](references/voice-and-tone.md).

## Word choice

- Use simple, everyday words. Prefer short words over long ones.
- Use contractions (*don't, isn't, you're*) to sound natural.
- Don't use jargon or acronyms without defining them.
- Don't use common words in new ways that confuse readers.
- Use technical terms carefully — define them on first use if the audience may not know them.
- Use US spelling. Avoid non-English words when an English alternative exists.
- Be consistent: if you mean the same thing, use the same word.

## Capitalization

- **Default to sentence-style capitalization**: capitalize only the first word and proper nouns.
- Never use title-style capitalization in headings, titles, or UI labels (unless it's a product name).
- Don't use ALL CAPS for emphasis.
- Don't capitalize the spelled-out form of an acronym unless it's a proper noun.
- Capitalize the word after a slash if the word before the slash is capitalized.

## Punctuation

- **Oxford comma**: always include the serial comma (*Android, iOS, and Windows*).
- **Periods**: skip them on headings, subheadings, and short list items (three words or fewer).
- **Em dashes**: use without spaces (*word—word*), not spaced en dashes.
- **One space** after periods, question marks, and colons.
- **Exclamation points**: use sparingly. One per document is a good rule of thumb.
- **Semicolons**: avoid when possible; prefer two shorter sentences.

For detailed rules, see [references/punctuation-and-formatting.md](references/punctuation-and-formatting.md).

## Scannable content

- **Put first things first.** Lead with what's most important. Front-load keywords.
- **Use headings liberally.** Break content into discrete, scannable sections.
- **Keep paragraphs short.** Three to seven lines maximum.
- **Use bulleted lists** for related items without sequence; numbered lists for steps.
- **Use tables** to present structured data or comparisons.
- **Establish patterns.** Consistent structure helps readers scan faster.

## Bias-free communication

- Use gender-neutral alternatives (*chair* not *chairman*, *workforce* not *manpower*).
- Don't use gendered pronouns in generic references. Rewrite to use *you*, plurals, or role-based nouns.
- It's OK to use *they/their* as a singular generic pronoun.
- Use a person's preferred pronouns when writing about real individuals.
- Represent diverse perspectives in examples and scenarios.
- Avoid slang, profanity, and terms with unconscious racial or military bias.
- Use *primary/subordinate* not *master/slave*; *stop responding* not *hang*.
- Focus on people, not disabilities. Don't mention disability unless relevant.

For the complete reference, see [references/bias-free-communication.md](references/bias-free-communication.md).

## Global communications

- Assume content will be read worldwide and may be translated or localized.
- Use simple sentence structures that translate well.
- Avoid idioms, colloquialisms, and culturally specific references.
- Don't make generalizations about people, countries, or cultures.
- Use equivalent geographic references (don't mix countries with states).
- Verify that named cities/regions aren't politically disputed.

For the complete reference, see [references/global-communications.md](references/global-communications.md).

## Grammar and usage

- Use **present tense** as the default.
- Use **active voice** unless passive avoids blaming the user or is less awkward.
- Use **imperative mood** for instructions; **indicative** for explanations.
- Use second person (*you*) to address readers; first person plural (*we*) for the organization.
- Spell out zero through nine; use numerals for 10+. Always use numerals for measurements, percentages, and times.
- Spell out acronyms on first use; don't introduce acronyms used only once.

For detailed rules, see [references/grammar-and-usage.md](references/grammar-and-usage.md).

## Developer content and procedures

- Brand voice still applies to developer docs.
- Use code font for code elements, bold for UI elements, italic for placeholders.
- Code examples should be concise, tested, secure, and reusable.
- Write step-by-step instructions with numbered lists; use imperative verbs.
- Use input-neutral verbs (*select* not *click*) to support all abilities.
- Abbreviate navigation with angle brackets: **Settings** > **Accounts** > **Email**.

For detailed rules, see [references/developer-content.md](references/developer-content.md).

## Accessibility and AI writing

- Write brief, meaningful text optimized for screen readers.
- Use heading hierarchy (not formatting) to convey structure.
- Don't rely on directional terms alone for location.
- Spell out special characters (*and* not +, *about* not ~).
- Document all input methods; use input-neutral verbs.
- For bots: keep messages short, be transparent about AI, provide graceful fallbacks.

For detailed rules, see [references/accessibility-and-ai.md](references/accessibility-and-ai.md).

## Content planning and publishing

- Plan content by defining audience, goals, format, discoverability, and success metrics.
- Front-load keywords in headings, summaries, and link text for SEO.
- Write for responsive/mobile: short text, simple visuals, limited table columns.
- Run a final publishing checklist before shipping.

For detailed rules, see [references/content-planning-and-publishing.md](references/content-planning-and-publishing.md).

## A–Z word list and term collections

The Microsoft Writing Style Guide includes an extensive A–Z word list and 12 term collections. When reviewing specific terminology, consult these resources:

- [A–Z word list](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/a-z-word-list) — hundreds of entries with approved usage
- **Term collections**: [Accessibility](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/accessibility-terms), [AI and bot](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/ai-bot-terms), [Bits and bytes](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/bits-bytes-terms), [Cloud-computing](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/cloud-computing-terms), [Computer and device](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/computer-device-terms), [Date and time](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/date-time-terms), [Keys and keyboard shortcuts](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/keys-keyboard-shortcuts), [Mouse and mouse interaction](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/mouse-mouse-interaction-terms), [Security](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/security-terms), [Special characters](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/special-characters), [Touch and pen interaction](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/touch-pen-interaction-terms), [Units of measure](https://learn.microsoft.com/en-us/style-guide/a-z-word-list-term-collections/term-collections/units-of-measure-terms)

### Key terminology rulings (recent updates)

| Term | Ruling |
|------|--------|
| plugin | One word (not plug-in) |
| timeout | One word (not time-out) |
| real-time (adj) | Hyphenated as adjective; two words as noun (*in real time*) |
| pane | Use *pane* (not *blade*); preposition is *in* |
| blacklist / whitelist | Use *block list* / *allow list* (two words) |
| enable / disable | Avoid when possible; prefer specific actions |
| front end / back end | Two words as nouns; hyphenate as adjectives (*front-end server*) |
| white paper | Two words |
| screen reader | Two words, lowercase |
| navigate | Use for moving between locations; don't use for scrolling |
| anti-malware | Hyphenated |
| opt in / opt out | Two words as verbs; hyphenate as adjectives (*opt-in checkbox*) |

## Example transformations

| Before | After | Rule |
|--------|-------|------|
| If you're ready to purchase Office 365 for your organization, contact your Microsoft account representative. | Ready to buy? Contact us. | Bigger ideas, fewer words |
| Invalid ID | You need an ID that looks like this: someone@example.com | Write like you speak |
| what you are interested in, what is on your calendar | what you're interested in, what's on your calendar | Use contractions |
| Android, iOS and Windows | Android, iOS, and Windows | Oxford comma |
| Find a Microsoft Partner | Find a Microsoft partner | Sentence-style capitalization |
| You can access Office apps across your devices, and you get online file storage and sharing. | Store files online, access them from all your devices, and share them with coworkers. | Revise weak writing |
| Use pipelines — logical groups of activities — to consolidate activities. | Use pipelines—logical groups of activities—to consolidate activities. | No spaces around em dashes |

## Output format

When reviewing content, structure your response as:

```
## Style review

### Issues found

1. **[Rule name]** — "original text"
   - Problem: explanation
   - Suggested: rewritten text

2. ...

### Summary
- X issues found across Y categories
- Overall compliance: high/medium/low

### Rewritten version (if requested)
...
```
