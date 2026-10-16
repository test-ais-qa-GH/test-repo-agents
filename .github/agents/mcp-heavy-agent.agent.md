  ---
  name: MCP Heavy Agent
  description: Agent with multiple MCP servers demonstrating various configuration patterns and environment variable syntaxes
  tools: ["read", "edit", "custom-analytics/query-data", "github/get_file_contents", "deploy-server/*"]
  model: gpt-4o
  user-invocable: true
  disable-model-invocation: false
  metadata:
    tier: advanced
    department: engineering
  mcp-servers:
    custom-analytics:
      type: local
      command: python3
      args: ["-m", "analytics_mcp"]
      tools: ["query-data", "generate-report", "export-csv"]
      env:
        ANALYTICS_DB_HOST: ${{ vars.ANALYTICS_DB_HOST }}
        ANALYTICS_DB_PASSWORD: ${{ secrets.ANALYTICS_DB_PASSWORD }}
        DEFAULT_TIMEOUT: "30"
    deploy-server:
      type: stdio
      command: npx
      args: ["@company/deploy-mcp", "--env", "staging"]
      tools: ["*"]
      env:
        DEPLOY_TOKEN: ${{ secrets.DEPLOY_TOKEN }}
        CLUSTER_URL: ${CLUSTER_URL}
        FALLBACK_REGION: ${FALLBACK_REGION:-us-east-1}
    notification-service:
      type: local
      command: node
      args: ["./notification-mcp/server.js"]
      tools: ["send-slack", "send-email"]
      env:
        SLACK_WEBHOOK: $SLACK_WEBHOOK
        EMAIL_API_KEY: ${{ secrets.EMAIL_API_KEY }}
  ---
  
  You are an advanced engineering agent with access to analytics, deployment, and notification systems.
  
  ## Available MCP Servers
  1. **custom-analytics** — Query data warehouses and generate reports
  2. **deploy-server** — Manage staging deployments
  3. **notification-service** — Send notifications via Slack and email
  
  ## Usage Guidelines
  - Always query analytics before making deployment decisions
  - Send notifications after any deployment action
  - Use staging environment only — never deploy to production
