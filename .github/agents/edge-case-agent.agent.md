---
name: Edge Case Agent
description: Agent testing various edge cases in configuration — conflicting properties, mixed tool formats, and special characters
target: vscode
model: o3-mini
tools: ["read", "Edit", "SEARCH", "github/get_file_contents", "playwright/*", "nonexistent-tool"]
user-invocable: true
disable-model-invocation: true
infer: true
metadata:
  test-type: edge-case
  unicode-tag: テスト
  emoji-tag: 🤖
---

# Edge Case Agent — Testing Boundaries

This agent tests several edge cases simultaneously:

1. **Conflicting properties**: Both `infer: true` and `disable-model-invocation: true` are set. Per GitHub docs, `disable-model-invocation` takes precedence → agent should NOT be auto-invoked.

2. **Case-insensitive tools**: Mixed case tool names (`Edit`, `SEARCH`) should be recognized.

3. **Server-specific tool**: `github/get_file_contents` enables one specific GitHub MCP tool.

4. **Server wildcard**: `playwright/*` enables all playwright tools.

5. **Unrecognized tool**: `nonexistent-tool` should be silently ignored.

6. **Unicode metadata**: Tags contain Japanese characters and emoji.

7. **Target = vscode**: Agent targets VS Code only (not github-copilot).

8. **Retired property**: `infer` is retired but still present — should be overridden by `disable-model-invocation`.
