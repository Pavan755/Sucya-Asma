# Automation architecture (planned)

**Design only. The repository contains specifications, not a complete autonomous production system.** Build after the pilot process is proven manually.

## Operating model

The user is creative lead and final approver. The director agent coordinates bounded tasks, reads approved documents, proposes artifacts, and records state. Specialist agents return structured drafts with source/asset references. Deterministic scripts validate paths, schemas, IDs, durations, captions, manifests, metadata, and export completeness. No component promotes draft to approved canon or publishes silently.

```text
Books/references → lawful notes + Zotero records → source/claim ledgers
  → research assistant → approved brief → story analyst → script draft
  → human script approval → character/environment canon + director plan
  → human board approval → asset tools → provenance/continuity checks
  → Kdenlive edit → audio/captions → technical QA
  → human final-cut/release approval → master + social package + archive
```

## Automation tiers

### Tier 1 — deterministic helpers

- Create episode folder and README from a template.
- Check required fields and unique episode/scene/shot/claim/asset IDs.
- Validate claim IDs in scripts and methods for planned shots.
- Check file existence, paths, size and manifest consistency.
- Use ffprobe to report duration, resolution, frame rate, audio tracks and codec.
- Check caption timing/language and missing credit fields.
- Produce checksums and archive manifests.

### Tier 2 — retrieval/drafting agents

- Research assistant finds candidate sources and drafts notes with page references; human reviews.
- Story analyst checks scope, causal clarity, pacing, and claim coverage.
- Character/environment agents retrieve approved canon and flag contradictions.
- Director proposes scenes, shots, duration, framing, motion, sound and production method from approved inputs.
- Prompt assistant drafts versioned shot prompts from approved bible/storyboard.
- Editorial assistant drafts social variants from approved material while retaining context and source labels.

Every output is `DRAFT`, declares inputs/versions, provides references, conforms to a schema, and has a checklist.

### Tier 3 — orchestration

After tiers 1–2 work reliably, a director runtime may move artifacts through explicit states, trigger local generation/render jobs, collect results, route failures, and present a review queue. Keep job logs, tool/model versions, cost/compute estimates, retry limits, and cancellation. Human approvals remain required for source framing, thesis, script, character design, storyboard, final cut and release.

## Approval states

`IDEA → RESEARCH → BRIEF_APPROVAL → SCRIPT_DRAFT → SCRIPT_APPROVAL → BOARD_DRAFT → BOARD_APPROVAL → ASSET_PRODUCTION → EDIT_DRAFT → REVIEW → FINAL_APPROVAL → RELEASED → ARCHIVED`

A return state records the reason and earlier artifact to revise. Agent completion is not approval. Record actor, time, version, decision and notes.

## Failure handling

- Missing source: return to research; never invent a citation.
- Conflicting sources: surface disagreement and require editorial choice.
- Unsupported line: flag; block approval until sourced, rewritten or labeled.
- Character drift: reject/regenerate with approved references or request bible revision.
- Generation failure: bounded retry, then stills/graphics or blocked status.
- Broken path: report expected path and ID; never silently overwrite originals.
- Rights uncertainty: block public use until clarified or replaced.
- Render/caption failure: preserve previous approved cut and create a new version.

## Evaluation before scaling

Compare agent drafts to human-approved results: citation correctness, unsupported-claim rate, continuity errors, revision count, time saved, and compute/cost. Start with one episode and few shots. Expand only when automation reduces repetitive work without making fact-checking harder.
