# Production roles and handoffs

These are responsibilities, not a requirement to hire a large crew. At the beginning, Pavan may hold several human roles and AI agents may prepare drafts or checklists. The same person can direct the whole film; separating the jobs makes omissions visible and gives automation clear, bounded tasks.

| Role | Main responsibility | Required output | Safe automation role | Human approval |
|---|---|---|---|---|
| **Creative lead / series creator** | Defines purpose, audience, tone, cultural boundaries, and series canon. | Series bible, creative brief, approved character/environment versions. | Agent can surface canon conflicts and collect decisions. | Final creative and cultural direction. |
| **Producer / production coordinator** | Keeps scope, schedule, dependencies, files, rights, and review gates organized. | Episode status, task list, asset register, release checklist. | Strong candidate for folder creation, reminders, manifests, status summaries. | Scope, resource, schedule, and go/no-go decisions. |
| **Researcher / historical editor** | Finds and evaluates sources; builds sourced claims and uncertainty notes. | Zotero records, source ledger, claim ledger, research brief. | Candidate-source discovery, metadata extraction, citation cross-check drafts. | Every central claim, source framing, and disputed interpretation. |
| **Cultural/subject reviewer** | Checks respectful treatment, tradition variation, and potential harm. | Review notes, terminology guidance, unresolved concerns. | Agent can prepare questions and detect flagged terms. | Human specialist/community review where appropriate. |
| **Story editor** | Turns research into a focused question, thesis, outline, and coherent dramatic arc. | Beat sheet and revision notes linked to claim IDs. | Draft alternatives and pacing/coverage analysis. | Thesis, scope, and final story structure. |
| **Scriptwriter / narrator** | Writes understandable dialogue and narration for the intended audience and runtime. | Versioned script with claim IDs, pronunciation notes, and timing. | First drafts, timing estimates, simplification options. | Every factual line, interpretation, and final wording. |
| **Director** | Converts approved script into scene intention, emotional progression, performances, and shot plan. | Director's breakdown, scene objectives, storyboard/shot list. | Propose shot coverage, continuity reminders, and schedule. | Storyboard and performance direction. |
| **Art director / production designer** | Defines the visual language, palette, symbols, props, locations, and continuity. | Style guide, character/environment packs, source labels. | Reference collection and checklist-based continuity flags. | Final design and culturally meaningful visual choices. |
| **Character designer** | Builds repeatable character identity and reference sheets from the bible. | Turnaround, expression, costume/prop, scale sheets. | Generate candidate sketches and compare against approved traits. | Character identity, costume, symbolism, and version lock. |
| **Environment designer** | Builds historically/traditionally grounded places, layouts, and props. | Location bible, maps/layouts, time/period assumptions. | Organize references and flag inconsistent details. | Geography, period interpretation, and visual claims. |
| **DOP / cinematographer** | Plans framing, lens feel, camera movement, light, composition, and visual continuity. | Shot-by-shot camera plan: size, angle, movement, light, focal attention, transition. | Draft coverage options and convert approved terms into shot prompts. | Final camera language where it shapes meaning or evidence. |
| **Storyboard / animatic artist** | Turns the shot plan into timed visual panels and tests clarity before full production. | Board with shot IDs, timing, narration, and rough transitions. | Generate rough panels, timing sheets, animatic assembly. | Approve visual sequence and timing before asset production. |
| **Animation / AI asset operator** | Creates, cleans, versions, and logs each shot or still. | Approved assets, prompt/model record, provenance and continuity notes. | Queue jobs, name outputs, check dimensions and missing files. | Select usable takes; reject misleading or culturally inaccurate outputs. |
| **Voice / sound editor** | Records/cleans narration, checks pronunciation, and balances effects/music. | Separate tracks, transcript, mix notes, license/credit data. | Transcription draft, silence/peak checks, file organization. | Voice performance, pronunciation, music tone, and final mix. |
| **Editor** | Shapes picture and sound into a clear, paced film. | Kdenlive project, rough cut, review renders, approved master. | Media relinking checks, proxy creation, technical reports. | Story rhythm, transitions, final cut. |
| **Quality reviewer** | Checks factual accuracy, cultural portrayal, continuity, captions, audio, and delivery specs. | Timecoded review report and resolved-issue log. | Technical checks, ID/claim coverage, caption timing, metadata. | Accept/reject interpretive, factual, and visual concerns. |
| **Release / social producer** | Adapts approved work for platforms, schedules release, and preserves context. | Master, captions, thumbnail, description, vertical/short cuts, source/credit note, archive package. | Create drafts/cutdown plans from approved segments and verify package completeness. | Final copy, platform choices, upload, and release timing. |

## DOP / camera plan fields

Each shot record should identify: shot ID; scene/beat; narration/claim IDs; shot size; angle; subject placement; camera motion; lens/depth impression; light and color; action; duration; transition; focus of attention; evidence/reconstruction label; continuity constraints; asset method; and status. Use plain language first; translate to model-specific prompts only after the user approves the board. Camera language should not imply a witness or documentary recording when the scene is a reconstruction.

## Handoff pattern

Every handoff names the upstream approved version, the receiving role, the requested output, the deadline/status, unresolved questions, and approval needed. Drafts carry `DRAFT`; a role cannot self-approve a gate assigned to the creative lead. If a handoff fails, route it to the earliest responsible phase (for example, missing evidence returns to research, character drift returns to design, unclear pacing returns to story edit).

## Small pilot crew

For the first short episode, keep it simple:

1. **Pavan as creative lead, producer, director, editor, and final reviewer.**
2. **Research assistant workflow** organizes sources and claim references; Pavan approves the evidence and framing.
3. **Character/art workflow** completes one static approved character pack before motion.
4. **Director/DOP/storyboard workflow** creates a timed board from the approved script.
5. **Production workflow** assembles a still-led cut in Kdenlive with narration, maps/graphics, captions, and source/rights notes.
6. **Optional subject/cultural review** is sought where the story or representation requires expertise beyond the project lead.

After the pilot, measure where time was spent. Automate the repetitive handoffs and checks that actually caused delays. Keep final meaning, accuracy, canon, and release under human control.
