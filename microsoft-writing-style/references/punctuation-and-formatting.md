# Punctuation and formatting

Source: [Punctuation](https://learn.microsoft.com/en-us/style-guide/punctuation/) | [Capitalization](https://learn.microsoft.com/en-us/style-guide/capitalization) | [Scannable content](https://learn.microsoft.com/en-us/style-guide/scannable-content/)

## Capitalization rules

### Sentence-style capitalization (default)

- Capitalize only the first word and proper nouns.
- Apply to: headings, titles, UI labels, button text, checkbox labels, column headers, list items.
- Never use Title Case for headings. Never use ALL CAPS for emphasis.

### When to use title-style capitalization

Only for:
- Product and service names (Azure DevOps, Microsoft 365)
- Book/song titles in citations
- Titles of people (Vice President of Engineering)
- Blog post titles that reference article names in citations

### Title-style rules (when required)

- Capitalize first and last words always.
- Don't capitalize *a, an, the* unless first/last word.
- Don't capitalize prepositions of four or fewer letters (*on, to, in, up, of, for*) unless first/last.
- Don't capitalize *and, but, or, nor, yet, so* unless first/last.
- Capitalize all nouns, verbs (including *is*), adverbs, adjectives, pronouns.
- Capitalize the word after a hyphen if it would be capitalized alone.

## Punctuation rules

### Oxford (serial) comma

Always include the comma before the conjunction in a list of three or more items.

- Correct: "Android, iOS, and Windows"
- Incorrect: "Android, iOS and Windows"

### Periods

- Every sentence in body copy ends with a period.
- **Skip periods** on: headings, subheadings, UI titles, list items of three or fewer words.
- Use one space (not two) after a period.

### Em dashes

- No spaces around em dashes: *word—word*
- Use to set off parenthetical phrases or to elaborate.
- Don't use spaced en dashes (word – word) as a substitute.

### En dashes

- Use in ranges: *pages 5–10*, *Monday–Friday*, *2020–2024*.
- No spaces around en dashes in ranges.

### Colons

- Capitalize the first word after a colon only if it begins a complete sentence.
- Use a colon to introduce a list (when the introductory text is a complete clause).

### Semicolons

- Avoid when possible. Prefer two shorter sentences.
- OK between closely related independent clauses or items in a complex list.

### Exclamation points

- Use sparingly — at most one per topic or page.
- Never use in error messages or warnings.
- Never use more than one in a row (!!!).

### Question marks

- Use sparingly. Prefer declarative or imperative sentences.
- OK in headings that address a genuine user question.

### Quotation marks

- Use only for direct quotations, not for emphasis.
- Periods and commas go inside quotation marks (US style).
- Colons and semicolons go outside.

## Formatting for scannability

### Headings

- Use sentence-style capitalization.
- Keep headings short and descriptive.
- Front-load keywords for scanning.
- Don't end headings with periods.
- Use heading hierarchy consistently (don't skip levels).

### Lists

- Use bulleted lists for items without sequence.
- Use numbered lists for sequential steps.
- Start each item with the same part of speech (parallel structure).
- Skip periods on items of three or fewer words.
- Use periods on items that are complete sentences.
- Don't mix sentence fragments and complete sentences in the same list.

### Paragraphs

- Keep paragraphs to three to seven lines.
- Single-line paragraphs are fine occasionally.
- Lead with the most important information.
- One idea per paragraph.

### Tables

- Use tables for structured data, comparisons, or reference information.
- Keep table cells concise.
- Use sentence-style capitalization in headers.

### Bold and italic

- Use **bold** for UI elements the user interacts with (button names, menu items).
- Use *italic* sparingly for emphasis or introducing new terms.
- Don't use ALL CAPS, underline, or color for emphasis.

## Text formatting — common elements

Source: [Formatting common text elements](https://learn.microsoft.com/en-us/style-guide/text-formatting/formatting-common-text-elements)

| Element | Convention | Example |
|---------|-----------|---------|
| Database names | Bold | **Contoso** database |
| Emphasis | Italic (sparingly) | Microsoft will *never* call you to charge for fixes. |
| Error messages | Sentence-style cap; quotation marks when referenced in text | "Check scanner status and try again" |
| File attributes | All lowercase | hidden, system, read-only |
| File name extensions | All lowercase | .mdb, .doc, .xlsx |
| File names | Title-style capitalization | My Taxes for 2016 |
| Folder/directory names | Sentence-style cap (internal caps OK) | MyFiles\Accounting\Payroll |
| Math constants/variables | Italic | *a² + b² = c²* |
| New terms (first mention) | Italic, then define immediately | Microsoft Exchange consists of both *server* and *client* components. |
| Ports | All uppercase | LPT1 |
| Products/services/trademarks | Title-style cap (check trademark list) | Microsoft Arc Touch Mouse |
| UI text/strings | Sentence-style capitalization | Find on page |
| URLs | All lowercase | www.microsoft.com |

## Formatting titles

- Use **sentence-style capitalization** for titles by default.
- Use **bold** for titles of standalone works (books, reports, white papers) in running text.
- Don't use quotation marks for emphasis on titles.
- Italicize titles of published works when referencing in formal citations.

## Alternative text (alt text)

Source: [Alternative text](https://learn.microsoft.com/en-us/style-guide/accessibility/alternative-text)

Alt text provides a textual replacement for images for users who can't view them.

### General rules

- Add alt text to all images that convey important meaning.
- Purely decorative images don't need alt text (use `alt=""` in HTML).
- Begin with a capital letter. End with a period.
- Don't start with "Image" or "Picture" — screen readers already announce these.
- Start by specifying what the image is (screenshot, diagram, chart, photograph).
- Don't use the file name as alt text.
- Include embedded text if surrounding content doesn't already.
- Limit to 150 characters. For complex images, provide a detailed description in surrounding text.
- Don't repeat surrounding text or captions.

### Buttons and links with images

- If a button/link has an image but no text: alt text describes what it *does*, not what it shows.
- Don't start with "Button" or "Link" — screen readers already announce these.
- If a button/link has both image and text: the image is decorative (no alt text needed).

### Examples

| Scenario | Good alt text | Bad alt text |
|----------|--------------|-------------|
| Screenshot illustrating preceding steps | "Screenshot of the tab for creating an account." | Describing every detail already covered in steps |
| Gear icon button (no label) | "Open user settings." | "Image of two interlocking gears." |
| Search magnifying glass button | "Search this site." | "Magnifying glass button for searching." |
