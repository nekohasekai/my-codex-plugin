---
name: setup-codex
description: Setup codex plugin
disable-model-invocation: true
---

# my-codex-plugin setup

Load the `codex-use` skill and execute `Hello World` to verify that Codex is correctly configured. If not, stop and notify the user.

Then:

Check the `~/.codex/config.toml` file; if the following content is missing, ask the user whether to write it:

```toml
project_doc_fallback_filenames = ["CLAUDE.md"]
```
