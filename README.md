# Design Engineer — AI Rules for Every Tool

Bring **design engineering craft** to any AI coding assistant — the intersection of design and code, focused on interaction quality, motion, and the invisible details that make interfaces feel alive.

Inspired by the design engineering community and resources curated at [desengs.com](https://desengs.com/).

## What It Does

When your AI builds UI components, animations, or interactive experiences, these rules guide it to:

- Apply proper **timing and easing** (no more `linear` or default transitions)
- Follow the **12 Principles of Animation** adapted for UI
- Build components with **all interaction states** (hover, active, focus, disabled, loading)
- Use **spring physics** and custom cubic-bezier curves that feel natural
- Implement **scroll-driven effects**, staggered reveals, and orchestrated animations
- Add **sound and haptic feedback** where appropriate
- Respect **accessibility** (`prefers-reduced-motion`, keyboard navigation, touch targets)
- Think in **design systems** (tokens, variants, composition)
- Prioritize **performance** (compositor-only animations, containment, intersection observers)

## Quick Install (All AI Tools)

One command installs the skill across **all your AI agents** — Claude Code, Cursor, Codex, Gemini CLI, OpenCode, Amp, and more:

```bash
npx skills add darasoba/design-engineer-plugin@design-engineer
```

Browse on the skills registry: [skills.sh](https://skills.sh/)

## Manual Install by Tool

### Claude Code (Plugin)

```bash
claude --plugin-dir ./design-engineer-plugin
```

### Cursor

Copy `rules/.cursorrules` to your project root:

```bash
cp rules/.cursorrules /path/to/your/project/.cursorrules
```

Or set it globally in Cursor Settings > Rules > User Rules.

### Windsurf

Copy `rules/.windsurfrules` to your project root:

```bash
cp rules/.windsurfrules /path/to/your/project/.windsurfrules
```

### GitHub Copilot

Copy to your repo's `.github/` directory:

```bash
mkdir -p /path/to/your/project/.github
cp rules/copilot-instructions.md /path/to/your/project/.github/copilot-instructions.md
```

### Cline (VS Code)

Copy `rules/.clinerules` to your project root:

```bash
cp rules/.clinerules /path/to/your/project/.clinerules
```

### ChatGPT

1. Open ChatGPT > Settings > Personalization > Custom Instructions
2. Paste the contents of `rules/chatgpt-custom-instructions.md` into "How would you like ChatGPT to respond?"

Or use it as the system prompt when creating a **custom GPT**.

### Claude Projects (claude.ai)

1. Open your Claude Project > Project Settings
2. Paste the contents of `rules/system-prompt.md` into the project instructions

### Any Other AI (Universal)

Use `rules/system-prompt.md` — it works as a system prompt for:
- **OpenAI API / Playground** — paste as system message
- **Local LLMs** (Ollama, LM Studio, llama.cpp) — use as system prompt
- **Aider** — save as `.aider.conf.yml` convention or paste in chat
- **Continue.dev** — add to `.continuerules`
- **Any AI tool** that accepts custom instructions or a system prompt

## What's Inside

```
design-engineer-plugin/
├── .claude-plugin/
│   └── plugin.json                        # Claude Code plugin manifest
├── skills/
│   └── design-engineer/
│       └── SKILL.md                       # Claude Code skill
├── rules/
│   ├── .cursorrules                       # Cursor
│   ├── .windsurfrules                     # Windsurf
│   ├── .clinerules                        # Cline
│   ├── copilot-instructions.md            # GitHub Copilot
│   ├── chatgpt-custom-instructions.md     # ChatGPT / Custom GPTs
│   └── system-prompt.md                   # Universal (any AI)
├── LICENSE
└── README.md
```

## Examples

```
> Build a toast notification system with stacking and swipe-to-dismiss

> Create a command palette component with keyboard navigation

> Add scroll-driven reveal animations to this page

> Make this button feel more responsive — add proper interaction states

> Build a modal with spring physics and focus trapping
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
