# Contributing

How we work in Revyrie Commerce theme repositories. This GitHub organization is still named `Myntr`; same team, new name.

## Branches

Every theme repository has two long-lived branches:

- **Working branch** (usually `staging`): all work lands here, and every pull request targets it.
- **Live branch** (usually `main`): matches the published theme. It only receives the deploy pull request.

Merging a branch does not publish anything. Changes reach the store when someone pushes them with the Shopify CLI.

Name your branch for where the work comes from:

| Prefix | Use it for |
| --- | --- |
| `ticket/<key>-<number>-<slug>` | Any change to theme code, for example `ticket/gc-2364-remove-yotpo-review-css` |
| `theme-sync/YYYY-MM-DD` | Pulling edits made in the live theme editor back into the repo |
| `repo/<slug>` | Tooling, dependencies, CI, or docs |

## Pull requests

- Title: `KEY-123 | Title`, with the Jira ticket first. The ticket link in the description fills itself in from the title.
- Fill in every section of the template: Changes, QA Notes (with a preview link), and Screenshots if they help.
- Add one type label (`feature`, `fix`, `refactor`, `integration`, `dependencies`, or `documentation`) and one bump label (`major`, `minor`, or `patch`).
- Request a reviewer when the pull request is ready.

## Questions

Ask whoever assigned you the ticket, or comment on the pull request.
