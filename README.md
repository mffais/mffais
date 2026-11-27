# I find the wording that makes AI pay out

I red-team AI agents that handle money. What matters isn't whether some backend control eventually blocks the action. It's what the agent commits to in the conversation: will it tell a customer, a vendor, or an employee yes to a refund, discount, credit, new terms, waived return, or payment it shouldn't, because they talked it into it? If the agent says yes, the company can be held to it, whether or not the money ever moves.

## What I'm building

A test harness for money-wording attacks. Each case passes or fails on what the agent agreed to, not on whether a downstream control would have caught it: did it commit to a refund, credit, or terms it shouldn't? If the agent says yes, the company can be held to that, so that's what I score.

* The wording that talks an agent into a refund, discount, credit, new terms, waived return, or payment it shouldn't make
* Semantic loopholes: the model blocks a "$5 credit" but clears a "$5 negative invoice." Same money, different word.
* Multi-turn manipulation: no single message trips a filter, but the conversation adds up to a yes it shouldn't give
* What automated scanners miss, because they match keywords, not meaning

## Why me

A few hundred people worldwide hold the AWS Golden Jacket (every active AWS certification at once). An estimated few hundred hold both the FPAC and CTP finance credentials. Almost no one holds all three. I know how the money moves, and I know the many ways to ask for it that a keyword or intent filter won't catch.

## Background

* 15 years as VP of IT, hands-on: built and ran the systems the money moved through, from payments and billing to ERP, and handled security from penetration testing to threat response.
* I build and operate real production systems end to end on AWS (serverless backends, multi-tenant isolation, least-privilege IAM, a SEC EDGAR XBRL pipeline across thousands of public companies), so I read an agent the way someone who has built and secured systems does.
* Multi-agent development: I build my own software with a team of AI agents for orchestration, development, and independent QA. Watching them report work as done when it was only planned is where my rule comes from.

Trust what you've tested. Not what the model promises.
