# action-template

Starting point for a new Action repo. When a proposal in [`actions-hub`](../) is approved, copy this folder's contents into a new repository and go from there.

## What to change

1. `action.yml` — fill in `name`, `description`, `inputs`, `outputs`, and the `runs` steps.
2. This README — describe what the action does and show a `uses:` example.
3. `.github/workflows/test.yml` — keep it green; it runs the action against itself on every push.

## Usage (fill in once published)

```yaml
- uses: anjaniswarna0/<your-new-repo>@v1
  with:
    example-input: value
```
