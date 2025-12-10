# NATH Syntax  
*“A minimal markup system for human-readable notes and machine-readable meaning.”*

![License: MIT](https://img.shields.io/badge/License-MIT-pink.svg)
![Language: NATH](https://img.shields.io/badge/language-NATH-8A6FE8.svg)
![VS Code](https://img.shields.io/badge/editor-VS%20Code-23A9F2.svg)
![Status: Stable](https://img.shields.io/badge/status-syntax_only-lightgrey.svg)
![Made with Love](https://img.shields.io/badge/made_with-%F0%9F%8C%88-ffb3ff.svg)

# NATH Syntax  
_Neuro-Aligned Typological Hierarchy_

NATH is a lightweight cognitive markup language designed for expressive journaling, structured emotional description, and machine-friendly reasoning.

This repository contains the **syntax-only VS Code extension** for NATH:

- syntax highlighting  
- rune definitions  
- snippets  
- themes (light + dark)  
- example files  

NATH uses single-character “runes” to categorize lines, creating a format that is easy to write and exceptionally efficient for humans, search engines, and AI models.

---

# ✨ Why NATH?

NATH emphasizes **clarity, accessibility, and computational simplicity**.  
It is designed for scenarios where emotional data, introspection notes, or structured reflections must be:

- quick to write  
- easy to revisit  
- trivial to parse  
- efficient for embeddings  
- friendly for LLM-based reasoning agents  

### Minimal overhead

No brackets, commas, nesting, or indentation rules.  
Just **rune + content** on each line.

### Predictable structure

Every rune maps to a semantic field, which makes NATH ideal for:

- dataset creation  
- embeddings  
- low-token LLM contexts  
- retrieval-augmented generation  
- emotional reasoning tools  

### Dual-layer architecture

NATH separates entries into:

1. **Structural meaning (runes, headings, tags)**  
2. **Free-form narrative (`[text]`)**

This duality allows tools to perform structured analysis while preserving natural expression.

---

# 🧭 Dual-Layer Indexing: Headings & Tags

NATH provides two built-in indexing mechanisms that dramatically improve searchability and machine parsing.

### 1. Section Headings (`#`)

Each heading creates a new entry block and is ideal for:

- outlining  
- document navigation  
- search segmentation  
- timeline reasoning  

Example:

    # overwhelmed @evening

### 2. Tags (`@`)

Tags attach categorical metadata to a section.

- easy to grep  
- efficient for embeddings  
- ideal for clustering and filters  
- useful for AI-assisted analysis  

Example:

    # conflict @relationship @fear

Tags may be chained:

    # morning_rush @routine @adhd @stress

### Why this matters for AI

Headings define **context boundaries**, and tags provide **quick semantic anchors**.  
Combined, they enable powerful retrieval pipelines without requiring heavy parsing or additional metadata layers.

LLMs benefit from this because they:

- receive clean, well-segmented chunks  
- avoid accidental cross-contamination between topics  
- can “jump to” relevant sections via tags  
- work with low-token structural cues  

---

# 📘 What Is NATH?

NATH (Neuro-Aligned Typological Hierarchy) is a notation system for capturing:

- internal states  
- emotions  
- needs and impulses  
- constraints  
- outcomes  
- contextual narratives  

A typical NATH record looks like this:

    # overwhelmed @evening

    ^identity
    /machine_key

    !fear
    :inadequate
    .busy
    >avoid
    ?quiet
    |no_quitting
    =I_am_trying
    +stability
    _small_step
    %reset
    &friend
    $energy_low
    *environment
    'today
    "they_checked_in
    ~not_sure
    >>felt_slightly_better

    [narrative: short context description]

Each line stands alone, making NATH entries simple to index, search, embed, or transform.

---

# 🔠 Rune Reference

| Rune | Meaning | Example |
|------|---------|---------|
| `^` | Identity / self-reference | `^me` |
| `/` | Machine key / unique identifier | `/2025-01-04_m1` |
| `!` | Affect (broad category) | `!fear` |
| `:` | Emotion (specific named feeling) | `:inadequate` |
| `.` | Tone (surface-level signal) | `.busy` |
| `-` | Aversion, fear, or avoidance marker | `-conflict` |
| `>` | Impulse / action tendency | `>avoid` |
| `?` | Need / unmet requirement | `?quiet` |
| `|` | Boundary | `|no_quitting` |
| `=` | Truth / grounding statement | `=I_am_trying` |
| `+` | Value / principle | `+stability` |
| `_` | Strategy | `_small_step` |
| `%` | Revision / change marker | `%reset` |
| `&` | Living entity | `&friend` |
| `$` | Limiter (time/energy/money constraints) | `$energy_low` |
| `*` | System agent (external forces) | `*algorithm` |
| `'` | Time marker | `'today` |
| `"` | Evidence / observation | `"they_checked_in` |
| `~` | Uncertainty | `~not_sure` |
| `>>` | Outcome | `>>felt_slightly_better` |
| `@` | Tags | `@evening` |
| `#` | Section heading | `# overwhelmed` |
| `[text]` | Narrative | `[narrative: ...]` |

---

# 🚀 Quick Start

### 1. Install the extension locally

    npm install
    npm run compile

Launch the extension using:

- **F5** in VS Code

### 2. Create a `.nath` file

    example.nath

### 3. Use the snippet

Type:

    nrec

Then press **Tab** to insert a full NATH record template.

---

# 🎨 Themes

This repository includes:

- **Pastel Cognition Light** — soft, gentle palette  
- **Pastel Cognition Dark** — aurora-inspired dark mode  

Both themes colorize runes consistently to support readability and structural clarity.

---

# 📂 Project Structure

    nath-syntax/
    ├── README.md
    ├── CONTRIBUTING.md
    ├── package.json
    ├── language/
    ├── themes/
    ├── .github/
    │   ├── ISSUE_TEMPLATE/
    │   └── pull_request_template.md
    └── examples/

---

# 🪪 License

This project is licensed under the **MIT License**.

---

# 💗 Acknowledgments

NATH is crafted for clarity, expressiveness, and cognitive readability while remaining lightweight enough for modern AI systems and everyday journaling.
