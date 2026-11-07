# Core pipeline

**Status:** design specification; no complete production runtime is implemented yet.

## Artifact flow

`ProjectBrief → SourceLedger → ClaimLedger → StoryOutline → Script → Character/Environment References → Storyboard → ShotPlan → AssetManifest → EditProject → ReviewReport → DeliveryPackage`

Each stage reads versioned, approved inputs and creates a new version. It must not modify the previous stage in place. Every artifact records its status and upstream versions.

## Minimum object IDs

- `EP###` episode
- `SRC###` source
- `CLM###` claim
- `SC###` scene
- `SH###` shot
- `CHR###` character
- `ENV###` environment
- `AST###` asset
- `APR###` approval

Use stable IDs in filenames and manifests; descriptive titles can change without breaking links.

## First implementation order

1. Episode folder/template generator.
2. Markdown/CSV source and claim ledgers.
3. Deterministic validation for required fields, references, and missing files.
4. Media probe/report using ffprobe.
5. Caption, credit, and archive-manifest checks.
6. Retrieval/drafting agents with explicit schema and human approval states.
7. Orchestrator only after the first pilot proves the handoffs.

## Quality gates

- **Research gate:** source identity and claim references are inspectable.
- **Script gate:** each factual line maps to a claim; uncertain lines are labeled.
- **Character/board gate:** approved canon and source status attached.
- **Asset gate:** provenance, rights, model/checkpoint and review captured.
- **Edit gate:** versions, captions, credits and technical metadata verified.
- **Release gate:** creative lead approves final master and package.

See `docs/PRODUCTION_WORKFLOW.md` and `docs/AUTOMATION_ARCHITECTURE.md` for full procedures.
# Core pipeline

**Status:** design specification; a complete production runtime is not implemented.

## Artifact flow

`ProjectBrief → SourceLedger → ClaimLedger → StoryOutline → Script → Character/Environment References → Storyboard → ShotPlan → AssetManifest → EditProject → ReviewReport → DeliveryPackage`

Each stage reads versioned, approved inputs and creates a new version. Do not modify prior stages in place. Record status and upstream versions.

## Minimum IDs

`EP###` episode, `SRC###` source, `CLM###` claim, `SC###` scene, `SH###` shot, `CHR###` character, `ENV###` environment, `AST###` asset, `APR###` approval.

## Implementation order

1. Episode folder/template generator.
2. Source and claim ledgers.
3. Required-field, ID, reference and missing-file checks.
4. ffprobe report.
5. Caption, credit and archive checks.
6. Retrieval/drafting agents with schemas and approvals.
7. Orchestrator only after pilot handoffs are stable.

See `docs/PRODUCTION_WORKFLOW.md` and `docs/AUTOMATION_ARCHITECTURE.md` for stage gates.
