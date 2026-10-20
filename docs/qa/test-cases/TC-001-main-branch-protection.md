# TC-001: Direct push to `main` is blocked

| Field | Value |
|---|---|
| ID | TC-001 |
| Area | Repository controls / release gate |
| Type | Negative test |
| Priority | High |
| Related control | Ruleset `protect-main` (pull request required, deletions restricted, force pushes blocked) |

## Objective
Confirm that nobody can commit directly to `main`; every change must go through a pull request.

## Preconditions
- Ruleset `protect-main` is **Active** and targets the default branch.
- Local repository is on `main` and up to date.

## Steps
1. Create an empty commit on `main`: `git commit --allow-empty -m "test: direct push to main should be rejected"`
2. Run `git push`.
3. Reset the local branch: `git reset --hard origin/main`

## Expected result
The push is rejected with a repository rule violation.

## Actual result
The push was rejected:

```
remote: error: GH013: Repository rule violations found for refs/heads/main.
remote: - Changes must be made through a pull request.
 ! [remote rejected] main -> main (push declined due to repository rule violations)
```

## Result
**Pass**

## Notes
- Executed on 2026-10-20 by the project owner.
- Required approvals are set to 0 because GitHub does not allow approving your own PR in a one-person project. Real teams would require 1 or more.
- Not yet covered: force-push and branch-deletion rules were not tested.