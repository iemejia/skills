# Accessibility and AI writing

Source: [Accessibility](https://learn.microsoft.com/en-us/style-guide/accessibility/accessibility-guidelines-requirements) | [Chatbots and virtual agents](https://learn.microsoft.com/en-us/style-guide/chatbots-virtual-agents/)

## Writing for all abilities

Microsoft style — clean, simple design and crisp, clear content — is inherently more accessible. Pay special attention to these guidelines.

### Put the person first

- Use people-first language by default: refer to the person, then the disability.
- Consult approved accessibility terminology for specific terms.
- Use identity-first language only when you know the audience prefers it.

### Write brief, meaningful, and focused text

- Be especially clear and concise in instructions for setup, basic features, input methods, and accessibility features.
- Lead with what matters most.
- Keep paragraphs short; aim for one verb per sentence.
- Read text aloud — imagine it spoken by a screen reader.
- Use parallel writing structures for similar things.
- Spell out words like *and*, *plus*, and *about* — screen readers can misread special characters (+, ~).
- Write brief but meaningful link text that makes sense without surrounding context.

### Use content structure to communicate

- Use heading levels (not text formatting) to communicate hierarchy.
- Don't rely solely on directional terms (*left, right, above, below*) for location.
- Instead use specific language: "the first item in the following list" or "on the toolbar."
- Provide brief descriptions of tables before them in the text.
- Use concise, specific column headings.

### Visual accessibility

- Distinguish link text with redundant cues (color + underline).
- Don't force line breaks within sentences/paragraphs.
- Add alt text to all meaningful images (decorative images don't need it).
- Don't rely on color alone to convey information — use patterns or labels too.

### Document alternate input methods

- Document all supported input modes: mouse, keyboard, voice, game controller, gestures, touch.
- Use input-neutral verbs (*select* not *click*; *choose* not *tap*).
- Provide keyboard shortcuts alongside mouse instructions.

### Accessibility terminology

| Use this | Not this |
|----------|----------|
| person with a disability | disabled person, handicapped |
| person who is blind | blind person (unless audience prefers identity-first) |
| person who is deaf or hard of hearing | hearing-impaired |
| person with low vision | sight-impaired |
| person who uses a wheelchair | wheelchair-bound, confined to a wheelchair |
| accessible | handicap-accessible |

## Writing for chatbots and virtual agents

### When to use a bot

A virtual agent is suitable when it's easier to ask for what you want than navigate menus or search keywords. Not suitable for everything — know the limitations.

### Two types

- **Scripted**: responds only to pre-programmed questions.
- **AI-powered**: understands natural language, grows with interactions.

### Structural and technical considerations

- Define the bot's scope clearly — what it can and can't do.
- Provide graceful fallbacks when the bot doesn't understand.
- Make it easy to reach a human when needed.
- Design conversations to be short and goal-oriented.
- Plan for error handling and unexpected input.

### Writing for bots

- Give the bot a consistent personality aligned with brand voice (warm, crisp, helpful).
- Keep messages short — one to two sentences per response when possible.
- Use plain language; avoid jargon.
- Write natural, conversational prompts.
- Provide clear options when the user needs to make a choice.
- Confirm actions before executing irreversible operations.
- Be transparent: make it clear the user is interacting with a bot, not a person.
- Acknowledge mistakes: "I didn't understand that. Could you try rephrasing?"

### Care and feeding

- Test continuously with real users.
- Monitor conversations for failures and gaps.
- Update the bot's knowledge regularly.
- Review logs for opportunities to expand coverage.
- Maintain brand voice consistency as the bot evolves.

### AI-specific guidance

- Be transparent about AI capabilities and limitations.
- Don't anthropomorphize excessively — avoid claiming the bot "thinks" or "feels."
- Provide confidence indicators when appropriate ("I'm not sure, but...").
- Respect user data and privacy in all interactions.
- Design for graceful degradation when AI confidence is low.
