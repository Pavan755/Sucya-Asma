# Cost and continuity policy

**Default budget: zero.** The project must remain useful without a subscription, paid API, cloud GPU rental, or paid storage. No production step may assume that a free quota will always be available.

## Allowed baseline

- Use free/open-source desktop tools for research management, editing, audio, and media conversion.
- Keep source notes, scripts, shot plans, and project manifests in GitHub and local storage.
- Use the separate Google account's included Drive space for active documents and small working files, after checking its actual quota.
- Use MEGA only as an optional second copy if the free account's current quota and transfer terms work for the project.
- Use Zotero locally without paid attachment sync; keep a second copy of important PDFs in an authorized local or project storage location.
- Treat hosted GPU access as optional and temporary. Colab/free compute may change availability, reset sessions, or impose limits; it is not a production dependency.

## No-charge guardrails

1. Do not enter payment details, start a trial, subscribe, enable pay-as-you-go, or create paid API keys for this project.
2. Before any service is used, verify whether the action can incur charges and whether billing is enabled. If unclear, stop and choose a local or no-charge fallback.
3. Record the tool/model version, license, source, and storage location. Do not upload copyrighted books or private source files to hosted services without confirmed rights and a privacy review.
4. Check remaining storage before importing books, image packs, checkpoints, or video exports. Keep large media out of Git.
5. Review each proposed production expense in writing before it is incurred. The default decision is to defer it.

## Continuity plan if a service stops working

- **Drive unavailable or full:** continue from the local project folder and GitHub for documents; archive exported media locally and to any verified secondary storage. Do not upgrade automatically.
- **MEGA unavailable or quota/transfer restricted:** keep the working copy local; use the GitHub repository only for suitable text/code, and identify another no-cost destination before uploading large media.
- **Colab or hosted GPU unavailable:** continue with approved stills, camera moves, typography, compositing, and simple Blender/Kdenlive motion. The story and episode plan remain valid.
- **ComfyUI too slow or memory-limited:** use hand-built/reference-approved artwork, lower-resolution drafts, or non-generative motion graphics. Do not buy compute to rescue a single shot.
- **Any tool or service changes its terms or begins requiring payment:** pause that dependency, preserve local files, and switch to an open format or documented fallback.

## Production gate

Before a pilot enters production, confirm a complete local backup, source and asset rights, a reproducible edit/export path, current storage headroom, and a no-cost fallback for every cloud-dependent step. If any gate fails, stay in pre-production and revise the workflow.

## Costs that cannot be promised away

Software can be free while internet access, electricity, storage hardware, suitable GPU hardware, commercial licenses, and optional cloud compute still have real costs. The zero-budget plan avoids requiring these purchases; it cannot guarantee a full AI-generated video workflow at commercial scale on current free quotas or this laptop's 6 GB GPU.
