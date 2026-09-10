# Contributing a new Action

Thanks for wanting to add a new Action! This repo is the front door for that request — read this before opening anything.

## 1. Check it doesn't already exist

Search existing action repos first. Duplicating an existing action just fragments maintenance.

## 2. Open a proposal issue

Use the **New Action Proposal** issue template (Issues → New Issue). Fill in:

- What the action does and why it's needed
- Proposed name
- Inputs / outputs it will expose
- Who will maintain it long-term
- Any alternatives you considered (existing actions, manual scripts, etc.)

## 3. Triage

A maintainer labels the issue within a few days:

- `needs-info` — we need more detail from you
- `approved` — go ahead, a repo will be created
- `declined` — closed with a reason (e.g. duplicate, out of scope)

## 4. Repo creation

Once approved, a maintainer creates the new repo from [`action-template/`](./action-template) in this repo, so it starts with the right structure: `action.yml`, a README, and a test workflow.

## 5. Open your PR

Push your actual action code to the new repo as a pull request, not directly to `main`. Your PR should include:

- The action implementation (`action.yml` plus any scripts)
- A README explaining inputs/outputs and a usage example
- A passing test workflow

## 6. Review and release

A CODEOWNER reviews the PR. Once merged, tag a release (`v1`) so consumers can pin to a stable version instead of `main`.

## Questions

Open a discussion or comment on your proposal issue — a maintainer will follow up.
