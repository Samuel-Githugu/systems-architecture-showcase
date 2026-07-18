# Public Portfolio Publication Policy

This repository is a deliberately limited public view of private and evolving
engineering work. Its purpose is to demonstrate engineering judgement without
disclosing private context, sensitive data, or enough implementation detail to
reconstruct a private system.

When accuracy, completeness, and privacy conflict, privacy takes priority.
Omission is the default when disclosure is uncertain.

## 1. Allowed Content

The portfolio may publish:

- a generic description of the problem a project addresses;
- broad architectural boundaries and component responsibilities;
- technologies that are materially present in the implementation;
- sanitized, high-level data flows;
- engineering decisions and lessons that do not reveal private operations;
- honest implementation status and clearly labelled future work;
- synthetic examples that cannot be connected to a real person or organisation.

## 2. Prohibited Content

The portfolio must not publish:

- employer, client, customer, tenant, family, or other private-person names;
- private project codenames or private repository URLs;
- real messages, records, documents, addresses, identifiers, or financial data;
- credentials, secrets, tokens, tenant configuration, mailbox identifiers, or
  permission details;
- local filesystem paths, workstation details, or private deployment topology;
- private prompts, routing rules, scoring thresholds, business rules, or
  operational playbooks;
- detailed internal schemas or contracts that are not intentionally public;
- screenshots derived from real or private data;
- security weaknesses described with unnecessary exploit detail;
- planned capabilities presented as implemented;
- claims of production use, scale, impact, or reliability without publishable
  evidence.

An internal denylist of private names and terms may be used during review, but
that denylist must not be committed to this public repository.

## 3. Status Vocabulary

Every project uses one of these public statuses:

| Status | Meaning |
| --- | --- |
| Implemented | The described capability exists and has been verified. |
| Partially implemented | A working foundation exists, but named parts remain incomplete. |
| Prototype | A working experiment or demonstration, not a production system. |
| Architecture target | A designed future state that is not yet implemented. |
| Planned | Intended work with no claim of current implementation. |
| Maintained intermittently | A real project developed without a regular delivery cadence. |

Each case study must include a current-state section that separates implemented,
partial, and planned capabilities.

## 4. Safe Technical Depth

Architecture diagrams should explain responsibility boundaries, not reproduce
the private implementation. They should avoid real infrastructure names,
identifiers, network details, credentials, internal endpoints, exact contracts,
and private data models.

Code excerpts, sample payloads, screenshots, and detailed schemas are excluded
unless they are intentionally created for public use and pass the publication
review below.

## 5. Publication Workflow

Updates follow this sequence:

1. Inspect private sources in a read-only manner.
2. Draft a minimal public-safe change locally.
3. Verify every implementation claim against code, tests, or current project
   documentation.
4. Run privacy, secret, path, link, and placeholder checks.
5. Review the complete diff for unnecessary disclosure.
6. Obtain explicit human approval.
7. Only then commit, push, or publish.

No scheduled process or agent may publish directly to the public branch.

## 6. Shared Public Metadata

`projects.yaml` is the approved public project index. Other public surfaces may
consume or copy only the fields in that file. Private repositories must not be
queried during a public website build.

Automated or scheduled audits may identify stale entries and prepare proposed
changes. They must not update `projects.yaml` or public documentation without
the manual publication gate.

## 7. Final Review Questions

Before publication, every change must answer yes to all of the following:

- Is every claim supported and correctly labelled?
- Is every included detail necessary to demonstrate the engineering work?
- Would disclosure remain acceptable if read by an employer, client, or the
  subject of the underlying data?
- Can the example be understood without private context?
- Has uncertain or unnecessarily detailed information been removed?

If any answer is no or unclear, do not publish the detail.
