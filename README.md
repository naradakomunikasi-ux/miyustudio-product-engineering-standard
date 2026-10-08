# MiyuStudio Product Engineering Standard

Standar proses product-to-production untuk proyek MiyuStudio.

## Lifecycle
PRD → TOGAF → Workbook → Sitemap → UI/UX Runnable HTML → Design Freeze → Engineering Readiness → Coding & Testing → Release → Operations.

## Source of truth
- Google Drive: controlled handbook documents and approved releases.
- GitHub: reusable templates, engineering controls, CI configuration, and non-sensitive manifests.
- SQLite: local governance checkpoint ledger; never commit internal database files to a public repository.

## Release policy
A release is FINAL only after source validation, visual/document QA, security review, traceability, owner acceptance, and cross-system reconciliation.

## Confidentiality
This repository is PUBLIC. Do not commit personal data, credentials, internal project records, unpublished manuscripts, or private SQLite files.
