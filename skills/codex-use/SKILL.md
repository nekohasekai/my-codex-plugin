---
name: codex-use
description: |-
    Guide to calling OpenAI Codex as a full-featured sub agent
user-invocable: false
---

Codex is very affordable and fast, making it ideal for outsourcing all tasks that don't require design work.

`mcp__plugin_my-codex-plugin_codex__codex`(
    `prompt`: <Input Prompt>
    `cwd`: <Current Directory>
    // Do not fill in other parameters based on your own assumptions
)

It returns a thread ID, allowing you to continue interacting after it completes (like SendMessage):

`mcp__plugin_my-codex-plugin_codex__codex-reply`(
    `threadId`: <Thread ID Returned By mcp__codex__codex>
    `prompt`: <Continued Prompt>
)

Notes:

* Codex has been configured to read CLAUDE.md, so you don't need to add extra commands; simply use it just as you would the Claude Agent.
* Codex has already been configured with unrestricted permissions.

