# Awesome Mind Agent Skills [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![Built on SIP](https://img.shields.io/badge/Built%20on-SIP-c9b6ff.svg)](https://github.com/frankxai/Starlight-Intelligence-System)
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0%201.0-lightgrey.svg)](LICENSE)

> A curated guide to agentic systems, skills, and resources for understanding, structuring, and extending the human mind — the front door to the Mind Intelligence ecosystem.

The thesis in one line: a mind is not one thing — it's attention, memory, emotion, belief, and nine other constructs that interact. The interesting work isn't building one monolithic "mind app"; it's modeling those constructs cleanly, then composing agents and skills that read and structure your own thinking against them. This list is the map of the systems that do that.

One discipline runs through everything here: these systems **model** a mind, they never **diagnose** one. Observation, interpretation, and hypothesis stay separate from anything clinical. If you want the deep version of that rule, it lives in [agentic-mind-os](https://github.com/frankxai/agentic-mind-os).

## Contents

- [The Mind Intelligence ecosystem](#the-mind-intelligence-ecosystem)
- [By cognitive construct](#by-cognitive-construct)
- [Agent skills](#agent-skills)
- [Related ecosystems](#related-ecosystems)
- [Start here](#start-here)
- [Contributing](#contributing)
- [License \& attestation](#license--attestation)

## The Mind Intelligence ecosystem

Every repo in the swarm, grouped by family. Naming doctrine: **OS** = lived (you run it daily), **System** = engineered (a runtime/schema you build on), **Systems** = a category portfolio. `live` ships today; `planned` is chartered but not yet built — listed honestly so the map matches reality.

### Canon

| Repo | Role | Status |
|---|---|---|
| [mind-intelligence-systems](https://github.com/frankxai/mind-intelligence-systems) | The umbrella. Naming doctrine, the 12-module human-mind model, and the repo mesh that defines who depends on whom. | live |

### Cognitive

| Repo | Role | Status |
|---|---|---|
| [human-mind-intelligence-system](https://github.com/frankxai/human-mind-intelligence-system) | The engineered System above the model — cognitive schemas, an ontology, and response-prediction. Turns the 12 constructs into something agents can reason over. | live |

### Lived OS

| Repo | Role | Status |
|---|---|---|
| [agentic-mind-os](https://github.com/frankxai/agentic-mind-os) | The personal mind OS lived daily — a local-first vault, a fleet of personal agents, and a weekly review loop built on the canonical model. | live |
| [starlight-mind-os-pro](https://github.com/frankxai/starlight-mind-os-pro) | Premium distribution of the lived OS — guided onboarding, dashboards, and workshop material for people who want the system without assembling it. | live |

### Discovery

| Repo | Role | Status |
|---|---|---|
| [awesome-mind-agent-skills](https://github.com/frankxai/awesome-mind-agent-skills) | This curated map — the front door that links every node in the swarm. | live |

### Memory palace

| Repo | Role | Status |
|---|---|---|
| [mind-palace-agent-skills](https://github.com/frankxai/mind-palace-agent-skills) | The Blessing-Protocol skills — ingest a builder's GitHub, witness the week, and grow a palace from what is whole. | live |
| [frankx-mind-palace](https://github.com/frankxai/frankx-mind-palace) | Frank's own blessed work as data — the reference instance the palace skills produce. | live |

### Research

| Repo | Role | Status |
|---|---|---|
| [research-intelligence-os](https://github.com/frankxai/research-intelligence-os) | A reusable research runtime — the engine other verticals run their literature work through. | planned |
| [research-intelligence-systems](https://github.com/frankxai/research-intelligence-systems) | The cross-domain research portfolio that sits above the individual verticals. | planned |
| [psychology-research-intelligence-system](https://github.com/frankxai/psychology-research-intelligence-system) | The psychology vertical — research that feeds the human-mind model evidence. | planned |
| [neuroscience-research-intelligence-system](https://github.com/frankxai/neuroscience-research-intelligence-system) | The neuroscience vertical — the biological substrate behind the constructs. | planned |

## By cognitive construct

The human-mind model has **12 modules**. Each is defined in `models/human-mind/<module>.md` in the [canon repo](https://github.com/frankxai/mind-intelligence-systems/tree/main/models/human-mind), and each is also a shared lens the lived OS and palace skills read your notes against. The table points to the model file and names which skill touches the construct most directly.

| Construct | Model file | Touched by |
|---|---|---|
| **attention** | [attention.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/attention.md) | `weekly-blessing` (what you attended to vs. ignored this week) |
| **memory** | [memory.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/memory.md) | `palace-build` (turns a ledger into recallable rooms); `mind-skills` consolidation |
| **emotion** | [emotion.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/emotion.md) | `weekly-blessing` (what moved you) |
| **motivation** | [motivation.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/motivation.md) | `weekly-blessing` (the one path forward) |
| **identity** | [identity.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/identity.md) | `blessing-standard` (`soul.md` — what the repo, or builder, is) |
| **learning** | [learning.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/learning.md) | `mind-skills` recall builder (active recall against the week) |
| **belief** | [belief.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/belief.md) | the cognitive System's response-prediction layer |
| **behavior** | [behavior.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/behavior.md) | `github-bless` (what you actually shipped, not what you intended) |
| **consciousness** | [consciousness.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/consciousness.md) | the human-mind model (reference construct) |
| **metacognition** | [metacognition.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/metacognition.md) | `weekly-blessing` + `mind-skills` review (the core of the loop — thinking about your thinking) |
| **decision-making** | [decision-making.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/decision-making.md) | `weekly-blessing` (ratify what is whole, name what to ignore) |
| **social-cognition** | [social-cognition.md](https://github.com/frankxai/mind-intelligence-systems/blob/main/models/human-mind/social-cognition.md) | `github-bless` connectors (collaboration signal across repos) |

## Agent skills

The skills that exist in the swarm today, plus the planned set in the lived OS. Each is a self-contained `SKILL.md` — portable across Claude Code, Claude.ai, Cursor, Codex, Gemini, and any runtime that reads them.

### Blessing Protocol (mind-palace-agent-skills) — live

The four skills that turn a week of work into a memory palace. The loop: **ingest → witness → grow**, with an onboarding step to make any repo blessable.

- [`github-bless`](https://github.com/frankxai/mind-palace-agent-skills/blob/main/skills/github-bless/SKILL.md) — **ingest.** Rolls the week's commits and merged PRs across repos and connectors into a candidate set, and names every gap. Reads the week; blesses nothing itself.
- [`weekly-blessing`](https://github.com/frankxai/mind-palace-agent-skills/blob/main/skills/weekly-blessing/SKILL.md) — **witness.** The Sunday ritual: a six-section entry that ratifies what is whole, names what to ignore for seven days, and surfaces the one path forward. Invoked, never auto-fired.
- [`palace-build`](https://github.com/frankxai/mind-palace-agent-skills/blob/main/skills/palace-build/SKILL.md) — **grow.** Turns the blessing ledger into `rooms.json` plus a portable, build-step-free HTML palace that grows each week.
- [`blessing-standard`](https://github.com/frankxai/mind-palace-agent-skills/blob/main/skills/blessing-standard/SKILL.md) — **onboard.** Scaffolds the five Blessing Protocol files (`soul.md`, `agent.md`, `skills.md`, `palace.md`, `bless.md`) into any repo and fills them from what the repo already is.

### Mind-skills (agentic-mind-os) — planned

The personal mind OS ships a set of **mind-skills** its agent runtime auto-activates — the consolidation half of the loop, anchored to the 12 constructs. They live alongside the [personal agent cards](https://github.com/frankxai/agentic-mind-os) (cartographer, weekly-reviewer, focus coach, recall builder) and the `/map-mind` + `/review-week` commands. See [agentic-mind-os/skills](https://github.com/frankxai/agentic-mind-os).

## Related ecosystems

Sibling [frankxai](https://github.com/frankxai) systems that genuinely compose with the mind swarm. Linked because each one carries weight here, not for completeness.

- [Starlight Intelligence System](https://github.com/frankxai/Starlight-Intelligence-System) — the **SIP substrate** every repo in this list is built on. The persistent context, agent-identity, and attestation layer; "Built on SIP" on a repo means it composes the Starlight Intelligence Protocol and honors its sovereignty clause.
- [second-brain-os](https://github.com/frankxai/second-brain-os) — a **memory/knowledge OS**: a two-vault Obsidian template with hard privacy separation, where your coding-agent session is the compute that summarizes your thinking. The knowledge-management neighbor to the lived mind OS — where the mind OS models *how* you think, the second brain stores *what* you know.

## Start here

A short path for someone new to all of this:

1. **You are here.** Read this list top to bottom. It's the map — you don't need to clone anything yet.
2. **Install the lived OS.** Clone [agentic-mind-os](https://github.com/frankxai/agentic-mind-os), copy its vault skeleton somewhere you live, and drop its agents + skills into your runtime. Write a daily note; run `/review-week` on Sunday. This is the one repo you actually live in.
3. **Add the palace.** Want your shipped work to accumulate into something you can walk through? Add the [mind-palace-agent-skills](https://github.com/frankxai/mind-palace-agent-skills) and run the **ingest → witness → grow** loop weekly.
4. **Read canon when you need it.** When an agent asks about your *attention* or *belief* state and you want the precise definition, the [12-module model](https://github.com/frankxai/mind-intelligence-systems/tree/main/models/human-mind) is the source of truth. Read it on demand, not up front.

## Contributing

PRs welcome — add a repo, a skill, or a related ecosystem that genuinely belongs. Keep links live, keep claims verifiable, and say in one clause why an entry earns a reader's time. One entry per PR; match the format of the section you're adding to. Status must be honest: `planned` is not `live`. And the hard line holds — nothing clinical or diagnostic gets in. See the [contribution guidelines](CONTRIBUTING.md).

## License \& attestation
[CC0 1.0](LICENSE) — curation dedicated to the public domain.
**Built on SIP.** Part of the [Mind Intelligence Systems](https://github.com/frankxai/mind-intelligence-systems) portfolio, composing the [Starlight Intelligence Protocol](https://github.com/frankxai/Starlight-Intelligence-System).
Built by [Frank Riemer](https://frankx.ai). For builders, not consumers.
