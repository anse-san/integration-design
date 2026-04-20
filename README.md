# menta — Integration Design Map

Single-file React app that serves as menta's Integration Design Map knowledge base.

**Live site:** https://anse-san.github.io/integration-design/

## Contents

- `index.html` — the full app. All KB content (decisions, pre-conditions, rules, integration tests, secondary market tests, guidelines) lives in a JSON blob inside the `<script id="kb-data">` tag.

## Editing the KB

Edits are made through the `kb-modifier` skill in Claude Code. The skill reads `index.html`, modifies the JSON, and commits + pushes the change to this repo — which auto-deploys to GitHub Pages.

## Local preview

```sh
open index.html
```
