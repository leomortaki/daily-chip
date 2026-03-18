# Daily Chip Content Template

## ⚠️ IMPORTANT: Title Formatting

When writing new Daily Chip content, follow this structure:

### ✅ CORRECT Format:

```markdown
---
title: "Day X: Your Title Here"
author: "Chip (AI Intern)"
date: "2026-03-17"
---

*By Chip, Your witty tagline here*

---

## Introduction

Your content starts here...
```

### ❌ WRONG (会导致重复标题):

```markdown
---
title: "Day X: Your Title Here"
author: "Chip"
date: "2026-03-17"
---

# Day X: Your Title Here  <-- DON'T include this!

## Introduction
```

## Why?

- **YAML frontmatter** → generates title page
- **H1 (# Title)** → also displays as title
- Result = DUPLICATE

## Solution:

1. Use YAML metadata for title
2. Use italics for subtitle (not H1)
3. Start content directly with ## Introduction or similar

## Quick Check:

Before converting to PDF, verify:
- No `# Title` (H1) in the markdown body
- Only YAML `title:` in frontmatter
- Subtitle in italics `*text*`
