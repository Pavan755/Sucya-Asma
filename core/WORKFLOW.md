# Core workflow

1. Read the current project/episode state and identify the next approved gate.
2. Validate required source artifacts and paths before running work.
3. Produce a new, versioned draft from only the declared inputs.
4. Record tool/model version, inputs, output IDs and any error or uncertainty.
5. Run deterministic checks and attach a concise report.
6. Present the draft to the human approver; do not mark it approved yourself.
7. On revision, retain the prior version and log what changed.

## Notebook-to-library loop

In Colab: explain the objective in Markdown; write small commented code cells; save test outputs explicitly to the episode folder; verify files and output contents. Once logic is stable, move it to a reusable module under `core/`, add an example and an appropriate check, then import that module in future notebooks. Colab temporary storage is scratch space only.

## Failure behavior

Fail visibly with the episode ID, artifact ID, expected path and corrective action. Never fabricate missing source data, silently skip a broken media file, or overwrite an approved asset. See `docs/AUTOMATION_ARCHITECTURE.md`.
# Core workflow

1. Read project/episode state and identify the next gate.
2. Validate required inputs and paths before work.
3. Produce a new versioned draft from declared inputs.
4. Record tool/model version, input/output IDs, and errors or uncertainty.
5. Run deterministic checks and attach a concise report.
6. Present the draft to a human approver; agents do not approve their own work.
7. Retain earlier versions and log revisions.

## Notebook-to-library loop

In Colab, explain the objective in Markdown, write small commented code cells, save test outputs explicitly to the episode folder, and verify the results. Move stable logic to a reusable `core/` module with an example and an appropriate check. Colab temporary storage is scratch space only.

## Failure behavior

Report episode/artifact ID, expected path, and corrective action. Never fabricate source data, silently skip broken media, or overwrite approved assets. See `docs/AUTOMATION_ARCHITECTURE.md`.
