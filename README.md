# Deep Thinking

## Overview

This skill provides a comprehensive deep reasoning framework that guides systematic, thorough thinking for complex tasks. It automatically applies for multi-step problems, ambiguous requirements, architectural decisions, debugging sessions, and any task requiring careful analysis beyond surface-level responses.

Inspired by [Claude God Mode](https://jaglab.org/claude-god-mode/), this protocol ensures responses stem from genuine understanding and careful reasoning rather than superficial analysis.

## When to Apply

Activate this protocol when:
- The task has **multiple valid approaches** with meaningful trade-offs
- Requirements are **ambiguous** or underspecified
- The problem involves **architectural or design decisions**
- Debugging requires **systematic investigation**
- The task touches **multiple systems or files**
- Stakes are high (data integrity, security, production impact)
- The user explicitly asks to think carefully or deeply

Skip for trivial, single-step tasks with obvious solutions.

## Core Thinking Sequence

### 1. Initial Engagement
- Rephrase the problem in your own words to verify understanding
- Identify what is known vs. unknown
- Consider the broader context — why is this question being asked? What's the underlying goal?
- Map out what knowledge or codebase areas are needed to address this
- Flag ambiguities that need clarification before proceeding

### 2. Problem Decomposition
- Break the task into core components
- Identify explicit and implicit requirements
- Map constraints and limitations
- Define what a successful outcome looks like

### 3. Multiple Hypotheses
- Generate at least 2-3 possible approaches before committing
- **Keep multiple working hypotheses active** — don't collapse to one prematurely
- Consider unconventional or non-obvious interpretations
- **Look for creative combinations** of different approaches
- Evaluate trade-offs: complexity, performance, maintainability, risk
- Show why certain approaches are more suitable than others

### 4. Natural Discovery Flow
Think like a detective — each realization should lead naturally to the next:
- Start with obvious aspects, then dig deeper
- Notice patterns and connections across the codebase
- Question initial assumptions as understanding develops
- Circle back to earlier ideas with new context
- Build progressively deeper insights
- **Be open to serendipitous insights** — unexpected connections often reveal the best solutions
- Follow interesting tangents, but tie them back to the core issue

### 5. Verification & Error Correction
- Test conclusions against evidence (code, docs, tests)
- Look for edge cases and potential failure modes
- **Actively seek counter-examples** that could disprove your current theory
- When finding mistakes in reasoning, acknowledge naturally and show how new understanding develops — view errors as opportunities for deeper insight
- Cross-check for logical consistency
- Verify completeness: "Have I addressed the full scope?"

### 6. Knowledge Synthesis
- Connect findings into a coherent picture
- Identify key principles or patterns that emerged
- **Create useful abstractions** — turn findings into reusable concepts or guidelines
- Note important implications and downstream effects
- Ensure the synthesis answers the original question

### 7. Recursive Application
- Apply the same careful analysis at both **macro** (system/architecture) and **micro** (function/logic) levels
- Use patterns recognized at one scale to inform analysis at another
- Maintain consistency while allowing for scale-appropriate methods
- Show how detailed analysis supports or challenges broader conclusions

## Additional Resources

For extended guidance, examples, and domain-specific applications, see:
- [SKILL.md](deep-thinking/SKILL.md) - Complete skill definition and protocol details
- [reference.md](deep-thinking/reference.md) - Reference guide with thinking patterns and examples
