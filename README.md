# code-code-platform-session

Session persistence, transcript state, and platform domain contract helpers for
Code Code.

This repository owns:

- `packages/session`: session repository, transcript message, resource, status,
  condition, and active-run persistence logic.
- `packages/platform-contract`: platform-owned Go domain contract helpers used
  by session and runtime state projection.
- `code-code-contracts`: generated shared contracts as a Git submodule.

Useful checks:

```bash
cd packages/platform-contract && go test ./...
cd packages/session && go test ./...
```
