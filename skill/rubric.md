## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| Alive | Last 10 commits on the default branch (Code tab commit list, or Insights → Commits) | At least one commit within the last 90 days | required |
| In-Use | Star count and open issue count, shown in repo header | ≥50 stars, OR ≥5 open issues with activity (comments/labels) in the last 90 days | required |
| Scope | Issue body text under the specific issue in the Issues tab | Bug: includes reproduction steps and expected vs. actual behavior. Feature: describes what it should do, what problem it solves, and what files/areas are relevant | required |
| Unclaimed | Assignees field in issue sidebar, comment thread, linked PRs shown above issue body | No assignees; no comments within the last 60 days claiming the issue; no open linked PR | required |
| Newcomer-friendly label | Labels on the issue (Issues tab) | Has `good first issue` or `help wanted` label | preferred |
| Maintainer responsiveness | Comment timestamps on the last 3-5 closed issues | Maintainer replied within 14 days on most of them | preferred |

## Verdict rule

Accept only if every required check passes. If any required check is `unclear`, treat it as fail (reject) — do not guess in the maintainer's favor. Preferred checks never flip accept/reject; use them only to rank issues that already passed all required checks (more preferred checks passed = higher priority).
