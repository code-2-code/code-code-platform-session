# Agent Rules

- This repository owns session persistence, transcript state, active-run state,
  and platform domain contract helper packages.
- Do not edit protobuf source or generated contract bindings here.
- If a public contract must change, make that change in `code-code-contracts`
  first, then update this repository to the released contract version.
- Keep runtime orchestration, provider, auth, egress, profile, catalog,
  notification, UI, and deployment behavior out of this repository.
- Keep persistence changes atomic and covered by the narrowest relevant tests.
