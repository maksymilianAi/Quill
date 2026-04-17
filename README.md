# 🪶 Quill

**Quill** is an AI copywriting assistant for fintech product design. It reads Figma context and suggests UX copy that matches your product's existing style and tone. Always provides 3 options with a recommended pick and brief rationale.

## What It Does

Quill is trained on real copy from your product designs and applies consistent UX writing principles — verb-first descriptions, precise domain terminology, and the tone your users already know. It works entirely within Claude Projects and requires no backend infrastructure.

## Setup

Download [Claude](https://claude.ai) desktop app and create a new Project named **Quill**. Paste the contents of `system_prompt.md` into the Project Instructions field. Upload both files from the `knowledge/` folder as Project knowledge. Connect your Figma account through Claude's connector settings if not already done.

## How It Works

Quill integrates two inputs: your Figma designs via the Figma MCP connector, and a curated knowledge base of existing product copy and style rules. When given a screen, frame, or element, it reads surrounding context before writing — matching terminology, sentence structure, and tone to what already exists in the product.

## Updating the Knowledge Base

Add new copy examples to `knowledge/existing_copy.md` as the product evolves. Use `knowledge/style_notes.md` to record explicit style decisions and feedback from your team. Commit and share updated files via this repository so the whole team stays in sync.
