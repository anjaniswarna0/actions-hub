# action-template

Starting point for a new Action repo. When a proposal in [`actions-hub`](../) is approved, copy this folder's contents into a new repository and go from there.

## What to change

1. `action.yml` — fill in `name`, `description`, `inputs`, `outputs`, and the `runs` steps.
2. This README — describe what the action does and show a `uses:` example.
3. A test workflow in the new repo's own `.github/workflows/` — see the note below.

## Important: workflow file location

GitHub Actions only reads workflows from `.github/workflows/` at the **root** of a repository — never from a subfolder. That's why this template's CI check lives at [`/.github/workflows/test-action-template.yml`](../.github/workflows/test-action-template.yml) in *this* repo (`actions-hub`), one level up from here, instead of inside `action-template/` itself.

When you copy this folder into a brand-new repo, also copy that workflow file into the new repo's `.github/workflows/test.yml` (at the new repo's root) — otherwise your tests silently never run.

## Usage (fill in once published)

```yaml
- uses: anjaniswarna0/<your-new-repo>@v1
  with:
    example-input: value
```
