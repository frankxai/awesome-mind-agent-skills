# Awesome Mind Agent Skills

> A curated index of open-source projects, tools, papers, MCP servers, agent skills, and frameworks for mind intelligence — spanning second brains, memory systems, neuroscience, psychology, learning science, and research agents.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

**See the swarm diagram**: [assets/diagrams/mind-intelligence-swarm-architecture.html](../assets/diagrams/mind-intelligence-swarm-architecture.html)

---

## Purpose

This list exists at the intersection of **human cognition** and **machine intelligence**. It serves three distinct audiences simultaneously:

**Knowledge workers and researchers** building personal knowledge infrastructure — people who want to externalise memory, accelerate synthesis, and connect ideas across disciplines (neuroscience, psychology, learning science, philosophy of mind).

**AI engineers and agent builders** who need a structured map of capabilities: which MCP servers expose memory tooling, which skills are composable for research workflows, which frameworks wire into second-brain systems.

**Multi-agent swarms** that need a machine-readable discovery layer — a catalogue of what exists, what it does, and how components connect, so agents can self-direct toward the right tool without human lookup.

The curation principle: **depth over breadth**. Each entry earns its place by being genuinely useful, actively maintained (or historically significant), and either open-source or openly documented. No link-farms. No dead projects without a note on why they are still worth reading.

---

## How People Explore

The categories below reflect natural inquiry paths a human researcher takes. Each file is a self-contained reading list for that domain.

| Category | What you will find | Good for |
|---|---|---|
| [Second Brain](categories/second-brain.md) | PKM tools, note-taking frameworks, graph databases, linking schemas | Anyone building a personal knowledge system |
| [Memory Systems](categories/memory-systems.md) | Spaced repetition, episodic memory tools, semantic stores | Learning scientists, memory researchers |
| [Neuroscience](categories/neuroscience.md) | Open datasets, analysis libraries, brain atlases, cognitive models | Researchers, curious minds |
| [Psychology](categories/psychology.md) | Cognitive science papers, behavioural models, IFS/parts work, decision-making | Self-development practitioners, therapists |
| [Learning Science](categories/learning-science.md) | Pedagogy tools, retrieval practice, interleaving, metacognition | Educators, self-directed learners |
| [Agent Skills](categories/agent-skills.md) | Claude skills, prompt libraries, Fabric patterns, agent templates | AI engineers, agent composers |
| [MCP Servers](categories/mcp-servers.md) | Memory, search, graph, and knowledge MCP implementations | Claude Code users, MCP integrators |
| [Research Agents](categories/research-agents.md) | Autonomous research frameworks, paper agents, hypothesis engines | Researchers, power users |
| [Quantified Self](categories/quantified-self.md) | Biometrics, sleep tracking, HRV, cognitive performance | Self-optimisers |
| [Open Science](categories/open-science.md) | Reproducible research tooling, open data, preprint platforms | Scientists, open-access advocates |

### Browsing tips

- **Start with a domain** (e.g. neuroscience) and follow `Integrates with` cross-references to adjacent categories.
- **Filter by `Type:`** fields inside each file — `tool`, `paper`, `dataset`, `MCP`, `skill`, `framework` — to narrow to what you can actually use today.
- **Sections marked `[unverified]`** are placeholders that passed initial curation but await a link-check pass. They are worth investigating; do not discard them.

---

## How Agents Use This List

This repository is designed to be **agent-readable** as well as human-readable. Each category file follows a consistent schema agents can parse without special tooling:

```
## <Section Name>

### <Entry Name>
- **Repo/URL**: <link>
- **Type**: <tool | paper | dataset | MCP | skill | framework>
- **Integrates with**: <comma-separated list>
- **Agent use case**: <one sentence on how an agent would invoke or reference this>
```

### Discovery workflow

An agent exploring this list typically:

1. **Scans the category table** in this README to narrow domain ("I need a memory store" → `categories/mcp-servers.md`).
2. **Filters by `Type: MCP`** inside the file to find directly invocable servers.
3. **Follows `Integrates with`** to find the full capability chain (e.g. Obsidian → Self-hosted MCP bridge → Logseq export format).
4. **Uses `Agent use case` fields** as prompt fragments — they are written as capability descriptions an LLM can match against a user intent.

### Skill auto-loading pattern

When a research agent in the Starlight swarm needs a capability it does not have locally, it can:

```
1. Read categories/<relevant>.md
2. Find entries with Type: skill or Type: MCP
3. Check Integrates with: Claude Code
4. Load via: npx skills add <skill-id>
        or: register MCP server in .claude/settings.json
```

This list is the swarm's **capability registry** — a verified map of what already exists before an agent invents a solution from scratch.

---

## Usefulness for the Swarm

In a multi-agent architecture (e.g. the Starlight Intelligence System), this list functions as a **shared knowledge substrate** for the entire fleet:

### 1. Capability Discovery Before Hallucination

Agents have a tendency to invent tools when none is named in their context. A structured, verified catalogue gives the orchestrator a ground-truth lookup step: *does this capability exist as a real tool before I ask an agent to build it from scratch?*

### 2. Routing by Specialisation

The category taxonomy maps directly to agent specialisations. A `neuroscience` query routes to agents that have loaded `categories/neuroscience.md` as working context. The list becomes a **curriculum** for specialised sub-agents without requiring long system prompts.

### 3. Composable Building Blocks

The `Agent use case` fields in each category are written as tool-call descriptions. An orchestrator can read them as a soft catalogue of available sub-operations and chain them into novel workflows without hallucinating capability names.

### 4. Reducing Cold-Start Cost

New agents (or new conversations) can load a single category file as working context rather than performing open-ended web searches. The list is dense, pre-filtered, and structured — optimised for LLM consumption, not human skimming.

### 5. Cross-Domain Synthesis

The swarm's most valuable work happens at category intersections: neuroscience × second-brain, psychology × agent-skills, quantified-self × learning-science. This list makes those intersections explicit through `Integrates with` fields, giving agents a map of non-obvious connections.

---

## Category Status

```
categories/
├── second-brain.md        ✅  seeded
├── neuroscience.md        ✅  seeded
├── agent-skills.md        ✅  seeded
├── memory-systems.md      🔜  structure ready, entries pending
├── psychology.md          🔜  structure ready, entries pending
├── learning-science.md    🔜  structure ready, entries pending
├── mcp-servers.md         🔜  structure ready, entries pending
├── research-agents.md     🔜  structure ready, entries pending
├── quantified-self.md     🔜  structure ready, entries pending
└── open-science.md        🔜  structure ready, entries pending
```

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for entry format, quality bar, and the verification process.

Link verification passes run on a scheduled Codex agent. Entries marked `[unverified]` are placeholders awaiting a search check — flag with a PR comment rather than removing.
