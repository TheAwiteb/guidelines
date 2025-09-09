# Contributing

## Contribution Workflow

Before writing code, please read [our code style](./CODE_STYLE.md).

To contribute a patch:

- Fork the repository 
- Create a topic branch 
- Commit patches (PR, emails, nostr, ...)

In general, commits should be atomic and diffs **easy to read**.

## Deprecation policy

Where possible, breaking existing APIs should be avoided.
Instead, add new APIs and mark the old ones as deprecated.

Deprecated APIs are typically maintained for one release cycle.
In other words, an API that has been deprecated with the 0.10 release 
can be expected to be removed in the 0.11 release.
This allows for smoother upgrades without incurring too much technical debt inside this library.

If you deprecated an API as part of a contribution, we encourage you to "own" that API
and send a follow-up to remove it as part of the next release cycle.

### Terminology

Concept ACK — Agree with the idea and overall direction, but haven't reviewed the code changes or tested them.

utACK (untested ACK) — Reviewed and agree with the code changes but haven't tested them.

tACK (tested ACK) — Reviewed the code changes and have verified the functionality or bug fix.

ACK — A loose ACK can be confusing. It's best to avoid them unless it's a documentation/comment-only change in which case there is nothing to test/verify; therefore, the tested/untested distinction is not there.

NACK — Disagree with the code changes/concept. Should be accompanied by an explanation.
