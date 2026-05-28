---
title: spike-executor
---

<!-- Auto-generated from registry.yaml. Do not edit directly. -->


# spike-executor

Execute RHOAI SPIKE investigations with human-in-the-loop approval gates. 9-step lifecycle: intake, plan, Jira sync, AI research enrichment with hallucination detection, pytest test suites on OpenShift, rubric-based scoring with security gates, and RFE generation. Supports both runtime and protocol library evaluations.

!!! info "Plugin Details"

    - **Version**: 0.2.0
    - **Author**: IKRedHat
    - **License**: Apache-2.0
    - **Category**: [Product Planning](../../categories/planning.md)
    - **Repository**: [IKRedHat/SPIKE-executor](https://github.com/IKRedHat/SPIKE-executor)
    - **Tags**: <span class="tag-pill">spike</span> <span class="tag-pill">evaluation</span> <span class="tag-pill">jira</span> <span class="tag-pill">research</span> <span class="tag-pill">scoring</span> <span class="tag-pill">rfe</span> <span class="tag-pill">openshift</span> <span class="tag-pill">rhoai</span> <span class="tag-pill">feasibility</span>

## Dependencies

- [`rfe-creator`](../rfe-creator/index.md)

## Skills

| Skill | Description | Invocable |
|-------|-------------|-----------|
| [`/SPIKE-executor`](SPIKE-executor.md) | Execute RHOAI SPIKE investigations with human-in-the-loop approval gates | :material-check: |

## Installation

```bash
/plugin install spike-executor@opendatahub-skills
```
