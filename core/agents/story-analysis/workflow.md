# Story Analysis Agent Workflow

## Objective

Transform a verified mythology source into a structured production blueprint that can be used by every downstream Sucya-Asma production agent.

The workflow prioritizes factual integrity, chronological consistency, and reusable structured knowledge.

---

# Stage 1 — Source Validation


cat > core/agents/story-analysis/workflow.md << 'EOF'
# Story Analysis Agent Workflow

## Objective

Transform a verified mythology source into a structured production blueprint that can be used by every downstream Sucya-Asma production agent.

The workflow prioritizes factual integrity, chronological consistency, and reusable structured knowledge.

---

# Stage 1 — Source Validation

Input:

- Verified source document
- Source verification report

Tasks:

- Confirm source authenticity
- Confirm chronology
- Confirm translation/version
- Detect uncertainty markers
- Reject unverified sources

Output:

Verified Story Source

---

# Stage 2 — Story Understanding

Tasks:

- Read the complete story
- Understand narrative purpose
- Detect beginning, middle, climax and conclusion
- Identify major events
- Identify minor events
- Detect emotional progression

Output:

Narrative Structure

---

# Stage 3 — Character Extraction

Tasks:

Identify every character.

For each character extract:

- Name
- Role
- Importance
- First appearance
- Last appearance
- Relationships
- Personality
- Emotional state
- Physical description
- Divine attributes
- Future Character Bible updates

Output:

Character Database Updates

---

# Stage 4 — Environment Extraction

Detect:

- Forests
- Mountains
- Oceans
- Kingdoms
- Temples
- Architecture
- Time of day
- Weather
- Atmosphere
- Sacred elements

Output:

Environment Database Updates

---

# Stage 5 — Scene Segmentation

Divide the story into cinematic scenes.

Each scene should contain:

- Beginning
- Ending
- Characters
- Environment
- Emotional objective
- Narrative objective

Output:

Scene List

---

# Stage 6 — Emotional Analysis

For every scene identify:

- Primary emotion
- Secondary emotion
- Emotional intensity
- Audience expectation
- Emotional transition

Output:

Emotional Arc

---

# Stage 7 — Cinematic Opportunity Detection

Classify scenes into:

- Documentary Scene
- Motion Scene
- Dialogue Scene
- LTX Handcrafted Scene
- Reflection Scene
- Transition Scene

Output:

Production Recommendations

---

# Stage 8 — Complexity Analysis

Estimate:

- Image complexity
- Motion complexity
- Character count
- Background complexity
- GPU cost
- Production time

Output:

Production Estimates

---

# Stage 9 — Quality Validation

Verify:

- Chronology preserved
- Characters consistent
- No hallucinated mythology
- Respectful adaptation
- Source traceability
- Documentary clarity
- Child-friendly language

Output:

Approved Story Analysis

---

# Final Deliverables

The Story Analysis Agent exports:

- Story Report
- Character Updates
- Environment Updates
- Scene Breakdown
- Emotional Arc
- Production Recommendations
- Complexity Report
- Episode Suggestions

These outputs become the inputs for every downstream production agent.
