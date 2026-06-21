# SAPE Director Decision Engine

Version: 1.0

Status: Draft

---

# Purpose

The Decision Engine is responsible for making operational decisions throughout the production pipeline.

It does not generate creative content.

Instead, it evaluates system state, production quality, available resources, human approvals, and provider capabilities to determine the next action.

---

# Decision Philosophy

The Director never guesses.

Every decision is based on:

- Current Episode State
- Incoming Events
- System Rules
- Quality Metrics
- Human Approvals
- Provider Availability
- Production Policies

---

# Decision Categories

## Scheduling Decisions

Determine:

- Which task executes next
- Parallel vs sequential execution
- Task priority
- Queue ordering

---

## Provider Decisions

Determine:

- Which provider should execute the task
- Whether a free provider is available
- Whether a fallback provider is required
- Whether execution should wait

---

## Quality Decisions

Determine:

- Pass
- Retry
- Manual Review
- Reject

---

## Approval Decisions

Determine:

- Continue automatically
- Pause for approval
- Escalate to reviewer

---

## Recovery Decisions

Determine:

- Retry same provider
- Switch provider
- Roll back stage
- Cancel production

---

# Decision Inputs

The Decision Engine evaluates:

- Episode State
- Production Events
- Agent Results
- Validation Reports
- QA Scores
- Provider Registry
- Production Policies

---

# Decision Outputs

The Decision Engine may issue:

- ExecuteTask
- RetryTask
- SwitchProvider
- Wait
- PausePipeline
- ResumePipeline
- RequestApproval
- CancelProduction
- CompleteEpisode

---

# Example Workflow

Image Generation completed

↓

Quality Score = 92

↓

Approval Required?

↓

No

↓

Continue to Motion Generation

---

Example

Image Generation completed

↓

Quality Score = 61

↓

Retry allowed?

↓

Yes

↓

Retry using alternate provider

---

Example

Retry Count = 3

↓

Still Failed

↓

Request Human Review

---

# Decision Rules

Rule 1

Never skip mandatory approvals.

---

Rule 2

Never publish without passing QA.

---

Rule 3

Prefer free providers when production quality requirements are satisfied.

---

Rule 4

Switch providers automatically when recoverable failures occur.

---

Rule 5

Every decision must be logged.

---

# Long-Term Intelligence

Future versions of the Decision Engine may learn from:

- Viewer retention
- Production speed
- QA history
- Human corrections
- Provider reliability
- Cost efficiency

The objective is continuous operational improvement without modifying verified source material.

---

