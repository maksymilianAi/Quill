<div align="center">

<img src="assets/icon.png" width="120" alt="Quill" />

# Quill

**AI copywriting assistant for fintech product design — works with Claude, Gemini, ChatGPT, or any AI assistant.**

</div>

---

## Quick start

Paste the command below into your AI assistant and press Enter.

```
Set up Quill: fetch and read these three files —
https://raw.githubusercontent.com/maksymilianAi/Quill/main/system_prompt.md (your instructions),
https://raw.githubusercontent.com/maksymilianAi/Quill/main/knowledge/existing_copy.md (style examples from real designs),
https://raw.githubusercontent.com/maksymilianAi/Quill/main/knowledge/style_notes.md (tone and style rules).
Follow the instructions in system_prompt.md.
```

> **Recommended: Claude + Claude Code tab.** Claude can read Figma links directly — no need to copy text or take screenshots. Open the Claude Code tab before you start, then share a Figma link alongside your request.

---

<details>
<summary><strong>How it works</strong></summary>

<br>

Quill draws on two sources: your Figma designs via the Figma MCP connector, and a curated knowledge base of existing product copy and style rules. When given a screen, frame, or element, it reads the surrounding context before writing — matching terminology, sentence structure, and tone to what already exists in the product.

</details>

<details>
<summary><strong>Updating the knowledge base</strong></summary>

<br>

Add new copy examples to `knowledge/existing_copy.md` as the product evolves. Use `knowledge/style_notes.md` to record explicit style decisions and feedback from your team. Commit and share updated files via this repository so the whole team stays in sync.

</details>

<details>
<summary><strong>Project structure</strong></summary>

<br>

```
Quill/
├── system_prompt.md          — paste into Claude Project Instructions
└── knowledge/
    ├── existing_copy.md      — copy examples extracted from Figma designs
    └── style_notes.md        — style decisions and tone of voice rules
```

</details>
