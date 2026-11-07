# Decision log

Record durable project decisions here. Change a decision by adding a dated entry; do not silently rewrite history.

## 2026-11-07 — Use the existing repository as the canonical project

- **Decision:** retain `Pavan755/Sucya-Asma` as the source repository and work from a separate local clone at `RESUMES/Sucya-Asma-Project`.
- **Reason:** it already contains the director/agent structure, Rama and Hanuman bibles, templates, and a pilot story.
- **Follow-up:** keep large assets/books outside Git; remote publication of changes has not yet been done.

## 2026-11-07 — Treat the current creative scope as a Ramayana-inspired animated series

- **Decision:** use existing repo materials as the starting series; do not assume that the earlier phrase “history video” means all Ramayana-associated stories are established historical events.
- **Reason:** the repo includes epic characters and a pilot already labeled as a traditional narrative.
- **Follow-up:** add citations and clearly label text, history, living tradition, interpretation, and dramatization.

## 2026-11-07 — Google Drive for active workspace; MEGA for secondary archive

- **Decision:** recommend the separate Gmail-linked Drive for Colab and active structured work; MEGA for a second copy of approved large files, after verifying account quotas and transfer limits.
- **Reason:** Colab works naturally with Drive, while MEGA offers more free space for larger files. Avoid two competing live copies.
- **Follow-up:** accounts are not connected; verify actual quotas and recovery settings before storing project data.

## 2026-11-07 — Start with a still-led pilot and automate proven stages

- **Decision:** use Zotero, Kdenlive, Audacity, FFmpeg, GitHub and Colab first; add ComfyUI/LTX after hardware and model terms are checked.
- **Reason:** research, character consistency, editing and delivery can be validated without waiting on expensive/slow video generation.
- **Follow-up:** inspect hardware and install/verify the minimal toolset; no installations were performed in this setup step.

## 2026-11-07 — Defer local LTX video generation on the current laptop

- **Decision:** do not make local LTX generation a prerequisite for the pilot.
- **Evidence:** local check found an RTX 3050 Laptop GPU with 6 GB VRAM. The current LTX Desktop repository lists 24 GB VRAM for Windows local generation and a 9 GiB lower compatibility check for fp8-capable GPUs; [current requirements](https://github.com/Lightricks/LTX-Desktop). The LTX-2.5 quick start describes roughly 66 GiB for its listed set of model components; [official inference repository](https://github.com/Lightricks/LTX-2).
- **Reason:** the available GPU is below the current generation floor. The pilot can proceed with stills, maps, motion graphics and conventional editing; revisit hosted/borrowed GPU options only with cost and privacy in view.
- **Follow-up:** system RAM was not available to the local check; confirm it before any later image-generation test.

## Open decisions

- Target audience, age range, language(s), voice and subtitles.
- First pilot runtime, release goal and final story selection.
- Animation approach (2D, illustrated motion, 3D, mixed) based on references and hardware.
- Actual Drive and MEGA quotas, directory names, backup cadence, and local media cache.
- Whether the current Codex app can register the cloned repository as a separately named sidebar project.
