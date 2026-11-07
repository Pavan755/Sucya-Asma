# Core library

Reusable production code will live here in Python modules after the workflow is proven in notebooks. The core library should be small, testable, independent of a particular AI provider, and safe to run more than once.

Planned responsibilities:

- `paths.py`: explicit project paths and safe path construction.
- `filesystem.py`: directory creation, file discovery, copy/manifest helpers; never overwrite originals silently.
- `validator.py`: required-field, identifier, reference and asset checks.
- `logger.py`: readable structured run history without secrets.
- `sources.py`: source/claim ledger parsing and cross-reference validation.
- `media.py`: ffprobe metadata collection and export checks.

Learn and prototype in `06_Notebooks/` in the Drive workspace; export stable code into the repository `core/` package. Use relative/configured paths, not hard-coded machine-specific paths. Keep API keys out of notebooks and source control. Add code only when a repeated workflow justifies it.

**Current state:** planning documentation only. A file name in this plan does not imply that the module exists.
# Core library (planned)

Reusable production code will live here in Python modules after the workflow is proven in notebooks. Keep the core small, testable, provider-independent, and safe to run more than once.

Planned responsibilities:

- `paths.py`: configured project paths and safe path construction.
- `filesystem.py`: folder creation, discovery, copy and manifest helpers; never overwrite originals silently.
- `validator.py`: required fields, IDs, references and asset checks.
- `logger.py`: readable run history without secrets.
- `sources.py`: source/claim ledger parsing and cross-reference checks.
- `media.py`: ffprobe metadata collection and export checks.

Prototype in Colab under the Drive workspace; export stable logic into this repository. Use configured/relative paths, not machine-specific paths. Keep API keys out of notebooks and version control.

**Current state:** design documentation only. A planned module name does not mean that module exists.
