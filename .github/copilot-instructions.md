# Repository AI Instructions — File Output and Verification

Apply these rules when creating, editing, exporting, or delivering files in this repository. They do not override system/developer instructions, security requirements, access controls, or platform constraints.

- Deliver the actual final artifact and direct links to exact final files wherever supported; do not substitute a placeholder page or intermediate version.
- Use meaningful, human-readable filenames. Do not leave `%XX` URL-encoding sequences in saved filenames, and do not use hashes or opaque IDs as user-facing names. If Cyrillic names are encoded in the final delivery route, create a separate, meaningful ASCII-transliterated file and verify that exact file and link.
- Check existence, filename, type, size, essential content, and final delivery route separately where tooling permits. A valid local path is not proof that the user-facing link targets the right file.
- Default to open, editable, copyable artifacts. Do not add passwords, encryption, DRM, or viewing/copying/editing restrictions without a concrete need and explicit authorization.
- For PDFs, inspect actual encryption/password status and relevant permissions before describing the file as unrestricted. For HTML, verify UTF-8, `lang="ru"` for Russian material, sensible structure, responsive layout, print rules when needed, and no unnecessary external dependencies.
- A URL signing parameter such as `sig` is a server-side link detail, not evidence that the document itself is encrypted or restricted.
- Verify rendering when visual fidelity matters. Never claim a render, link, permission, upload, commit, or synchronization was checked unless the check actually happened.
- After a failure, fix the artifact and the delivery route; a repeated rule, apology, or unverified copy is not a fix.
- Treat each repository, connector, memory store, session, account, and device as a separate destination. One successful write does not imply global synchronization. Confirm writes and re-read destinations when supported.
- Keep changes scoped to the requested project. Do not modify unrelated repositories or expose personal information as part of generic project instructions.
