# Contributing

Thank you for your interest. We welcome questions, bug reports and proposals. We review code only for changes we agreed to beforehand. That keeps these projects small and keeps your time from going into work we cannot merge.

## How to take part

1. **Ask a question.** Use [Discussions](https://github.com/gramatr/.github/discussions): how a guard behaves, what it does and does not catch, how to configure it.
2. **Report a bug.** Open an issue with the bug report form. Give the version and a description of the shape of the input, with a fabricated value.
3. **Propose a change.** Open an issue with the proposal form, and wait for it to be marked `accepted`. Write code only after that. A pull request that does not link to an accepted proposal is closed.
4. **Report a security problem, privately.** Use the Security tab of the repository and choose Report a vulnerability. See [SECURITY.md](SECURITY.md). Never describe a vulnerability in a public place.

**Never put a real credential, token, key or personal data in an issue, a discussion or a pull request**, not even a rotated or expired one. Describe its shape (length, character classes, which tool produced it) and use a made-up value of the same shape. Tests and fixtures in these projects are built the same way.

## What we do with what you send

These are small projects and we answer on a best-effort basis; no response time is promised. New issues get the `needs-triage` label. We then accept the issue, ask for more information (`needs-info`), or close it as out of scope. We may close or lock anything that is off topic, repeated or breaks the [code of conduct](CODE_OF_CONDUCT.md).

## What belongs in these projects

The open-source repositories provide an inference layer and the tools that protect a user from AI exposure, and they stay small and honest. The hard rule is no secrets: redact them in output, block them in publishes and commits, deny credential files, fast and synchronous. PII and prompt-injection findings are best-effort notices. Nuanced judgments, organisation-wide policy, audit and review belong to the platform that adopts the guards, whether that is grāmatr or any other, and are out of scope here. A proposal that adds that machinery will not be accepted, whoever sends it.

## Changes to code

Code is reviewed only for an accepted proposal, and only if it meets this minimum. A pull request that does not is closed without review.

1. **An accepted proposal.** The pull request links to it.
2. **A DCO sign-off on every commit.** Add it with `git commit -s`. It appends a `Signed-off-by: Your Name <your@email>` line, which certifies the [Developer Certificate of Origin](https://developercertificate.org): that you wrote the change or have the right to submit it under the project's licence. We use the DCO and not a contributor licence agreement because the projects are MIT-licensed.
3. **Signed commits.** The main branch of each project accepts only commits that GitHub shows as Verified. We squash-merge, so GitHub signs the merge commit; signing your own commits (GPG, SSH or S/MIME) is encouraged and makes review easier.
4. **Tests.** The change has tests. Their fixtures are built at run time with fabricated values.
5. **No real credentials or personal data**, anywhere: not in code, tests, commit messages or the description.
6. **Checks pass.** The project's automated checks must be green.
7. **Small and in scope.** One concern per pull request, within the scope above.
8. **Documentation.** Update it where behaviour changes. A change to a hook also gives before-and-after timing of the common path, an off switch, and a fallback to the previous behaviour.

We may close any pull request that is out of scope, unreviewed for a long time, or not moving. Closing it is not a judgment of you.
