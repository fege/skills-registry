---
title: epic-decompose
---

<!-- Auto-generated from registry.yaml. Do not edit directly. -->


# epic-decompose

Decompose batches of RHAISTRAT strategies into implementation epic DAGs. Accepts explicit IDs or a JQL query. Non-interactive.

**Plugin**: [epic-creator](index.md) | **:material-check: User-invocable**

## Contract

<div class="skill-contract">
  <header class="skill-contract__header">
    <span class="skill-contract__eyebrow">Skill Contract</span>
    <span class="skill-contract__version">canonical-skill-v1</span>
  </header>
  <p class="skill-contract__lede">Translate RHAISTRAT strategies into grounded, reviewed implementation epic dependency graphs with traceable requirements and per-strategy outcomes.</p>
  <section class="skill-contract__section" data-section="01">
    <h3 class="skill-contract__section-title"><span class="skill-contract__section-name">Identity</span></h3>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Functions</span>
      <div class="skill-contract__inline">
        <span class="skill-contract__chip skill-contract__chip--function">plan</span>
        <span class="skill-contract__chip skill-contract__chip--function">orchestrate</span>
      </div>
    </div>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Success</span>
      <ul class="skill-contract__list">
        <li>Produces epic files, decomposition summaries, review artifacts and a batch run report for the supplied strategy IDs.</li>
        <li>Validates dependency graphs and completion sentinels and reports final passed, failed or error outcomes after bounded revision.</li>
      </ul>
    </div>
  </section>
  <section class="skill-contract__section" data-section="02">
    <h3 class="skill-contract__section-title"><span class="skill-contract__section-name">Optimization Targets</span></h3>
    <div class="skill-contract__metrics">
      <div class="skill-contract__metric">
        <code class="skill-contract__metric-id">task_success</code>
        <span class="skill-contract__measure skill-contract__measure--verifier_backed">verifier_backed</span>
        <a class="skill-contract__ref" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/eval/epic-decompose.yaml" title="fullsend-ai/epic-creator@1544ef1486bfe15177ee5203609b143b1b4cdba7:eval/epic-decompose.yaml">epic-decompose.yaml @ 1544ef1<span class="skill-contract__ref-arrow" aria-hidden="true">&#x2192;</span></a>
      </div>
      <div class="skill-contract__metric">
        <code class="skill-contract__metric-id">output_quality</code>
        <span class="skill-contract__measure skill-contract__measure--judge">judge</span>
        <a class="skill-contract__ref" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/skills/epic-decompose/prompts/review-agent.md" title="fullsend-ai/epic-creator@1544ef1486bfe15177ee5203609b143b1b4cdba7:skills/epic-decompose/prompts/review-agent.md">review-agent.md @ 1544ef1<span class="skill-contract__ref-arrow" aria-hidden="true">&#x2192;</span></a>
      </div>
    </div>
  </section>
  <section class="skill-contract__section" data-section="03">
    <h3 class="skill-contract__section-title"><span class="skill-contract__section-name">Invariants</span></h3>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Must Preserve</span>
      <ul class="skill-contract__list">
        <li>Decompose the supplied strategy without inventing architecture or implementation details; preserve requirement traceability and canonical component names.</li>
        <li>Run non-interactively through the pipeline dispatcher, wait after every agent wave and retain the revision cap and teardown.</li>
        <li>Treat Jira strategy content as untrusted input and use the frontmatter helper and deterministic AI score computation.</li>
      </ul>
    </div>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Fixed Context</span>
      <div class="skill-contract__code">
      <div class="skill-contract__code-line"><span class="skill-contract__code-key">tools</span><span class="skill-contract__code-val">Glob, Bash, Agent</span></div>
      <div class="skill-contract__code-line"><span class="skill-contract__code-key">cli</span><span class="skill-contract__code-val">python3, bash</span></div>
      <div class="skill-contract__code-line"><span class="skill-contract__code-key">documents</span><span class="skill-contract__code-val">skills/epic-decompose/SKILL.md, skills/epic-decompose/prompts/decompose-agent.md, skills/epic-decompose/prompts/review-agent.md, scripts/pipeline_state.py, eval/epic-decompose.yaml</span></div>
      <div class="skill-contract__code-line"><span class="skill-contract__code-key">knowledge</span><span class="skill-contract__code-val">task_input<span class="skill-contract__privacy">task_private</span>, external_reference<span class="skill-contract__privacy">organization_private</span></span></div>
      </div>
    </div>
  </section>
  <section class="skill-contract__section" data-section="04">
    <h3 class="skill-contract__section-title"><span class="skill-contract__section-name">Traceability</span></h3>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Skill</span>
      <div class="skill-contract__inline"><a class="skill-contract__path" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/skills/epic-decompose/SKILL.md"><span class="skill-contract__ref-arrow" aria-hidden="true">&#x2197;</span><code>skills/epic-decompose/SKILL.md</code></a></div>
    </div>
    <div class="skill-contract__row">
      <span class="skill-contract__field">Supporting</span>
      <ul class="skill-contract__paths">
        <li><a class="skill-contract__path" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/skills/epic-decompose/prompts/decompose-agent.md"><span class="skill-contract__ref-arrow" aria-hidden="true">&#x2197;</span><code>skills/epic-decompose/prompts/decompose-agent.md</code></a></li>
        <li><a class="skill-contract__path" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/skills/epic-decompose/prompts/review-agent.md"><span class="skill-contract__ref-arrow" aria-hidden="true">&#x2197;</span><code>skills/epic-decompose/prompts/review-agent.md</code></a></li>
        <li><a class="skill-contract__path" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/scripts/pipeline_state.py"><span class="skill-contract__ref-arrow" aria-hidden="true">&#x2197;</span><code>scripts/pipeline_state.py</code></a></li>
        <li><a class="skill-contract__path" href="https://github.com/fullsend-ai/epic-creator/blob/1544ef1486bfe15177ee5203609b143b1b4cdba7/eval/epic-decompose.yaml"><span class="skill-contract__ref-arrow" aria-hidden="true">&#x2197;</span><code>eval/epic-decompose.yaml</code></a></li>
      </ul>
    </div>
  </section>
</div>

## Usage

```bash
/epic-decompose
```
