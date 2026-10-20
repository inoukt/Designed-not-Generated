---
name: designed-not-generated
description: Design, build, redesign, and audit web or mobile interfaces with a distinctive, context-appropriate visual identity rather than generic AI-generated UI patterns. Use for landing pages, apps, dashboards, components, websites, and frontend styling or visual polish. Apply when creating UI from scratch or improving an existing interface.
---

# Designed, Not Generated

Create interfaces that feel art-directed for a specific product, audience, and task—not assembled from the most common patterns in a UI model's training data. Distinctiveness must never come at the expense of clarity, accessibility, or actual usefulness.

## Controls (use the user's preferences when provided)

| Control | Default | Range / alternatives |
| --- | --- | --- |
| Distinctiveness | 4/5 | 1 = conservative, 5 = experimental |
| Information density | Contextual | compact / balanced / spacious |
| Visual tone | Derived from product | restrained / editorial / expressive / technical / playful |
| Motion | Restrained | none / restrained / expressive |
| Existing brand fidelity | Strict | strict / flexible / new identity |

Don't ask the user to set these controls unless the choice has a major consequence. Infer a sensible baseline from the task. A banking operations console and an independent music publication should not be styled alike.

## Prime directive

**Do not confuse visual novelty with good design.** Avoid generic AI aesthetics because they do not express the product—not because particular colors, fonts, or components are inherently bad. Keep familiar conventions when they help users complete tasks. Vary what matters; simplify what does not.

## Workflow

### 1. Read the situation before choosing the visuals

Identify, from the brief and codebase if available:

- What is the product, who is using it, and what is their main task?
- What should feel trustworthy, memorable, fast, serious, welcoming, or premium?
- What is the actual content hierarchy? Which information or action should dominate?
- Is there an existing brand, design system, component library, or accessibility requirement to preserve?
- Is this a marketing page, editorial experience, dense product UI, commerce flow, or operational dashboard?

Do not invent logos, testimonials, conversion metrics, or product claims to fill a layout. Where actual content is unavailable, use plainly illustrative text and data.

### 2. Set a design thesis before writing UI code

Consider **at least three materially different directions** (not three colorways of the same template). Choose **one** coherent direction that fits the context. State it briefly in your working plan or final explanation:

- **Character:** a few precise adjectives (e.g., utilitarian, crafted, assured)
- **Typographic voice:** role of display, body, numeric, and interface typography
- **Composition:** grid, width, density, alignment, and which elements break the rhythm
- **Color/material:** purposeful palette, surfaces, borders, and emphasis
- **Signature detail:** one meaningful identifying motif tied to the product

A signature detail may be a typographic system, a distinctive navigation treatment, a content-led layout, or a domain-specific visualization. It does not need to be a decorative flourish.

**Push one thoughtful idea further than is comfortable.** Increase the specificity of one high-impact element (e.g. navigation built from a route diagram, a timetable that resembles platform signage, a catalog built around product photography). Keep the rest calm. Do not spread novelty equally across every element.

**Distinctiveness stress test:** Remove the logo and product name. Could a knowledgeable user still tell what type of business this is, and does it feel unlike a hundred unrelated startups? If not, change the concept before coding.

### 3. Build the content hierarchy first

- Arrange information according to user priorities rather than defaulting to a standard hero/cards/testimonials/FAQ template.
- Choose a composition appropriate to the content: editorial flow, compact workspace, comparison matrix, step-based journey, product gallery, etc.
- Use whitespace to create emphasis, not simply to make a page look expensive.
- Establish hierarchy with scale, weight, alignment, density, grouping, and contrast before adding decoration.
- Vary section treatments only when the content or narrative warrants it.
- Make important tasks and real information visible without forcing unnecessary scrolling.

### 4. Give the interface a specific visual language

**Typography:** Choose fonts deliberately for tone and readability. A default UI font is acceptable when it genuinely fits; don't use one automatically. Build contrast between title, body, labels, and data with a controlled type scale. Check long headings, numbers, and line length.

**Color:** Select colors based on meaning and identity, not trend palettes. A quiet neutral palette may be distinctive through typography and composition. Use accent colors sparingly and consistently. Make hover, selected, warning, error, and success states clear.

**Shape and surfaces:** Use radii, borders, shadows, and elevation according to interface structure. Not every element needs a border, a card, and a shadow. Prefer fewer purposeful surface levels.

**Images and graphics:** Favor content-relevant imagery, illustration, or data visualization. Avoid generic stock photos, meaningless orbs, noisy abstract backgrounds, and decorative charts. No emoji-as-icon shortcuts unless the product's voice explicitly calls for them.

**Subtle background imagery can help.** A faint station photograph, architectural detail, material texture, archival print, cartographic fragment, landscape, or product-specific illustration can make a design feel placed in a real world instead of a blank component playground. Background images are an optional tool, not a required decoration. Choose imagery *because it belongs to the product's world*. Crop it intentionally; desaturate, tint, mask, or overlay it so text and controls stay fully legible. Where content overlays an image, use a robust contrast-preserving surface/gradient rather than hoping opacity is low enough. Keep responsive focal points and lightweight assets; include licensing/attribution where needed. Never let the image be the sole carrier of essential information.

**Microcraft:** Choose one purposeful visual detail and carry it through with restraint—line rhythm, row selection, diagrams, number formatting, icon geometry, caption placement, or a distinctive responsive transition. Favor intentional optical alignment over mechanically identical padding everywhere.

