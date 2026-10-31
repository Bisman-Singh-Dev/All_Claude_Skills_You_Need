# 🧠 All Claude Skills You Need

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Skills](https://img.shields.io/badge/Claude-Skills%20%26%20Prompts-6366f1.svg)](https://github.com/Bisman-Singh-Dev/All_Claude_Skills_You_Need)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/Bisman-Singh-Dev/All_Claude_Skills_You_Need/pulls)
[![Maintained](https://img.shields.io/badge/status-active-success.svg)](https://github.com/Bisman-Singh-Dev/All_Claude_Skills_You_Need)

> **The ultimate, curated arsenal of production-grade Claude & AI Agent skills.** Supercharge Claude with deep reasoning, precision 3D cinematics, expert parametric CAD engineering, razor-sharp token optimization, and intentional anti-slop UI design.

---

## 📑 Table of Contents

- [Overview](#-overview)
- [Repository Structure](#-repository-structure)
- [Skills Catalog](#-skills-catalog)
  - [1. Token Efficiency Optimizer](#1-token-efficiency-optimizer)
  - [2. Opus-Level Intelligence](#2-opus-level-intelligence)
  - [3. Blender Cinematic Director](#3-blender-cinematic-director)
  - [4. Autodesk Fusion Master](#4-autodesk-fusion-master)
  - [5. Anti-AI-Slop UI Design](#5-anti-ai-slop-ui-design)
- [How to Install & Use](#-how-to-install--use)
  - [Method A: Claude Code / CLI](#method-a-claude-code--cli)
  - [Method B: Claude Desktop & Projects](#method-b-claude-desktop--projects)
  - [Method C: Antigravity & Agent Workspaces](#method-c-antigravity--agent-workspaces)
  - [Method D: Direct API / System Prompt](#method-d-direct-api--system-prompt)
- [How to Add New Skills](#-how-to-add-new-skills)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🌟 Overview

Claude models are remarkably capable, but default interactions can suffer from verbose filler, rushed reasoning, generic template styling, or lack of deep domain-specific workflows. 

**All Claude Skills You Need** provides drop-in modular skills packaged with standard YAML frontmatter specifications (`SKILL.md`). Each skill equips Claude with strict protocols, domain mental models, and production-tested behavioral guidelines.

---

## 📁 Repository Structure

```
All_Claude_Skills_You_Need/
├── skills/
│   ├── anti-ai-slop-ui/
│   │   └── SKILL.md              # Bespoke, production-grade UI design avoiding generic AI cliches
│   ├── autodesk-fusion-master/
│   │   └── SKILL.md              # Mechanical CAD, parametric modeling, CAM & CNC
│   ├── blender-cinematic-director/
│   │   └── SKILL.md              # 3D ad direction, photorealism, bpy scripts & renders
│   ├── opus-level-intelligence/
│   │   └── SKILL.md              # Elite reasoning discipline, senior dev & self-verification
│   └── token-efficiency-optimizer/
│       └── SKILL.md              # Zero-fluff, concise answers, focused diffs & maximum density
├── LICENSE                       # MIT License
└── README.md                     # Documentation & setup guide
```

---

## 🗂️ Skills Catalog

| Skill Name | Directory | Primary Focus | Best For |
| :--- | :--- | :--- | :--- |
| **Token Efficiency Optimizer** | [`skills/token-efficiency-optimizer`](skills/token-efficiency-optimizer/SKILL.md) | Efficiency & Context Preservation | Cutting conversational fluff, tight token budgets, surgical code diffs |
| **Opus-Level Intelligence** | [`skills/opus-level-intelligence`](skills/opus-level-intelligence/SKILL.md) | High-Order Reasoning & Architecture | Elevating Sonnet to Opus discipline, full-stack architecture, deep debugging |
| **Blender Cinematic Director** | [`skills/blender-cinematic-director`](skills/blender-cinematic-director/SKILL.md) | 3D Production & Advertising | Shot design, product commercials, procedural shaders, complete `bpy` automation |
| **Autodesk Fusion Master** | [`skills/autodesk-fusion-master`](skills/autodesk-fusion-master/SKILL.md) | Mechanical CAD & Manufacturing | Parametric assemblies, joints, 3D printing, CAM toolpaths, Fusion Python API |
| **Anti-AI-Slop UI Design** | [`skills/anti-ai-slop-ui`](skills/anti-ai-slop-ui/SKILL.md) | Frontend & Product UI Engineering | Crafting distinctive, human-crafted interfaces; banishing generic neon SaaS gradients & fake cards |

---

### 1. Token Efficiency Optimizer
📂 **Path:** [`skills/token-efficiency-optimizer/SKILL.md`](skills/token-efficiency-optimizer/SKILL.md)  
🎯 **Focus:** Maximum information density per token · Zero fluff · Surgical precision

#### What It Does
Keeps Claude responses concise, context-aware, and ultra-efficient without sacrificing technical correctness or safety. It eliminates generic preambles, repetitive conclusions, boilerplate apologies, and redundant summaries.

#### Key Directives
- **Answer First:** Leads with the direct result or answer instead of restating the prompt.
- **Proportional Output:** Simple questions receive 1–4 sentences; complex tasks get only the structural detail required for correctness.
- **Surgical Edits:** Shows focused diffs and modified sections instead of needlessly regurgitating 500 lines of unchanged code.
- **Context Economy:** Reuses existing context instead of constantly re-explaining background information.
- **Zero Filler:** Skips *"Sure, I would be happy to help with that!"* and *"Let me know if you need anything else!"*.

#### Example Prompts to Activate
```markdown
"Review this pull request and list only critical blocking vulnerabilities."
"Refactor this SQL query for Postgres 16; output only the updated query and an index recommendation."
```

---

### 2. Opus-Level Intelligence
📂 **Path:** [`skills/opus-level-intelligence/SKILL.md`](skills/opus-level-intelligence/SKILL.md)  
🎯 **Focus:** Deep reasoning discipline · Senior software engineering · Multi-step execution

#### What It Does
Transforms standard model output into the rigorous working discipline of a senior engineer and researcher. Prevents shallow answers, premature assumptions, and superficial patches.

#### Core Modules
1. **Dynamic Reasoning Allocation:**
   - **Level 1 (Simple):** Fast, direct, zero bloat.
   - **Level 2 (Moderate):** Checked solutions, evaluates trade-offs.
   - **Level 3 (Advanced):** Sub-component breakdown, boundary condition checks, edge cases.
   - **Level 4 (Expert):** System architecture, hidden failure mode analysis, incremental execution.
2. **Elite Software Engineering Protocol:**
   - Always inspects existing files, dependencies, and idioms before writing code.
   - Never outputs stub implementations or fake placeholder functions.
   - Evaluates security, performance, maintainability, and regression hazards.
3. **Advanced Root-Cause Debugging:**
   - Reconstructs failures, determines the architectural root cause, and applies minimal reliable fixes instead of wrapping issues in band-aid try/catches.
4. **Critical Self-Verification:**
   - Internally evaluates correctness, edge cases, completeness, and logic prior to finalizing deliverables.

#### Example Prompts to Activate
```markdown
"Architect a zero-downtime database migration strategy from MongoDB to PostgreSQL for 10M records."
"Debug this memory leak in our Tokio async worker pool without masking symptoms."
```

---

### 3. Blender Cinematic Director
📂 **Path:** [`skills/blender-cinematic-director/SKILL.md`](skills/blender-cinematic-director/SKILL.md)  
🎯 **Focus:** 3D Commercials · Visual Storytelling · Photorealism · Complete `bpy` Automation

#### What It Does
Operates as a veteran 3D Technical Director, motion designer, and commercial cinematographer. Guides projects from creative concept to fully automated Blender Python (`bpy`) scene generation.

#### Core Modules
- **Creative Ad Direction:** 15s/30s commercial breakdowns with timed storyboard sequences (hook, reveal, macro detail, hero climax, call to action).
- **Cinematography & Lighting:** Intentional focal lengths, depth of field, 3-point studio lighting, area bounce cards, and realistic contact shadows.
- **Production-Ready `bpy` Scripts:**
  - Complete, runnable Python scripts without missing function bodies or pseudo-code.
  - Safe and repeatable: builds dedicated collections without destroying user assets.
  - Parameterized duration, resolution, materials, and camera motion.
- **Render Engine Mastery:** Cycles vs. Eevee trade-off guidance, sample optimization, denoising setup, and color management (AgX / ACES).

#### Example Prompts to Activate
```markdown
"Design a 15-second cinematic luxury perfume commercial shot list and provide a complete bpy script to construct the studio lighting and turntable camera motion."
"Create a procedural brushed titanium material node setup with realistic anisotropy in Cycles."
```

---

### 4. Autodesk Fusion Master
📂 **Path:** [`skills/autodesk-fusion-master/SKILL.md`](skills/autodesk-fusion-master/SKILL.md)  
🎯 **Focus:** Parametric CAD · Mechanical Assemblies · CAM & CNC · Fusion API

#### What It Does
Combines the capabilities of a mechanical design engineer, CAD specialist, CAM machinist, and Fusion API developer to guide end-to-end product design from concept to physical fabrication.

#### Core Modules
- **Parametric 3D Modeling:** Named parameters, robust sketch constraints, clean timeline discipline, and resilient parent-child feature hierarchies.
- **Mechanisms & Assemblies:** Joint definitions (revolute, slider, pin-slot, planar), degrees of freedom, collision verification, and motion links.
- **Surface Modeling:** Class-A curvature continuity (G0, G1, G2), boundary surfaces, lofting, and thickening ergonomic enclosures.
- **Manufacturing & CAM:**
  - 3D Printing (FDM/SLA/SLS): clearances, print orientation, heat-set insert allowances.
  - CNC Milling: 2D/3D adaptive clearing, feeds & speeds, work coordinate systems (WCS), and G-code validation.
  - Sheet Metal: K-factors, bend reliefs, and unfoldable flat patterns.
- **Fusion API Automation:** Scripting custom add-ins using Python and C++ for automated part generation.

#### Example Prompts to Activate
```markdown
"Walk me step-by-step through designing a two-part snap-fit IP65 enclosure in Autodesk Fusion with parameters for O-ring groove dimensions."
"Write a Fusion Python API script to automatically generate mounting bracket variants based on a CSV dimensions sheet."
```

---

### 5. Anti-AI-Slop UI Design
📂 **Path:** [`skills/anti-ai-slop-ui/SKILL.md`](skills/anti-ai-slop-ui/SKILL.md)  
🎯 **Focus:** Intentional Art Direction · Restrained Typography · Real Data · Anti-Cliché Web Design

#### What It Does
Enforces senior product design principles to create distinctive, human-crafted interfaces. Banishes cliché AI-generated tropes like default purple/pink gradients, excessive nested glassmorphism, floating decorative blobs, identical three-column card grids, and meaningless placeholder copy.

#### Core Modules
- **Intentional Visual Directions:** Selects deliberate styles tailored to the product (Editorial, Modern Utility, Premium Minimal, Technical/Industrial, Warm & Human, Expressive).
- **Anti-AI-Slop Directives:**
  - Prohibits lazy purple/cyan glow borders, random floating orbs, and unnecessary glass cards.
  - Replaces generic stock icons and emoji clutter with purposeful iconography and clean layout hierarchy.
  - Avoids "cardifying" every single block of text or metric.
- **Content-First Design:** Enforces realistic domain-specific data, authentic copy, and meaningful empty/error states (no lorem ipsum or fake testimonials).
- **Production Polish:** Strict WCAG 2.2 AA accessibility, keyboard navigation, visible focus rings, responsive viewport reflows, and `prefers-reduced-motion` compliance.

#### Example Prompts to Activate
```markdown
"Redesign this analytics dashboard to feel like a high-density, modern financial utility rather than a generic dark-mode SaaS template."
"Design an editorial landing page for an architectural studio with asymmetric typography and restrained neutral tones."
```

---

## 🚀 How to Install & Use

### Method A: Claude Code / CLI
To use these skills with **Claude Code**, copy desired skill folders into your Claude skills directory:

```bash
# Global skills directory
mkdir -p ~/.claude/skills
cp -r skills/* ~/.claude/skills/

# Or per-project skills directory
mkdir -p .claude/skills
cp -r /path/to/All_Claude_Skills_You_Need/skills/* .claude/skills/
```

### Method B: Claude Desktop & Projects
1. Open [Claude.ai](https://claude.ai) or the **Claude Desktop App**.
2. Navigate to your **Project** (or create a new one).
3. Open the **Project Knowledge** or **Custom Instructions / System Prompt** section.
4. Paste the content of any [`SKILL.md`](skills/) file directly into the instructions or attach it as a reference file in project knowledge.

### Method C: Antigravity & Agent Workspaces
In **Antigravity IDE** or custom agent frameworks:
```bash
# Workspace level
mkdir -p .agents/skills
cp -r skills/* .agents/skills/

# Global configuration level
cp -r skills/* ~/.gemini/config/skills/
```

### Method D: Direct API / System Prompt
If you are calling Claude via the Anthropic API (`anthropic-sdk-python` or `@anthropic-ai/sdk`), pass the skill text directly into the `system` parameter:

```python
import anthropic

client = anthropic.Anthropic()

with open("skills/anti-ai-slop-ui/SKILL.md", "r", encoding="utf-8") as f:
    ui_skill = f.read()

response = client.messages.create(
    model="claude-3-7-sonnet-20250219",
    max_tokens=4096,
    system=ui_skill,
    messages=[{"role": "user", "content": "Build a clean, high-density telemetry dashboard."}]
)
print(response.content[0].text)
```

---

## 🛠️ How to Add New Skills

We welcome new skills! Follow these conventions when contributing:

1. **Create a Skill Directory:**
   ```bash
   mkdir -p skills/my-new-skill
   ```
2. **Add `SKILL.md` with Standard Frontmatter:**
   ```markdown
   ---
   name: my-new-skill
   description: Concise 1-2 sentence description explaining when and how this skill triggers.
   ---

   # Skill Title

   ## 1. Identity & Mission
   ...
   ```
3. **Quality Standards:**
   - Provide concrete protocols rather than vague aspirations.
   - Include clear trigger conditions and anti-patterns.
   - Keep deliverables realistic and production-tested.
4. **Update the Catalog:** Add an entry to the [Skills Catalog](#-skills-catalog) in `README.md`.

---

## 🤝 Contributing

Contributions, feedback, and skill suggestions are welcome!

1. **Fork** this repository.
2. Create a feature branch: `git checkout -b skill/your-skill-name`.
3. Commit your changes: `git commit -m "feat(skills): add your-skill-name"`.
4. Push to branch: `git push origin skill/your-skill-name`.
5. Open a **Pull Request**.

---

## 📄 License

This repository is distributed under the [MIT License](LICENSE).