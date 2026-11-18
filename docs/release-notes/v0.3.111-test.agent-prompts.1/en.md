## 0.3.111-test.agent-prompts.1 (test)

Test build for the agent system prompt editor. Not an official release.

### Added

- A new “System prompt” editor on the Agents page for ZCode, Claude Code, Claude Desktop, OpenCode, OpenClaw, Hermes, DeepSeek Harness, Oh My Pi, Pi, Grok Build, Copilot CLI, VS Code Copilot, Antigravity CLI, WorkBuddy, and Kimi Code.
- Per-model overrides with replace, prepend, or append modes; replace keeps dynamic runtime context such as working directory, environment, and memory.
- System prompts can also be edited from ZCode’s model catalog and subagent dialogs.

### Fixed

- Custom prompts are applied by a local loopback endpoint instead of writing into strict client configuration files, so ZCode no longer risks discarding its model list.
- With no custom prompt set, agents keep connecting directly to the CPA kernel with no extra forwarding.

### Upgrade notes

- For verification only. Back up the current executable before installing. Keep ECPA running while custom prompts are active.