**Motion:** Animate changes in state, hierarchy, or navigation when useful. Avoid uniform fade-in on every section and pointless hover theatrics. Honor reduced-motion preferences.

### 5. Implement faithfully

- Work within the existing technology stack and component conventions unless asked to change them.
- Use shared design tokens/CSS variables for color, typography, spacing, radius, and motion. Keep them easy to adjust.
- Treat off-the-shelf component libraries as accessibility/behavior infrastructure, not the finished visual identity. Customize their visual system consistently.
- Make layouts work on narrow and wide screens, including long labels and variable content.
- Support keyboard navigation, visible focus, readable contrast, semantic controls, sensible hit targets, and empty/loading/error states as appropriate.
- Use functional, real interface behavior where requested; never substitute a decorative mockup for working UI.

### 6. Audit the result and revise it

If a preview or screenshot tool is available, inspect the rendered UI at desktop and mobile widths. Otherwise review the code and composition for the same issues. Never claim to have visually inspected something you did not inspect.

Ask:

1. **Identity:** Could the product name and logo be swapped with a random startup without the design feeling wrong? If yes, make the direction more specific.
2. **Template smell:** Are there multiple consecutive sections using the same centered title + subtitle + identical cards? Reconsider the information architecture.
3. **Hierarchy:** Is the most important thing obvious in three seconds? Can a user find the next action?
4. **Authenticity:** Do the copy, visuals, and data belong to this specific product? Remove generic filler and false polish.
5. **Craft:** Do typographic rhythm, spacing, alignments, states, and edge cases feel finished?
6. **Utility:** Is the interface still usable, accessible, fast, and responsive?

**Run two passes rather than merely restyling:**

- **Pass A — structural:** Is this the right interface for the job? Change layout, information order, labels, density, and interaction if necessary.
- **Pass B — art direction:** Strengthen the one chosen idea. Improve typographic hierarchy, meaningful imagery, transitions, alignment, and finished details; remove gratuitous flourishes.

If a screenshot is available, inspect at least one desktop and one narrow/mobile width. Ask if the interface would remain recognizable after replacing its product name and brand color; if yes, the distinctive idea is still too weak. Fix the most consequential weakness, then re-check. Do not stop at a first-pass screenshot that merely looks attractive.

## Recognizable AI patterns to challenge

These are **red flags, not absolute bans**. A choice is allowed when it has a clear product-specific reason.

- Purple-to-blue gradients, glows, floating blurred orbs, and glassmorphism used as default identity.
- A centered eyebrow pill, oversized generic headline, gray paragraph, and two CTA buttons on every landing page.
- Rows of three or six identical rounded feature cards with icon tiles and equal-length copy.
- Cards nested inside cards, shadows on every surface, and one radius applied indiscriminately.
- Overuse of generic iconography, decorative graphs, fake activity feeds, vanity metrics, and meaningless badges.
- Symmetry and spacing so uniform that nothing has priority.
- Generic promises such as “Reimagine your workflow” or “Everything you need, all in one place.”
- Template dashboards that make every KPI visually equal regardless of relevance.

Also challenge **second-wave anti-slop clichés**: an automatic cream/terracotta palette, obligatory giant editorial serif, acid-green-on-charcoal accents, random asymmetry, excessive monospace labels, arbitrary section numbers, and “one word in a different color” headlines. Replacing one recognizable template with another is not success.

## Context-specific defaults

- **Operational or analytics software:** Prioritize information density, scanning, tables, states, navigation, and domain-specific visual hierarchy. Less decoration, more precision.
- **Consumer app:** Prioritize task flow, emotional appropriateness, discoverability, approachable copy, and touch ergonomics.
- **Editorial or portfolio:** Let content, art direction, typography, and pacing lead. Unusual composition is appropriate only when reading and navigation remain clear.
- **Commerce:** Product imagery, comparison, pricing, availability, trust, and checkout clarity should dominate.
- **B2B landing page:** Use product proof and specific messaging; resist empty abstractions and overly generic hero formulas.

## Acceptance gate

Before finishing, verify all of the following:

- [ ] At least three genuinely different directions were considered, and a clear context-specific design thesis guided the work.
- [ ] The screen has a deliberate focal point and useful information hierarchy.
- [ ] The design does not depend on generic AI visual tropes for its personality.
- [ ] The result is not merely the latest fashionable "anti-AI" template.
- [ ] Typography, layout, color, imagery (including subtle background images where useful), and details form one coherent system.
- [ ] Mobile/responsive, accessibility, and interaction states are considered.
- [ ] No unsupported product claims, fabricated social proof, or decorative fake metrics were added.
- [ ] Both a structural critique and a visual-art-direction revision were completed.

If a gate fails, improve the result before delivering. For constrained tasks, prioritize fixing context, hierarchy, and usability over decorative distinctiveness.

## Output behavior

Deliver the actual requested code/design first. When useful, summarize the design thesis in 1–3 sentences and identify any consequential tradeoffs. Do not turn the process into a lengthy lecture or ask for aesthetic preferences that can be reasonably inferred.


## When asked to “push it further”

Increase **product specificity, not visual noise**. Prioritize: (1) a bolder content-driven composition, (2) a stronger intentional typographic contrast, (3) a single unforgettable but usable domain-specific motif, (4) considered photography, illustration, or **subtle background images** if they add atmosphere, and (5) polished interaction states. Never interpret “more design” as more cards, shadows, ornamental labels, random animation, or gratuitous asymmetry.
