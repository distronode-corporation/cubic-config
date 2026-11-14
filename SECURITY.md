# Security policy

## Supported versions

This repository holds configuration, not released software. Only the current `cubic.yaml` on
the default branch is in use, so that is the only version supported.

| Version | Supported |
|---|---|
| Default branch | Yes |
| Anything older | No |

## Reporting a vulnerability

Please report privately, not in a public issue, discussion or pull request.

- **Preferred:** GitHub's private vulnerability reporting. Open the repository's
  **Security** tab and choose **Report a vulnerability**, or go straight to
  <https://github.com/distronode-corporation/cubic-config/security/advisories/new>.
- **Fallback:** email **opensource@distronode.com** if you cannot use GitHub.

Include what you did, what happened, and what you expected. A proof of concept is welcome
but not required. Never include a real token or credential; if one is part of the problem,
say where it appeared, not what it was.

In scope here is anything in `cubic.yaml` that weakens review across the organization, for
example a setting that lets an outside contributor's pull request skip review, or an ignore
pattern that hides source code rather than generated files or lockfiles.

Expect an acknowledgement within a few working days. This is a small project with no paid
bug bounty; what you get is credit in the commit that fixes it, if you want it.
