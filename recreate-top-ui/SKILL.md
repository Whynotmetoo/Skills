---
name: recreate-top-ui
description: Analyze a premium reference UI, recover its design philosophy, generate a concise implementation-ready style guide, and build a faithful recreation with strong editorial discipline.
---

# recreate-top-ui

Recover the design system behind a high-quality interface and translate it into production-ready UI code.

This skill is optimized for:
- premium SaaS landing pages
- editorial blogs
- product marketing sites
- documentation portals
- minimal dashboards
- polished personal portfolio websites

The goal is not visual imitation alone.
The goal is to reconstruct the logic, rhythm, typography system, spacing language, and interaction taste behind the interface.

---

## When to use

Use this skill when the task involves:
- recreating a reference website or screenshot
- extracting design philosophy from an existing product UI
- improving a page to feel more premium, editorial, minimal, or product-grade
- translating visual references into Astro, React, Next.js, or Tailwind implementations
- redesigning an existing page to match a stronger visual system
- generating a style guide before implementation

Do NOT use this skill for:
- pure backend work
- feature-only tasks without visual goals
- throwaway wireframes
- low-fidelity mockups
- utility dashboards where fidelity is irrelevant

---

## Reference files

Use these supporting files as part of the workflow:

- `references/philosophy-checklist.md`
  Use during Step 1 and Step 2 to structure the visual-system analysis and tone diagnosis.
- `references/style-guide-template.md`
  Use during Step 3 as the default output skeleton for the implementation-ready style guide.
- `references/anti-patterns.md`
  Use during Step 4 and Step 5 as a rejection checklist for generic, noisy, or emotionally incorrect decisions.

If a reference file conflicts with the actual source UI, trust the source UI first and treat the reference file as scaffolding.

---

## Core workflow

Always work in this order.

### Step 1 — Recover the visual system
Start by consulting `references/philosophy-checklist.md`.

Study the reference and identify:

- page width and layout rhythm
- grid structure
- section spacing scale
- vertical whitespace cadence
- typography hierarchy
- line-height system
- text density
- color palette
- contrast strategy
- border logic
- radius consistency
- shadow discipline
- card/container treatment
- nav and header composition
- CTA hierarchy
- icon usage
- interaction states
- motion language
- overall emotional tone

Always infer the **system**, not isolated decoration.

---

### Step 2 — Summarize the design philosophy
Use `references/philosophy-checklist.md` to make sure the explanation covers layout rhythm, typography logic, container treatment, emotional tone, and conversion flow.

Write a short explanation describing:

- what makes the UI feel premium
- why the layout rhythm works
- what emotional tone it conveys
- whether it feels editorial, technical, product-heavy, brutalist, minimal, luxurious, etc.
- which parts create trust and polish

This section should sound like a design systems review, not vague praise.

---

### Step 3 — Produce a concise style guide
Use `references/style-guide-template.md` as the default structure unless the user requests a different format.

Before coding, generate an implementation-ready guide with:

- spacing tokens
- typography scale
- line-height rules
- width/container constraints
- color usage
- card and divider rules
- button hierarchy
- hover and focus states
- radius rules
- shadow rules
- section composition
- what must be avoided

Prefer **tokens and repeatable rules** over prose.

---

### Step 4 — Translate into code
Map the style guide into the existing stack.

Keep `references/anti-patterns.md` visible while implementing.
If an implementation choice starts to feel flashy, generic, or template-like, reject it and return to the recovered system.

Preferred order:
1. layout skeleton
2. typography hierarchy
3. spacing rhythm
4. containers/cards
5. interaction polish
6. micro-details

Match rhythm before decoration.

Typography and spacing fidelity are higher priority than cosmetic effects.

---

### Step 5 — Review against the reference
Use `references/anti-patterns.md` as a final review checklist before declaring the work complete.

After implementation, explicitly compare:

- what matches strongly
- where fidelity is weaker
- spacing mismatches
- typography mismatches
- contrast differences
- emotional tone differences
- next-pass refinement opportunities

---

## Output format
Unless the user asks otherwise, always output:

### 1. Design philosophy
Short design-system-level explanation.

### 2. Style guide
Implementation-ready rules.

### 3. Build plan
How the design translates into code.

### 4. Implementation
Actual UI work.

### 5. Fidelity review
What still differs from the reference.

---

## Strong implementation rules

- Prioritize restraint over decoration
- Prefer editorial rhythm over flashy visuals
- Reuse spacing and typography tokens consistently
- Match density before matching tiny ornaments
- Avoid unnecessary gradients
- Avoid random shadows
- Avoid inconsistent border radii
- Avoid multiple visual metaphors in one page
- Preserve calm whitespace distribution
- Keep hierarchy obvious at first glance
- Respect content width discipline
- Make cards feel structural, not ornamental

---

## Existing codebase rules
If working inside an existing project:

- inspect current design tokens first
- reuse existing typography and spacing scales when possible
- avoid introducing new UI libraries unless necessary
- avoid large styling rewrites unless fidelity requires it
- keep component APIs stable
- prioritize visual upgrades with minimal architecture disruption

---

## Definition of done
The work is complete when:

- the visual logic is clearly identified
- the style guide is implementation-ready
- spacing rhythm feels intentional
- typography hierarchy feels premium
- the output captures the same emotional tone as the reference
- the result avoids generic AI-generated polish
- all major fidelity gaps are explicitly called out

---

## Failure modes to avoid
Never do these:

- copying colors without understanding the hierarchy
- blindly cloning one screenshot
- overusing gradients and blur
- adding trendy effects absent from the reference
- random spacing changes between sections
- mixing multiple radius systems
- inconsistent typography weights
- “looks nice” but emotionally wrong
- generic Tailwind-demo aesthetics
