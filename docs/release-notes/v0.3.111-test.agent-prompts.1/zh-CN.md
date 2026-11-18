## 0.3.111-test.agent-prompts.1（测试版）

这是「智能体系统提示词编辑」的测试构建，不是正式版。

### 新增

- 智能体配置页新增「系统提示词设置」，可直接查看并修改 ZCode、Claude Code、Claude Desktop、OpenCode、OpenClaw、Hermes、DeepSeek Harness、Oh My Pi、Pi、Grok Build、Copilot CLI、VS Code Copilot、Antigravity CLI、WorkBuddy、Kimi Code 的系统提示词。
- 支持按模型单独覆盖系统提示词，并可选择替换、前置追加或末尾追加；替换时默认保留工作目录、环境信息和记忆等动态上下文。
- ZCode 的模型列表与子智能体设置中也可直接编辑系统提示词。

### 修复

- 自定义提示词通过本地回环端点改写请求，不写入客户端严格配置文件，避免 ZCode 清空模型列表。
- 未设置自定义提示词时不启用改写端点，仍直连 CPA 内核。

### 升级建议

- 仅用于验证；安装前备份现有程序。自定义提示词生效期间请保持 ECPA 运行。
