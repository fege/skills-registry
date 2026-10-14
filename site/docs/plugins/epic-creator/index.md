---
title: epic-creator
---

<!-- Auto-generated from registry.yaml. Do not edit directly. -->


# epic-creator

Decompose RHAISTRAT strategies into implementation epic dependency graphs with adversarial review, bounded revision and AI implementability scoring. Accepts strategy IDs or a JQL query for non-interactive batch processing.

!!! info "Plugin Details"

    - **Version**: 1.0.0
    - **Author**: Jessica Forrester
    - **Category**: [Product Planning](../../categories/planning.md)
    - **Repository**: [fullsend-ai/epic-creator](https://github.com/fullsend-ai/epic-creator)
    - **Tags**: <span class="tag-pill">epic</span> <span class="tag-pill">strategy</span> <span class="tag-pill">jira</span> <span class="tag-pill">decomposition</span> <span class="tag-pill">review</span>

## Skills

| Skill | Description | Invocable |
|-------|-------------|-----------|
| [`/epic-decompose`](epic-decompose.md) | Decompose batches of RHAISTRAT strategies into implementation epic DAGs. Accepts explicit IDs or a JQL query. Non-interactive. | :material-check: |

## Installation

**Claude Code**

```bash
/plugin install epic-creator@opendatahub-skills
```

**OpenAI Codex** — add the marketplace, then enable `epic-creator` from the `/plugins` browser:

```bash
codex plugin marketplace add opendatahub-io/skills-registry
```
