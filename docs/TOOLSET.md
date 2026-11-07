# Toolset and storage choices

**Decision status:** recommended baseline; no account has been connected and no software installation has been verified.

## Current computer snapshot

Checked locally on 7 November 2026: NVIDIA GeForce RTX 3050 Laptop GPU, 6 GB VRAM; about 235 GB free on C:. System RAM could not be read in this environment. The current official LTX Desktop page lists 24 GB VRAM as the Windows local-generation requirement (32 GB recommended) and says its lower compatibility check is 9 GiB VRAM on fp8-capable Windows GPUs; it also recommends at least 100 GB free disk. This GPU is below the local-generation floor. Do not plan local LTX video generation on this machine. [LTX Desktop system requirements](https://github.com/Lightricks/LTX-Desktop)

This does not prevent research, editing, audio work, simple graphics, or still-led animation. Local ComfyUI image generation may be possible only with a modest, memory-aware image checkpoint and careful settings; test one small workflow after checking exact model requirements. For video-model experiments, use a rented/borrowed compatible GPU or a genuinely free hosted session if available, and treat availability, queue time, privacy, and transfer limits as constraints. A hosted API may charge even when model code is open source.

## Storage decision

Use the separate Gmail account and its Google Drive as the **active project workspace**, because the planned learning/build environment is Google Colab and Drive is the straightforward location for notebooks, structured documents, small research files, and automation outputs. Google accounts normally include up to 15 GB shared among Gmail, Drive, and Photos; confirm the actual quota on the new account. [Google storage explanation](https://support.google.com/drive/answer/9312312?hl=en)

Use **MEGA as the secondary media/archive copy** for large approved exports and project backups when its current free allowance is available. MEGA commonly offers a 20 GB free account, but transfer limits and plan details affect practical use; confirm the quota shown in the account. [MEGA plans](https://mega.io/pricing)

Use **Proton Drive only if privacy is the priority for a particular source collection**; its listed free plan is 5 GB, which makes it a poor primary home for video work. [Proton Drive plans](https://proton.me/drive/pricing)

### Why Drive is primary and MEGA is backup

Drive fits Colab notebooks and structured project work. MEGA gives more initial free space for media, but is less convenient as Colab's live working filesystem and can impose transfer limits. This combines workflow fit with additional archive space without assuming either free quota can hold an unlimited video library.

### File placement rules

- **GitHub:** code, Markdown documentation, templates, small manifests, prompt text, decision records. Never commit books, credentials, large model files, raw video, or private data.
- **Google Drive:** live episode folder, notebooks, claim/source ledgers, scripts, storyboards, small assets, review materials, project manifests.
- **MEGA:** second copy of approved masters, lawful large source files, and periodic archive bundles. Keep folder names and IDs aligned with Drive; do not create two competing live copies.
- **Zotero:** bibliographic metadata, citations, notes, and reading status. Zotero software is free; its own online attachment sync is 300 MB free, so do not assume unlimited PDF storage. Keep larger attachments under stable source IDs in Drive/MEGA. [Zotero storage](https://www.zotero.org/storage)
- **Local computer:** active cache, proxies, model checkpoints, and scratch renders where practical. Back up final project and manifests to cloud storage.

Never store API keys, passwords, recovery keys, or account credentials in GitHub, notebooks, prompts, or shared folders.

## Free/open-source production stack

| Stage | Tool | Sucya-Asma use | Notes |
|---|---|---|---|
| Bibliography | Zotero | Books/articles, citations, notes, source status. | Free app; 300 MB Zotero attachment sync. |
| Notebook learning | Google Colab | Learn/prototype Python, access Drive, verify files. | Free compute is limited and availability changes; save outputs to Drive. |
| Version control | GitHub | Version documentation, code, prompts, and decisions. | Keep large media elsewhere. |
| Image/video generation | ComfyUI + LTX Desktop/model | Local workflows for concept images and selected short clips. | Hardware and checkpoint terms determine feasibility. Hosted/API options may cost. |
| Alternative video model | Wan2.2 through a compatible local workflow | Compare motion quality for selected shots. | Official repo says model assets use Apache-2.0; verify exact checkpoint and requirements. |
| Editing | Kdenlive | Assemble episodes, titles, maps, subtitles, social cuts. | Save project with stable relative media paths. |
| Audio | Audacity | Clean narration, inspect waveforms, prepare mixes. | Music/effects still need rights records. |
| Media tools | FFmpeg / ffprobe | Convert, inspect metadata, extract audio, thumbnails, technical checks. | Build configuration can affect FFmpeg licensing. |
| Optional 3D | Blender | Maps, camera moves, props, environments, simple controlled animation. | Add when a shot benefits from it. |

### Install and verify sequence

Install from official project sites or official releases. Start with Zotero, Kdenlive, Audacity, and FFmpeg; these support a still-led pilot. Add Blender only if storyboards identify a need. ComfyUI is a later optional experiment for small still models. Defer local LTX generation until using hardware that meets its current requirements; an API/hosted route may incur costs. Record versions and install locations in the project tool log.

## Model and asset rights

Application license, source-code license, model/checkpoint license, data terms, input asset rights, and generated-output terms are separate. Record exact versions and review terms before public distribution or monetization. For books, preserve citations and lawful notes; do not ingest or redistribute copyrighted books wholesale without rights. For archival images, check the institution's rights statement and exact asset. For music, retain license and attribution evidence. Generated historical imagery is illustration, not proof.

## Official references

- [Google account storage](https://support.google.com/drive/answer/9312312?hl=en)
- [MEGA plan page](https://mega.io/pricing)
- [Proton Drive free plan](https://proton.me/drive/pricing)
- [Zotero storage limits](https://www.zotero.org/storage)
- [LTX Desktop](https://github.com/Lightricks/LTX-Desktop) and [LTX models](https://github.com/Lightricks/LTX-2)
- [ComfyUI license](https://github.com/Comfy-Org/ComfyUI/blob/master/LICENSE)
- [Wan2.2 official repository](https://github.com/Wan-Video/Wan2.2)
- [Kdenlive](https://kdenlive.org/), [Audacity](https://www.audacityteam.org/), [FFmpeg](https://ffmpeg.org/), [Blender](https://www.blender.org/)
