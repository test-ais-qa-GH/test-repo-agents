---
name: Large Agent Stress Test
description: Agent with very large instructions body to test the 30K character limit handling and Base64 decode performance
model: gpt-4o
tools: ["read", "edit", "search", "execute"]
user-invocable: true
disable-model-invocation: false
metadata:
  test-type: performance
  size: large
mcp-servers:
  stress-test-mcp:
    type: local
    command: npx
    args: ["stress-test-server"]
    tools: ["analyze", "report", "benchmark"]
    env:
      API_KEY: ${{ secrets.POLICY_API_KEY }}
---

# Large Agent — Performance and Size Limit Test

This agent tests handling of large .agent.md files near GitHub s 30000 character maximum.

## Security Policy Guidelines

### Rule 1: Security Guideline

When reviewing code changes, ensure compliance with security policy 1. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

keeping short for now will check with near 30k characters
