# grāmatr

Real-time intelligent context engineering.

grāmatr is an AI platform. It sits between AI clients and agents and the work they do. With each request it assembles an **intelligence packet**: the directives and standards that apply, the context and knowledge that matter, and what has been learned before. A purpose-built model of our own, designed in the manner of a "System 1", acts as a fast first pass that responds in under 100 milliseconds: it pre-processes each request before it reaches a frontier model, so the larger model is used where it adds the most. Applications built on grāmatr start every request informed and behave consistently from one session to the next.

## Open source

### Guards: keep secrets out of AI agent sessions

The guards are a small, open-source safety layer for AI coding agents. They redact secrets in tool output, stop an agent from reading credential files or publishing a credential, and note possible personal data and prompt injection. They ship as two packages that move in lockstep:

| Project | What it is |
|---|---|
| [**guards-unified**](https://github.com/gramatr/guards-unified) | The server image: the secret, PII and prompt-injection detection behind one small service. |
| [**claude-plugin-guards**](https://github.com/gramatr/claude-plugin-guards) | The Claude Code plugin: hooks and an MCP server that wire the image into a session. |

Every release publishes signed build provenance, an SBOM and a full vulnerability scan with the image, so you can check what you are running. Start with the latest release of either repository.

### Why we do this in the open

grāmatr was built on the belief that the gap between a person who has an AI tool and a person who has a learning intelligence layer behind it is one of the most important gaps to close. An AI is only as good as what it knows when it starts: the rules it must follow, the context that applies, and what has already been learned. Getting that to it every time, and without delay, is what makes results consistent and shortens the time to value.

An AI that is handed that much also has to be trusted with it. Anything that sits between an AI agent and your secrets has to earn trust, not ask for it. So this part we keep small and open: you can read the code, check the signed release, and see exactly what it does and what it does not catch. The hard rule is no secrets; everything beyond that is best effort, and says so.

### What these projects are, and what they leave to you

The guards are a protection layer: an inference layer that detects secrets, personal data and prompt injection, and tools that put it between a person and an AI agent. They stay small on purpose. What to do about a finding beyond the hard rule of no secrets is a judgment for the platform that adopts the guards, and policy, audit and review are that platform's to decide. Any platform can adopt them, grāmatr included, and they work on their own.

### Contributing and security

Questions are welcome in [Discussions](https://github.com/gramatr/.github/discussions), and bug reports and proposals as issues. We review code only for changes we agreed to beforehand: propose first, as described in the [contributing guide](https://github.com/gramatr/.github/blob/main/CONTRIBUTING.md). If you find a security problem, please report it privately through the **Security** tab of the repository (Report a vulnerability); see our [security policy](https://github.com/gramatr/.github/blob/main/SECURITY.md).

## More

[gramatr.com](https://gramatr.com)
