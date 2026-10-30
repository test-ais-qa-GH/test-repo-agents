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

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 2: Security Guideline

When reviewing code changes, ensure compliance with security policy 2. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 3: Security Guideline

When reviewing code changes, ensure compliance with security policy 3. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 4: Security Guideline

When reviewing code changes, ensure compliance with security policy 4. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 5: Security Guideline

When reviewing code changes, ensure compliance with security policy 5. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 6: Security Guideline

When reviewing code changes, ensure compliance with security policy 6. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 7: Security Guideline

When reviewing code changes, ensure compliance with security policy 7. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 8: Security Guideline

When reviewing code changes, ensure compliance with security policy 8. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 9: Security Guideline

When reviewing code changes, ensure compliance with security policy 9. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 10: Security Guideline

When reviewing code changes, ensure compliance with security policy 10. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 11: Security Guideline

When reviewing code changes, ensure compliance with security policy 11. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 12: Security Guideline

When reviewing code changes, ensure compliance with security policy 12. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 13: Security Guideline

When reviewing code changes, ensure compliance with security policy 13. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 14: Security Guideline

When reviewing code changes, ensure compliance with security policy 14. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 15: Security Guideline

When reviewing code changes, ensure compliance with security policy 15. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 16: Security Guideline

When reviewing code changes, ensure compliance with security policy 16. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 17: Security Guideline

When reviewing code changes, ensure compliance with security policy 17. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 18: Security Guideline

When reviewing code changes, ensure compliance with security policy 18. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 19: Security Guideline

When reviewing code changes, ensure compliance with security policy 19. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 20: Security Guideline

When reviewing code changes, ensure compliance with security policy 20. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 21: Security Guideline

When reviewing code changes, ensure compliance with security policy 21. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 22: Security Guideline

When reviewing code changes, ensure compliance with security policy 22. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 23: Security Guideline

When reviewing code changes, ensure compliance with security policy 23. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 24: Security Guideline

When reviewing code changes, ensure compliance with security policy 24. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 25: Security Guideline

When reviewing code changes, ensure compliance with security policy 25. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 26: Security Guideline

When reviewing code changes, ensure compliance with security policy 26. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 27: Security Guideline

When reviewing code changes, ensure compliance with security policy 27. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 28: Security Guideline

When reviewing code changes, ensure compliance with security policy 28. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 29: Security Guideline

When reviewing code changes, ensure compliance with security policy 29. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 30: Security Guideline

When reviewing code changes, ensure compliance with security policy 30. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 31: Security Guideline

When reviewing code changes, ensure compliance with security policy 31. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

### Rule 32: Security Guideline

When reviewing code changes, ensure compliance with security policy 32. This includes checking for proper input validation, output encoding, authentication verification, and authorization checks. All API endpoints must implement rate limiting. Database queries must use parameterized statements. File operations must validate paths. Cryptographic operations must use approved algorithms.

**Checklist:**
- Verify input validation on all user-supplied data
- Check output encoding for XSS prevention
- Confirm authentication tokens are properly validated
- Ensure authorization checks exist for all protected resources
- Validate that error messages do not leak sensitive information
- Review logging to ensure no PII or secrets are written to logs
- Check that all external API calls use TLS 1.2 or higher
- Verify CORS configuration restricts origins appropriately

## Summary

This concludes the large agent definition. This file tests connector handling near the 30K limit.
