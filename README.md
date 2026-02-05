# Prompt Generator UI

Universal Design Prompt Generator (Ultimate Edition) — a single-file, offline tool to think through UI/UX decisions and generate structured prompts for design tools and AI assistants.

Open the app: [prompt-generator.html](/prompt-generator.html)

## Overview

This UI helps you capture design intent across context, visual direction, layout, design system, UX strategy, technical handoff, and marketing assets. It produces prompt output in three formats:

- Markdown — human-readable spec
- Plain text — compact, single-block text
- JSON — machine-readable schema

No build, no server. State is saved locally in your browser.

## Quick Start

- Open the HTML file in a modern browser (Chrome, Edge, Firefox, Safari).
- Fill sections in the left sidebar (accordions 1–15).
- Choose output format: Markdown, Plain, or JSON.
- Use Copy, Download, or Export to save results.
- Toggle theme (Dark/Light) to match your environment.
- Save a preset, load later, or share via a link.

## Core Features

- Structured prompt output: Markdown, Plain, JSON
- Comprehensive design inputs (15 sections)
- Presets: SaaS, Fintech, Portfolio
- Local autosave and named presets
- Shareable state via URL hash
- Theme toggle (Dark/Light)
- Output character and token estimates
- Import/Export JSON config

Key functions: [updatePrompt](/prompt-generator.html#L1755-L2083), [applyState](/prompt-generator.html#L1646-L1671), [exportConfig](/prompt-generator.html#L1685-L1691), [copyShareLink](/prompt-generator.html#L1703-L1713), [toggleTheme](/prompt-generator.html#L2159-L2166).

## Usage

1. Core Context
   - Role, Project Type, Goal, Audience, Decision, AI Tool
2. Visual DNA
   - Mood, Style spectrum, Representation, Form language, Energy and tone
3. Design Techniques
   - Movements (Glassmorphism, Swiss), Lighting, Materials
4. Layout & Structure
   - Frame, Navigation, Hero, Key sections
5. Design System
   - Typography, Colors, Buttons, Cards, Inputs, Spacing, Grid, Radius, Interactive states
6. Technical Implementation
   - Handoff, Component docs, Performance, Testing, Motion
7. UX Strategy & Content
   - Principles, Accessibility, Responsive behavior, Output format
8. Campaign Brief
   - Objective, KPI, Budget, Timeline, Channels, Audience, Geo, Compliance
9. Creative Requirements
   - Assets, Copy tone, Brand elements, Legal
10. Testing Plan
   - Hypotheses, Variants, Metrics, Rollout
11. Tracking & Handoff
   - UTM, Naming, Experiments, Events
12. Prompt Quality Controls
   - Context, Intent, Constraints, Negatives, Length, Structure
13. Few-shot Examples
   - Add exemplary inputs and ideal outputs
14. Citations & Safety
   - Fact-check, Authoritative sources, Privacy, Critique
15. Response Schema & Language
   - Preferred language, voice/tone, JSON/Markdown schema

## Output Formats

- Markdown: Structured design spec with sections and checklists.
- Plain: Single text block optimized for quick pasting.
- JSON: Schema with these top-level keys:
  - role, type, goal, audience, decision, aiTool
  - visual, layout, components, technical, ux
  - campaign, creative, qa, tracking
  - prompt_quality, few_shot, safety, response

## Presets & State

- Autosave restores your last session automatically.
- Save Preset, Load Preset, Delete Preset manage named configurations.
- State and presets are stored in localStorage on your device.

## Share Links

- Share encodes the current configuration into the URL hash (#state=…).
- Open the shared link to load the configuration in another browser instance.

## Import / Export

- Export JSON writes a prompt-config.json you can version and share.
- Import JSON loads a previously exported configuration.

## Theme & Counts

- Toggle Theme switches Dark/Light via CSS variables.
- Counts show character length and approximate token usage for prompt planning.

## UI/UX Checklists

- Visual Hierarchy
  - Clear primary action, scannable headings, consistent spacing
- Cognitive Load
  - Progressive disclosure, chunking, minimal choices per step
- Readability
  - WCAG AA contrast, 16px+ body size, line-length 60–80 chars
- Consistency
  - Shared components, tokens, grid, interaction states
- Accessibility
  - Keyboard navigation, focus indicators, semantic structure, screen reader support
- Responsiveness
  - Mobile-first strategy, flexible layouts, adaptive assets

## Design Prompts Tips

- State user intent and constraints explicitly.
- Prefer outcomes over features in copy.
- Name style anchors (mood, energy, materials).
- Specify layout primitives (hero, nav, sections).
- Include handoff and testing requirements.
- Add few-shot examples to steer outputs.

## Performance Guidance

- Optimize assets (SVG where possible, responsive images).
- Avoid unnecessary motion; prefer subtle micro-interactions.
- Defer non-essential work; consider lazy loading for content-heavy pages.

## Privacy & Security

- No network calls; data stays client-side.
- Configurations are stored locally; clear browser storage to remove them.
- Avoid entering sensitive or personal data.

## Browser & OS Notes

- Works on Windows and Linux with any modern browser.
- Recommended: Microsoft Edge or Chrome on Windows.

## File Structure

- Single file app: [prompt-generator.html](/prompt-generator.html)
- License: [LICENSE](/LICENSE)

## Roadmap Ideas

- More presets and example libraries
- Advanced export templates (Figma tokens, Storybook seed)
- Multi-language bundles and localized copy helpers
- Component checklist for design-to-dev handoff

## License

See [LICENSE](/LICENSE).
