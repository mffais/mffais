# Red-teaming AI agents that take real actions

I red-team AI agents that call tools, read untrusted content, and act on data with real permissions. The question isn't what the model says. It's what the agent does.

## What I'm building

A test harness for agent attacks, scored on actions, not answers: each case passes or fails on whether a forbidden tool call happened.

- Indirect prompt injection through documents, web pages, emails, and tool outputs
- Tool poisoning and malicious MCP servers
- Data exfiltration through tool calls
- Excessive agency: agents doing more than they should with the access they're given

## Background

- **15 years as VP of IT, hands-on:** on-site to cloud migration, ERP migrations, API services, custom ordering, warehouse, and payment systems, disaster recovery, patching, penetration testing, and threat response
- **Production AWS systems, built and operated end to end:** serverless backends on Lambda, API Gateway, and Aurora; multi-tenant isolation with a separate database, role, and encryption key per account; least-privilege IAM with permissions boundaries; OIDC-based CI/CD; an ingestion pipeline for SEC EDGAR XBRL filings across thousands of public companies
- **Multi-agent development:** I build my own software with a team of AI agents for orchestration, development, and independent QA

## AWS stack

- **Compute / serverless:** Lambda, API Gateway, EventBridge
- **Data:** Aurora (PostgreSQL), RDS Proxy, S3
- **Infra / platform:** Terraform, multi-account, IAM and permissions boundaries, CloudFront, CodeBuild

## Certifications

Golden Jacket: every active AWS certification at once, including Security Specialty. An estimated few hundred people worldwide hold it.

---

*Trust what you've tested. Not what the model promises.*
