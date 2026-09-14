# Security Policy

## Reporting a Vulnerability

Report security vulnerabilities by e-mail to Sergio at sergio@brighenti.me.

Do **not** open a public issue for security problems.

Reports that follow the rules below are taken seriously and addressed promptly.
Reports that do not follow them are closed without a reply.

## Scope

**Only code that is part of a published release is in scope.**

Anything that is not in a tagged release — development branches, unmerged pull
requests, work in progress on `master` or any other branch — is explicitly out
of scope. That code is not meant to run in production, it is not distributed to
users, and it may be rewritten or removed before it ever ships. Reports against
it will not be considered.

Every report must state the exact release (tag) it applies to. A report without
a release version is not actionable and will be discarded.

## Mandatory Manual Validation

**Every report must be manually validated by a human before it is sent.**

At a minimum, a report must include:

1. The affected release version (tag).
2. The affected file(s) and line(s).
3. Concrete, step-by-step reproduction instructions against a real,
   freshly installed instance of that release.
4. Evidence that you actually ran those steps and observed the issue
   (request/response, logs, screenshots, or a working proof of concept).
5. A realistic description of the impact, including which privileges an
   attacker needs.

"I believe this may be exploitable", "this pattern is generally unsafe", or a
paste of a tool's output is not a vulnerability report. If you have not
reproduced it, do not send it.

## AI-Generated Reports

Unvalidated AI output is not a security report. Reports that are clearly
machine-generated and never verified by a human — AI slop — receive **no
response** and are deleted. Repeated submissions of this kind get the sender
blocked.

If you use an AI assistant or an automated scanner to look for vulnerabilities
in XBackBone, then **opening a pull request with a working fix is mandatory**.
The pull request must:

- Target a supported release.
- Contain an actual fix, not a description of one.
- Include a test that fails before the fix and passes after it.
- Pass the existing test suite and static analysis.

No pull request, no report. Triaging unverified machine output is work that is
pushed onto a volunteer maintainer, and it will not be done for you.