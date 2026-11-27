# I find the wording that makes AI pay out

I red-team AI agents that handle money. The question isn't what the model says. It's what the agent does: will it approve the refund, the discount, the credit, the new terms, the waived return, or the payment it shouldn't, because a customer, a vendor, or an employee talked it into it?

## What I'm building
A test harness for money-wording attacks, scored on actions, not answers: each case passes or fails on whether the agent took a money action it shouldn't.

* The wording that talks an agent into a refund, discount, credit, new terms, waived return, or payment it shouldn't make
* Semantic loopholes: the model blocks a "$5 credit" but clears a "$5 negative invoice." Same money, different word.
* Multi-turn manipulation: no single message trips a filter, but the conversation adds up to a payout
* What automated scanners miss, because they match keywords, not meaning

## Why me
A few hundred people worldwide hold the AWS Golden Jacket (every active AWS certification at once). A few hundred hold both the FPAC and CTP finance credentials. Almost no one holds all three. I know how the money moves, and I know the many ways to ask for it that a keyword or intent filter won't catch.

## Background
* 15 years as VP of IT, hands-on: built and ran the systems the money moved through, from payments and billing to ERP, and handled security from penetration testing to threat response.
* I build and operate real production systems end to end on AWS (serverless backends, multi-tenant isolation, least-privilege IAM, a SEC EDGAR XBRL pipeline across thousands of public companies), so I read an agent the way someone who has built and secured systems does.
* Multi-agent development: I build my own software with a team of AI agents for orchestration, development, and independent QA. Watching them report work as done when it was only planned is where my rule comes from.

Trust what you've tested. Not what the model promises.
