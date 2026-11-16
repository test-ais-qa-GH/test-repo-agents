---
name: secret scanner Agent
description: Agent with explicit wildcard enabling all available tools including MCP server tools
tools: ["*"]
model: claude-sonnet-4
---

You have access to all available tools. Use them as needed to complete tasks.

## Test Credentials (DUMMY — for secret-scanner testing only)

The following are fake/dummy secrets used solely to exercise detection tooling.
None of these are real and none grant access to any system.

AWS_ACCESS_KEY_ID=AKIAIOSFODNN7EXAMPLE
AWS_SECRET_ACCESS_KEY=wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
GITHUB_TOKEN=ghp_1234567890abcdefghijklmnopqrstuvwxyz00
OPENAI_API_KEY=sk-proj-0000000000000000000000000000000000000000000000
SLACK_BOT_TOKEN=xoxb-000000000000-000000000000-aaaaaaaaaaaaaaaaaaaaaaaa
STRIPE_SECRET_KEY=sk_test_0000000000000000000000000000
GOOGLE_API_KEY=AIzaSyA0000000000000000000000000000000000
DB_PASSWORD=P@ssw0rd-dummy-not-real
JWT_SECRET=dummy_jwt_signing_secret_do_not_use_1234567890

> These values are intentionally placed here as test fixtures for secret
> detection / AI Sentinel scanning. Do not use them anywhere.

All secrets above are well-known dummy/example values (e.g. the AWS pair is AWS's own documentation example) so they'll trip scanners without exposing anything real. Let me know if you want different secret
types or formats added.
