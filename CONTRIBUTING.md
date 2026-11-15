# Contributing to Primordial Rise

Primordial Rise is a proprietary, commercial game. Its game repositories are **private**,
and only invited team members can work on them. Being invited does not grant any rights
to the code or assets beyond what your agreement with the project says.

If you are not on the team, you can still help a lot: report bugs, share playtest
feedback and suggest ideas through [the support forms](SUPPORT.md).

The rest of this page is the team's workflow.

## Workflow

1. **Start from an issue.** Every change links an issue that says why it is needed.
   Small fixes can open the issue and the pull request together.
2. **Branch from `main`.** Name the branch for the change: `feat/...`, `fix/...`,
   `docs/...`, `chore/...`. Never push to `main` directly.
3. **Commit with [Conventional Commits](https://www.conventionalcommits.org/)**, scoped
   where it helps: `feat(client): ...`, `fix(sim): ...`, `docs: ...`.
4. **Open a pull request** with the template filled in. Keep it to one coherent change.
5. **CI must be green**, and the pull request reviewed, before it merges. Merges are
   squash merges.

## What every change needs

- **Tests** for new behaviour, run with the repository's own test command (not just a
  build).
- **Saves keep working.** Breaking a player's save is the worst bug we can ship. A change
  to stored data must load data written by the previous version, with a test that proves
  it.
- **Visuals for anything visible.** A change you can see ships with screenshots or a
  short GIF in the pull request, and refreshes the docs' images when the UI changes.
- **Docs** updated in the same pull request when behaviour or setup changes.
- **No secrets** in code, commits, logs or screenshots.

## Confidentiality

Game code, rules, tuning, roadmaps and unreleased art stay inside the private
repositories. Do not post them in public places, including this repository's issues, and
do not name private repositories in public posts.

## Code of conduct

Everyone who takes part follows the [Code of Conduct](CODE_OF_CONDUCT.md).
