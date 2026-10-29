# File Output and Verification Standard

This file is the repository-level operating standard for agents working in this project. It governs artifact creation and delivery; it does not override system/developer instructions, security requirements, access controls, or platform constraints.

## Deliverable integrity

- Deliver the actual final artifact, not a placeholder page or an intermediate version. Use direct links to the exact final files whenever the platform supports them.
- Use meaningful, human-readable filenames. Never leave `%XX` URL-encoding sequences inside the saved filename, and never use hashes, opaque IDs, or obfuscated names as user-facing filenames. If the platform percent-encodes Cyrillic filenames in the final download route, create a separate meaningful ASCII transliteration and verify that exact artifact and link.
- The local path is not proof that the final hosted or downloadable link points to the intended object. Check file existence, filename, type, size, and final delivery route separately to the extent the tools permit.
- Default to open, editable, copyable files. Do not add passwords, encryption, DRM, or view/copy/edit restrictions without a specific need and explicit user authorization.
- For PDF, inspect whether the document is encrypted/password-protected and inspect relevant permissions before claiming it is unrestricted. For HTML, confirm UTF-8, `lang="ru"` for Russian documents, self-contained styling where practical, responsive screen layout, print-ready A4 rules where applicable, and no unnecessary external dependencies.
- Do not confuse a server-side link-signature parameter such as `sig` with encryption or permissions inside the document.

## Verification before claims

- Check the exact final file, not just its source or an earlier copy.
- Inspect rendering when visual fidelity matters; inspect content and structure when semantic fidelity matters.
- Never claim that a link, render, permission, encryption state, upload, commit, or synchronization was verified unless the relevant check actually occurred.
- When a failure occurs, fix the artifact and the delivery path. An apology, repeated rule, or new unverified copy does not constitute a fix.
- State concrete tool or platform limitations when a check cannot be performed. Distinguish created, uploaded, committed, re-read, and verified states.

## Synchronization scope

- Writing to one repository, connector, memory store, account, chat session, or device does not automatically update the others.
- For every requested destination, use the actual available write operation and confirm it succeeded; re-read the destination when supported.
- Never claim global synchronization across all sessions, accounts, devices, or connectors based on one successful write.
- Keep project-specific changes scoped. Do not add personal standards to unrelated repositories unless that repository is explicitly intended as the target.
