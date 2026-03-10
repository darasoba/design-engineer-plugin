# Design Engineer Plugin for Claude Code

A Claude Code skill that brings **design engineering craft** to your development workflow — the intersection of design and code, focused on interaction quality, motion, and the invisible details that make interfaces feel alive.

Inspired by the design engineering community and resources curated at [desengs.com](https://desengs.com/).

## What It Does

When you ask Claude Code to build UI components, animations, or interactive experiences, this skill activates and guides it to:

- Apply proper **timing and easing** (no more `linear` or default transitions)
- Follow the **12 Principles of Animation** adapted for UI
- Build components with **all interaction states** (hover, active, focus, disabled, loading)
- Use **spring physics** and custom cubic-bezier curves that feel natural
- Implement **scroll-driven effects**, staggered reveals, and orchestrated animations
- Add **sound and haptic feedback** where appropriate
- Respect **accessibility** (`prefers-reduced-motion`, keyboard navigation, touch targets)
- Think in **design systems** (tokens, variants, composition)
- Prioritize **performance** (compositor-only animations, containment, intersection observers)

## Install

```bash
# From the Claude Code CLI
/plugin install design-engineer
```

Or clone and use locally:

```bash
git clone https://github.com/israelsobaloju/design-engineer-plugin.git
claude --plugin-dir ./design-engineer-plugin
```

## Triggers

The skill activates when you mention:

- "design engineer", "interaction design", "micro-interactions"
- "craft", "polish", "delight", "feel right"
- "animation", "motion design", "haptics"
- "toast", "command palette", "design system components"
- Or any request for interfaces that feel alive and meticulously detailed

## Examples

```
> Build a toast notification system with stacking and swipe-to-dismiss

> Create a command palette component with keyboard navigation

> Add scroll-driven reveal animations to this page

> Make this button feel more responsive — add proper interaction states

> Build a modal with spring physics and focus trapping
```

## What's Inside

```
design-engineer-plugin/
├── .claude-plugin/
│   └── plugin.json
├── skills/
│   └── design-engineer/
│       └── SKILL.md
└── README.md
```

## Inspired By

Built from the collective knowledge of the design engineering community:

- [Rauno Freiberg](https://rauno.me/) — Invisible Details of Interaction Design, Web Interface Guidelines
- [Emil Kowalski](https://emilkowal.ski/) — Developing Taste, Sonner, animations.dev
- [The Component Gallery](https://component.gallery/) — Interface component reference
- [Design Engineering Club](https://designeng.club/) — Community
- [Devouring Details](https://devouringdetails.com/) — Interactive reference for interaction design
- [desengs.com](https://desengs.com/) — The ultimate resource hub for design engineers

## License

MIT
