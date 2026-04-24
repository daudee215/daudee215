# Maintenance Standards

Working notes for keeping the portfolio repositories in a reviewable state. The
aim is that anyone landing on a repository can tell what it does, run it, and
see that the results hold up.

## What counts as a real improvement

A commit should leave the repository more useful than it found it. In practice
that means one of the following:

- A test or validation fixture, with the expected result documented.
- A bug fix, with the case that exposed it captured in the test suite.
- Clearer run instructions, a documentation index, or a worked example.
- A data dictionary entry with units and a null policy.
- A smoke-test workflow or CI check.
- Better error messages or edge-case handling in a script.
- A case-study note covering the user, the problem, the data, and the output.

## What not to commit

- Empty commits, date-only edits, or formatting churn.
- Large generated files without a stated reason.
- Credentials, tokens, local lock files, or private client material.
- A claim that something is fixed without evidence that it is.

## Checks before pushing

Keep commits scoped, preferably one per repository, and run the checks that
actually apply:

| Repository type | Check to run |
| --- | --- |
| Node projects | `npm test` where a suite exists |
| Python scripts | The documented example command |
| Static interfaces | Confirm required files load and documented selectors resolve |
| Documentation only | `git diff --check` at minimum |

For behaviour-changing fixes a code diff is not evidence. Restart the process,
confirm it is listening, and capture real API or browser output before treating
the issue as resolved. If verification fails, report the blocker rather than
closing it out.

## After pushing

- Confirm local HEAD matches origin and the working tree is clean.
- Check any workflow the commit triggered and note success, failure, or pending.