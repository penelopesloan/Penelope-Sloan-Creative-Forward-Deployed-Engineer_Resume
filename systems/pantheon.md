# PSC Pantheon

A 40-agent ecosystem built in Claude Code, running strategy, research, content production and client delivery as coordinated specialists rather than one general-purpose assistant.

## The problem

A solo consultancy delivering across brand strategy, design, research and client operations hits a ceiling fast. Context switching is the tax. A single general assistant produces generic output because it holds no persistent role, standard or voice.

## The approach

Each agent owns one job, with its own scope, standards and voice. An orchestration layer routes work between them. A command centre surfaces state so the system is observable rather than a black box.

Critically, one agent exists purely to say no: a tone and quality gate that work passes through before it reaches a client. **The innovation is not generation, it is QA.**

## Architecture

- **Agent layer.** Specialist agents, each scoped to a single function with its own instructions and quality bar
- **Orchestration layer.** Routes tasks, sequences multi-agent work, holds shared context
- **Command centre.** Operational dashboard surfacing agent state and work in progress
- **Notion integration.** Persistent project and client data, readable and writable by agents

## Stack

Claude Code · Claude API · Notion API · Markdown-based agent definitions

## Design decisions worth noting

**Roles, not prompts.** Prompting is not a system. Persistent roles with defined scope produce consistent output across sessions; ad hoc prompting does not.

**Separate brands never bleed.** Multiple distinct brand voices run through the same ecosystem without contaminating each other, because the quality gate is applied per brand rather than globally.

**Constraints are the product.** The brand rules fed into the system are what stop output looking like everyone else's. The model is the multiplier, the constraints are the differentiator.

---

<!-- TO ADD: agent list or category breakdown, a sanitised example of an agent definition,
     and a screenshot of the command centre. Keep client data out. -->
