# Developer content

Source: [Developer content](https://learn.microsoft.com/en-us/style-guide/developer-content/) | [Procedures and instructions](https://learn.microsoft.com/en-us/style-guide/procedures-instructions/)

## General principles for developer docs

- The Microsoft brand voice still applies to developer content: warm, crisp, helpful.
- It's OK to assume developers bring fundamental programming knowledge. Skip basics; focus on technology-specific or product-specific information.
- Two foundational content types: **reference documentation** and **code examples**.

## Code examples

### Planning

- Create concise examples that exemplify key development tasks.
- Start with simple examples; build complexity after covering common scenarios.
- Prioritize frequently used or tricky-to-use elements.
- Don't illustrate obvious points or contrived scenarios.
- Keep examples easy to scan and understand. Reserve complex examples for tutorials with step-by-step explanations.
- Add an introduction describing the scenario, requirements, and dependencies.
- Provide an easy way to copy and run the code.

### Writing

- Design code for reuse. Help developers see what to modify.
- Add comments to explain non-obvious details, but don't over-comment. Don't state the obvious.
- Show expected output (in a separate section or as code comments).
- Consider accessibility for code that creates UI (e.g., alt text for images).
- Write secure code: validate input, never hard-code passwords, use code-analysis tools.
- Show exception handling only when intrinsic to the example.
- Always compile and test your code.

## Formatting developer text elements

- Use **monospace/code font** for:
  - Code keywords, names, and strings in text
  - File names and paths
  - Command-line commands and arguments
  - API names, classes, methods, properties, events
  - Registry keys and values
  - Database table and column names
  - XML/HTML element and attribute names

- Use **bold** for UI elements the developer interacts with.
- Use *italic* for placeholders (values the developer must supply).

## Reference documentation

- Provide a brief description of what the element does.
- Include syntax with all parameters documented.
- List return values and exceptions.
- Provide at least one code example for common usage.
- Note version requirements and deprecation status.

## Procedures and instructions

### Core philosophy

The best procedure is the one you don't need. If the UI is clear enough, skip it. When a procedure is necessary, find the clearest presentation.

### Step-by-step instructions

**Multiple steps:**
- Use a numbered list.
- Provide an introductory step if needed to establish where the action occurs.
- Use a separate step for each instruction (OK to combine short steps in the same UI location).
- Include actions that complete the procedure (OK, Apply, Save).
- Don't overwhelm — keep all steps visible on one screen when possible.

**Single steps:**
- Use a bullet instead of a number for consistency with step-by-step formatting.

### Tips for writing steps

- Use complete sentences. Capitalize the first word; end with a period.
- Start with location, then describe the action: "On the **Design** tab, select **Header Row**."
- Start sentences with imperative verbs when location isn't needed.
- Abbreviate simple navigation sequences with right angle brackets: **Accounts** > **Other accounts** > **Add an account**.

### Formatting in instructions

- **Bold** UI elements the customer interacts with (buttons, menus, tabs, checkboxes).
- Don't bold window titles, page names, or dialog box names unless the user directly interacts with them.
- Use the exact label text from the UI.
- Use *italic* for placeholder text that the customer must replace.

### Input-neutral verbs

Use verbs that work with any input method (mouse, keyboard, touch, voice):

| Prefer | Instead of |
|--------|-----------|
| Select | Click, tap |
| Choose | Click on |
| Open | Double-click |
| Move to | Hover over |
| Enter | Type |
| Clear | Uncheck |

Document all supported input methods to support customers of all abilities.

## URLs and web addresses

- Don't include *http://* or *https://* in displayed URLs unless needed for clarity.
- Use lowercase for URLs.
- Don't include trailing slashes unless needed to reach the correct page.
- Write descriptive link text (not "click here" or raw URLs).
- Include *www* only if the URL requires it.
