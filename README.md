# NextKnock

**Your next opportunity starts with a conversation.**

NextKnock is a reusable agent skill for exploring your next career step, preparing job-platform profiles, applying selectively, and drafting researched messages that give someone a reason to reply.

It is a folder of instructions for a capable agent, not a standalone application. It does not include a CV, candidate database, account access, or an email-sending service.

[Download v0.1.0](https://github.com/prasidhgautam/nextknock/releases/download/v0.1.0/nextknock-v0.1.0.zip) · [Releases](https://github.com/prasidhgautam/nextknock/releases) · [License](LICENSE) · [Permissions](LICENSE-NOTICE.md)

## What it helps you do

1. **Start with your evidence.** Share your CV and portfolio files or links. No portfolio? Continue with your CV.
2. **Choose a direction.** Discuss the work you want, assess options against your experience, and agree on roles, location, working preferences, and constraints.
3. **Choose platforms.** Select the job platforms and Gmail account you want to use. Get help preparing existing profiles or establishing missing ones.
4. **Pursue suitable opportunities.** Research live vacancies and employers, explain fit, and prepare or submit applications within your requested scope.
5. **Start better conversations.** Draft concise messages informed by company research, ideally a relevant development from the preceding 12 months, and grounded in your actual work.
6. **Keep track.** Separate confirmed submissions, saved Gmail drafts, replies, and steps that need manual help.

Emails remain **unsent Gmail drafts by default** for you to review and send. An unavailable upload, login, verification challenge, or unsupported control becomes an explicit manual step. NextKnock checks the result before resuming.

## Install in Codex

1. Download the release ZIP above and extract it.
2. Copy the complete `nextknock` folder into `~/.agents/skills/`, so the manifest is at `~/.agents/skills/nextknock/SKILL.md`. For a project-only installation, use `.agents/skills/nextknock/` inside that project instead. If the destination exists, review or back it up before replacing it.
3. Invoke `$nextknock` in your next Codex prompt. If it does not appear, restart Codex.

You can also ask Codex's built-in `$skill-installer` to install the skill from the root of [this repository](https://github.com/prasidhgautam/nextknock).

See [OpenAI's skill documentation](https://learn.chatgpt.com/docs/build-skills) for supported local skill locations and invocation. Other hosts that support the Agent Skills format may use different installation paths; follow that host's instructions. This release is a standalone skill, not a marketplace plugin.

## Start a conversation

```text
Use $nextknock to review my CV and portfolio and help me figure out my next career step. Discuss options with me before choosing job platforms or applying anywhere.
```

For a later, scoped run:

```text
Use $nextknock to research three roles that fit our agreed brief. Explain the fit, then prepare company-specific Gmail drafts for my review. Leave them unsent.
```

Installing the skill does not start applications or access your accounts. You choose the work it performs.

## Capabilities and accounts

The host agent needs document-reading tools for your supplied materials and live web research for current roles and company facts. Supported browser controls or platform connectors are needed for account and application actions. A Gmail connector or supported Gmail browser session is needed to save drafts in your chosen account.

There is no bundled runtime, MCP server, API key, or connector subscription. Any account, host, or tool requirements and charges belong to the services you choose. The skill cannot grant permissions or enable capabilities the host lacks. Without account access, it can prepare local materials and explain the manual steps.

## Privacy and boundaries

Provide your own current CV and authorized portfolio materials. Keep them, account details, preferences, trackers, and application history **outside this repository and the installed skill folder**. Do not submit personal documents or credentials in GitHub Issues.

The agent should use confirmed candidate evidence, leave unknown answers unresolved, ask you to complete credentials and personal declarations, and verify submissions before counting them. It does not bypass CAPTCHA or platform restrictions, run background monitoring, or guarantee replies, interviews, or employment. Review materials before sharing them.

## Files and validation

- `SKILL.md`: entrypoint and workflow boundaries.
- `agents/openai.yaml`: display metadata and invocation prompt.
- `references/`: onboarding, platform assistance, outreach, and tracking guidance.

The workflow received an instruction-level review using ten fictional scenarios covering missing evidence, missing accounts, failed uploads, unavailable Gmail, research gaps, duplicate drafts, partial draft completion, uncertain submissions, and rejection handling. Structure, local references, naming, and publication contents are checked for this release. **Live execution against job platforms and Gmail has not been verified.** Host capabilities and platform interfaces can change.

## License, credit, and commercial permission

The written skill materials are available under [CC BY-NC 4.0](LICENSE), with attribution to [@prasidhgautam](https://github.com/prasidhgautam). See [LICENSE-NOTICE.md](LICENSE-NOTICE.md) for the additional permission covering an individual's own job search, including paid employment.

Commercial use of the skill materials requires separate permission. To discuss commercial redistribution, paid services, or product integration, open a [commercial-permission inquiry](https://github.com/prasidhgautam/nextknock/issues). Opening an issue does not grant permission or establish a price. This is a public project with noncommercial licensing; it is not offered under an OSI-approved open-source license.

NextKnock is an independent community-created career skill and is not affiliated with similarly named recruiting firms, OpenAI, or the job platforms it may help you use.
