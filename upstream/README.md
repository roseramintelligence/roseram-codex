# Roseram with Codex CLI

Install the [official Codex CLI](https://github.com/openai/codex). Use [roseram.toml](roseram.toml) as the contents of `config.toml` in a separate Codex configuration directory so your existing Codex settings are preserved. Set `CODEX_HOME` to that directory and `ROSERAM_API_KEY` to your Roseram developer key in the shell where you launch `codex`. Launch from a project folder.

The profile selects the Roseram model and HTTPS Responses endpoint. It starts with read-only workspace access and asks before approval-gated actions. The key is read from the environment. The configuration contains no credential.

Start with a read-only task asking it to summarize one file in a test repository. Treat full request compatibility, usage metering and the Codex desktop app as separate verification work. The Roseram response adapter accepts a subset of the Responses API and may reject unsupported parameters.

Upstream source and license: [OpenAI Codex CLI, Apache-2.0](https://github.com/openai/codex/blob/main/LICENSE).
