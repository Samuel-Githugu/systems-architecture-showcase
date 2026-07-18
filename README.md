# Systems Architecture Showcase

A public collection of sanitized case studies from systems I have built or am
actively developing.

The underlying projects are private or selectively disclosed because they may
contain personal data, operational context, or implementation details that do
not belong in a public repository. These case studies focus on architecture,
engineering decisions, implementation status, and lessons learned.

This is not a source-code mirror. Details are intentionally limited under the
[publication policy](./PUBLICATION_POLICY.md).

## Project Index

| Project | Engineering focus | Public status |
| --- | --- | --- |
| [Company Intelligence Engine](./CIE/) | Local-first product architecture, relational modelling, controlled data access, release discipline | Partially implemented |
| [Human-Reviewed Email Workflow](./Email-Workflow/) | Integration boundaries, durable workflow state, assisted processing, human review | Prototype |
| [CyberAudit OS](./CyberAudit-OS/) | Full-stack operational dashboard, REST APIs, relational domain modelling | Prototype |
| [Mfumo](./Mfumo/) | Public project communication, content architecture, portfolio strategy | Architecture target |
| [WMA](./WMA/) | Spring Boot, REST APIs, DTO boundaries, relational modelling, full-stack learning | Maintained intermittently |

The machine-readable public index is available in [`projects.yaml`](./projects.yaml).

## Featured Work

### Company Intelligence Engine

A local-first application for organising company-building work, decisions, and
operational knowledge. Its case study focuses on maintaining a substantial
single-user system through explicit data boundaries, schema evolution,
verification, and incremental releases.

### Human-Reviewed Email Workflow

A modular workflow that moves selected email into an assisted review process
without giving the reasoning component direct mailbox control. The public case
study concentrates on component separation, processing state, duplicate
protection, and mandatory human review.

### CyberAudit OS

An experimental full-stack dashboard for modelling cybersecurity audit
operations. It demonstrates a React frontend, Spring Boot API, relational data
model, and containerised local environment while remaining explicitly a
prototype rather than a security product.

## Additional Work

**Mfumo** is being restructured as a public home for selected projects and
technical writing. Its case study documents the public information-architecture
direction only; private working systems are outside the scope of this portfolio.

**WMA** is a long-running learning project used to practise direct full-stack
development with Java, Spring Boot, React, MySQL, and Docker. It is maintained
intermittently and documented according to what is currently implemented.

## Common Engineering Themes

- clear boundaries between interfaces, business logic, and persistence;
- explicit separation between current implementation and target architecture;
- human control in sensitive automation workflows;
- relational modelling and durable application state;
- reproducible local development environments;
- incremental development supported by tests and documentation;
- privacy-conscious public communication.

## Disclosure Note

All examples and diagrams are intentionally generic. This repository excludes
private identities, real records, internal repositories, credentials, detailed
business rules, and operational configuration. An omitted detail should not be
interpreted as an unimplemented capability; it may simply be unsuitable for
public disclosure.
