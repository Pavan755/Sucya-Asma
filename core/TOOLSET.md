# Repository toolset and accounts

The canonical tool and storage decision is maintained in [`docs/TOOLSET.md`](../docs/TOOLSET.md). This file will later contain account setup instructions and reproducible environment configuration. Do not commit account emails, credentials, recovery keys, OAuth tokens, API keys, private book files, model weights, or user-specific personal data.

## Planned local configuration

- Project root: configured per machine or Drive workspace, never baked into reusable code.
- Secrets: environment-specific secret store only.
- Software versions: record application and model/checkpoint versions in each production manifest.
- Media paths: stable episode-relative directories with a documented archive copy.
- Colab: mount the project's Drive folder and verify a test write/read before running a notebook.
