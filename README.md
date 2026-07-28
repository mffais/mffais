# Cash Horizon: finance software, built by an operator

Cash flow forecasting and tracking that runs in your own AWS account. I'm a finance operator with 15 years owning a P&L who builds the software, not just advises on it.

> Most cash forecasting lives in a fragile spreadsheet. I build the system a finance team can actually trust: deterministic, transparent, and deployed where your data never leaves your control.

## What I build

**Cash Horizon** - cash flow forecasting and tracking software. Deterministic and finance-grade, deployed per customer in their own AWS account, with tenant isolation and least-privilege built in.

## Built, not just advised

Production AWS systems designed and operated end to end:

- Serverless finance application on Lambda, API Gateway, and Aurora
- Multi-account, per-customer isolated deployment: one instance per customer, data never co-mingled
- The production engineering that separates a demo from a system: least-privilege IAM with permissions boundaries, in-VPC data provisioning, OIDC-based CI/CD, and idempotent migration pipelines
- A large-scale ingestion pipeline processing SEC EDGAR XBRL filings across thousands of public companies

## AWS stack

- **Compute / serverless:** Lambda, API Gateway, EventBridge
- **Data:** Aurora (PostgreSQL), RDS Proxy, S3
- **Infra / platform:** Terraform, multi-account, IAM and permissions boundaries, CloudFront, CodeBuild

## Certifications

Golden Jacket: every active AWS certification at once, the complete current stack. An estimated few hundred people worldwide hold it.

---

*A finance operator who builds. Repos here reflect production-oriented finance and AWS work; not all are public or complete.*
