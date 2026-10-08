# Google Drive ↔ GitHub ↔ SQLite reconciliation

1. Register an artifact ID, version, owner, classification and SHA-256 locally.
2. Upload approved document bytes to controlled Google Drive folder.
3. Read back the Drive metadata and bytes; verify SHA-256 against the source.
4. Commit only non-sensitive templates or approved manifest metadata to GitHub.
5. Record GitHub commit SHA, Drive file ID and revision ID in SQLite checkpoint ledger.
6. Re-read remote state and compare identifiers, checksums, and approval status.
7. Mark reconciliation PASS only when all checks pass; otherwise log a gap.

Never publish sensitive Drive links, document contents, credentials or local database dumps to a public repository.
