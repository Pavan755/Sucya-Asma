# Core architecture

```text
Human creative lead
  ├── approves brief, source framing, script, character canon, board, final edit, release
  └── directs the production coordinator / director
         ├── research assistant → source and claim drafts
         ├── story analyst → outline and script checks
         ├── character intelligence → canon retrieval and continuity flags
         ├── environment intelligence → place, period and prop references
         ├── storyboard/director → scene and shot proposals
         └── production assistant → asset tracking, edit checklist and delivery pack

Deterministic core library: paths, ledgers, schemas, validation, logs, media metadata
Storage: GitHub for text/code; Drive for live structured production; MEGA for additional archive copy
```

Agents exchange structured, versioned drafts and references. The core library validates data and coordinates tools; it does not decide historical truth. The user's approval is a recorded state transition, not a natural-language guess. Provider connectors should be replaceable so one model service does not own the project.

## Separation of concerns

- **Canon and research:** versioned human-reviewed records.
- **Reasoning:** narrow agents that cite input artifact IDs.
- **Execution:** scripts and local/provider tools with logs and bounded retries.
- **Approval:** explicit human decisions and revision notes.
- **Delivery:** editor project, master, captions, credits and provenance.

The architecture is aspirational until implemented. See the stage gates in `docs/AUTOMATION_ARCHITECTURE.md`.
# Core architecture

```text
Human creative lead
  ├─ approves source framing, brief, script, canon, storyboard, final cut, release
  └─ directs production coordinator
       ├─ research assistant → source and claim drafts
       ├─ story analyst → outline/script checks
       ├─ character intelligence → canon retrieval/continuity flags
       ├─ environment intelligence → place/period/prop references
       ├─ director → scene and shot proposals
       └─ production assistant → asset tracking, edit checks, delivery

Deterministic core: paths, ledgers, schemas, validation, logs, media metadata
Storage: GitHub text/code; Drive live production; MEGA archive copy
```

Agents exchange structured, versioned drafts. The core library validates data; it does not decide historical truth. Human approval is an explicit recorded transition. Provider connectors should be replaceable.

Separate canon/research, reasoning, execution, approval, and delivery. This architecture is aspirational until implemented; see `docs/AUTOMATION_ARCHITECTURE.md`.
