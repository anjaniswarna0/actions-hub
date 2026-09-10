# actions-hub

A working demo of how a GitHub Actions org (like `Amtrak-actions`) can let anyone propose a **new Action repo**, and how that proposal turns into a real, reviewed repository.

This mirrors a pattern used by many action-hosting orgs: a request comes in as a structured issue, maintainers triage it, and — once approved — a new repo is stamped out from a template so every action repo looks and behaves the same way.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for the full process.

## How a proposal becomes a repo

```
Contributor
   |
   v
Opens an Issue here using
"New Action Proposal" template
   |
   v
Maintainers triage
   |
   +-- Rejected --> issue closed, reason given
   |
   v (Approved)
Maintainer creates a new repo
from action-template/
   |
   v
Contributor opens a PR with the action code
   |
   v
CI runs (lint + test)
   |
   +-- Fails --> back to contributor
   |
   v (Passes)
Review by CODEOWNERS
   |
   v
Merge to main + tag a release (v1)
   |
   v
New action is live
```

`action-template/` in this repo is exactly what a maintainer copies to start a brand-new action repo — see [action-template/README.md](./action-template/README.md).
