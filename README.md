# deep-thinking

A Claude Code skill that provides a comprehensive deep reasoning framework for systematic, thorough thinking on complex tasks — automatically applied for multi-step problems, ambiguous requirements, architectural decisions, and debugging sessions.

Inspired by [Claude God Mode](https://jaglab.org/claude-god-mode/).

## Installation

Add this to your Claude Code project settings (`.claude/settings.json`) or user settings:

```json
{
  "skills": [
    "github:amankr-novo/deep-thinking"
  ]
}
```

Or install from the CLI:

```bash
claude skill add github:amankr-novo/deep-thinking
```

## Prerequisites

- None. This skill works automatically with any Claude Code session — no external tools, APIs, or configuration required.

## Usage

This skill activates **automatically** based on task complexity. No slash command is needed.

### When It Activates

| Trigger | Example |
|---|---|
| Multiple valid approaches with trade-offs | "Should I use Redis or in-memory caching?" |
| Ambiguous or underspecified requirements | "Make the app faster" |
| Architectural or design decisions | "Add real-time updates to the dashboard" |
| Systematic debugging | "Users are seeing intermittent 500 errors" |
| Changes touching multiple systems or files | "Refactor the authentication system" |
| High-stakes changes (data, security, production) | "Migrate the database schema" |
| Explicit request | "Think deeply about this", "Analyze carefully" |

### When It Skips

Trivial, single-step tasks with obvious solutions — typo fixes, simple renames, one-line changes.

## Thinking Phases

| Phase | What it does |
|---|---|
| **Initial Engagement** | Rephrases the problem, identifies knowns vs. unknowns, maps required knowledge areas, flags ambiguities. |
| **Problem Decomposition** | Breaks the task into components, identifies explicit and implicit requirements, defines success criteria. |
| **Multiple Hypotheses** | Generates 2-3+ approaches before committing. Evaluates trade-offs across complexity, performance, maintainability, and risk. |
| **Natural Discovery** | Follows leads like a detective — starts with the obvious, digs deeper, questions assumptions, circles back with new context. |
| **Verification** | Tests conclusions against evidence, seeks counter-examples, checks for edge cases and logical consistency. |
| **Knowledge Synthesis** | Connects findings into a coherent picture, extracts reusable principles, notes downstream effects. |
| **Recursive Application** | Applies the same analysis at both macro (architecture) and micro (function) levels. |

## Adaptive Depth

The skill scales analysis depth based on the situation:

| Factor | Shallow | Deep |
|---|---|---|
| **Complexity** | Simple lookup | Multi-dimensional problem |
| **Stakes** | Low-risk formatting | Production database migration |
| **Time sensitivity** | Quick fix needed now | Long-term architecture decision |
| **Information** | Complete spec | Vague description |
| **Scope** | One file change | Cross-module refactor |

## Anti-Patterns

| Anti-Pattern | Instead Do |
|---|---|
| Jumping to implementation immediately | Analyze the problem space first |
| Considering only one approach | Generate and compare alternatives |
| Ignoring edge cases | Actively seek boundary conditions |
| Assuming without verifying | Read the code, check the docs |
| Over-engineering simple tasks | Match depth to complexity |
| Analysis paralysis on trivial decisions | Set a time-box, then decide |
| Drawing premature conclusions | Verify with evidence before committing |
| Not seeking counter-examples | Actively look for cases that disprove your theory |
| Mechanical checklist thinking | Let reasoning flow organically |

## Verification Checklist

Before delivering a response, the protocol verifies:

- All aspects of the original question are addressed
- Conclusions are supported by evidence (not assumptions)
- Edge cases and failure modes are considered
- Trade-offs are explicitly stated
- The recommended approach is justified over alternatives
- No logical inconsistencies in the reasoning
- Detail level matches the user's expertise and needs

## Repo Structure

```
deep-thinking/
  deep-thinking/
    SKILL.md              # Skill definition (protocol, phases, quality metrics)
    reference.md          # Reference guide (thinking patterns, domain examples)
```
