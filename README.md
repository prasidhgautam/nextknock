# NextKnock

**Your next opportunity starts with a conversation.**

NextKnock is a reusable agent skill for exploring your next career step, preparing job-platform profiles, applying selectively, and drafting researched messages that give someone a reason to reply.

It is a folder of instructions for a capable agent, not a standalone application. It does not include a CV, candidate database, account access, or an email-sending service.

[Download v0.3.0](https://github.com/prasidhgautam/nextknock/releases/download/v0.3.0/nextknock-v0.3.0.zip) · [Try the fictional demo](examples/walkthrough.md) · [LinkedIn walkthrough](examples/linkedin-walkthrough.md) · [License](LICENSE) · [Permissions](LICENSE-NOTICE.md)

## What it helps you do

1. **Start with your evidence.** Share your CV and portfolio files or links. Build a private evidence bank that preserves sources, your actual responsibilities, and gaps. No portfolio? Continue with your CV.
2. **Choose a direction.** Compare suitable next steps, adjacent moves, and stretches with evidence, tradeoffs, and practical exploration steps. Agree on roles, location, working preferences, and constraints.
3. **Choose platforms.** Select the job platforms and Gmail account you want to use. Get help preparing existing profiles or establishing missing ones.
4. **Pursue suitable opportunities.** Research live vacancies and employers, explain fit, and prepare or submit applications within your requested scope.
5. **Write in your own voice.** Use an optional writing sample or choose between short examples. Draft concise outreach connecting a relevant company observation to your actual work and a useful reason to respond.
6. **Continue the conversation.** Prepare replies, relevant work examples, call briefs, and recaps from what was actually discussed. Keep availability and commitments under your control.
7. **Keep track and improve.** Separate confirmed submissions, saved Gmail drafts, replies, completed conversations, and manual steps. Review your edits and outcomes privately when requested.

For a scoped LinkedIn run, cover each suitable vacancy's Easy Apply or external form and research **2–3 relevant senior people in its department plus 1–2 relevant recruiting/HR people**. Prefer people close to the actual hiring team, explain inferred influence, and record shortfalls rather than contact unrelated executives. Shared contacts across vacancies have one history. Premium/Open Profile/InMail routes depend on actual eligibility, available credits, and the user's budget.

NextKnock divides substantial runs into application, research, writing, acceptance/reply review, and quality-check responsibilities under one coordinator. Hosts with subagent tools can delegate; other hosts use the same checklist sequentially. One coordinator reconciles state and controls account actions, reducing duplicate work and conflicting updates.

Emails remain **unsent Gmail drafts by default** for you to review and send. An unavailable upload, login, verification challenge, or unsupported control becomes an explicit manual step. NextKnock checks the result before resuming.

**LinkedIn execution:** its [published rules prohibit third-party site automation](https://www.linkedin.com/help/linkedin/answer/a1341387). LinkedIn submissions, invitations, messages, and connection checks therefore default to prepared materials and manual steps. An automated action needs a verified explicitly permitted integration for that specific operation; having browser controls or Premium is insufficient. This package includes no such integration. External employer forms use their own supported workflow.

## Install in Codex

1. Download the release ZIP above and extract it.
2. Copy the complete `nextknock` folder into `~/.agents/skills/`, so the manifest is at `~/.agents/skills/nextknock/SKILL.md`. For a project-only installation, use `.agents/skills/nextknock/` inside that project instead. If the destination exists, review or back it up before replacing it.
3. Invoke `$nextknock` in your next Codex prompt. If it does not appear, restart Codex.

You can also ask Codex's built-in `$skill-installer` to install the skill from the root of [this repository](https://github.com/prasidhgautam/nextknock).

To upgrade an existing installation, back up the installed `nextknock` folder, then replace it with the complete folder from the new ZIP. Keep your private `job-search` workspace separate; its evidence, preferences, and tracker can be used when you resume. Restart Codex if the update does not appear.

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

For LinkedIn preparation:

```text
Use $nextknock for these two LinkedIn opportunities. Prepare the applications and research 2–3 relevant department contacts and 1–2 recruiting contacts for each. Deduplicate shared people, show why each contact matters, and write individual notes in my voice. Give me the manual LinkedIn steps. Offer an acceptance/reply watch setup, but do not schedule anything until we agree on its source and timing.
```

## Acceptance and reply watching

When requested, help configure a bounded watch using an actually available scheduler and permitted source. A user-assisted connection check or authorized relevant email notifications can support the workflow; notifications require identity/state reconciliation. New confirmed acceptances can lead to researched individual pitches, while existing InMail/email contact and replies prevent duplicate introductions.

Before enabling a watch, agree on contacts, account/source, cadence, timezone, end date, and action scope. Record the real scheduler reference. Checks happen at the next successful configured interval, not instantly. Without scheduling or permitted source access, provide an honest manual check plan. Installing this skill does not enable monitoring, and this release does not start a watcher on your account.

## Try it without personal documents

Follow the [fictional walkthrough](examples/walkthrough.md) with the included [sample CV](examples/sample-cv.md) and [research packet](examples/research-packet.md). It shows career comparison, an outreach angle, and preparation for a reply. No login is needed; the demo uses local outputs only. All people, companies, and source excerpts in the demo are invented and must not be used as live evidence.

## What changed in v0.3.0

- LinkedIn application and hiring-team networking coverage for each suitable opportunity, with quality-based contact shortfalls.
- Distinct invitation, acceptance, InMail/direct-message, and application records, deduplicated across vacancies and channels.
- Recipient-specific pitches after confirmed acceptance, or eligible direct-message routes with checked credit budgets.
- Bounded acceptance/reply watch setup with source, scheduler, permission, and manual-fallback checks.
- Coordinated agent responsibilities, one canonical writer/action gate, and recovery from interrupted or uncertain actions.
- A fictional LinkedIn walkthrough and held-out scenario cases. Existing evidence, voice, career guidance, Gmail drafts, and conversation support remain available.

## Capabilities and accounts

The host agent needs document-reading tools for your supplied materials and live web research for current roles and company facts. Supported and permitted browser controls or platform connectors are needed for account and application actions. A Gmail connector or supported Gmail browser session is needed to save drafts in your chosen account. Real delegation tools are needed for multiple agents, and a supported scheduler plus permitted source are needed for background checks; both have explicit fallbacks.

There is no bundled runtime, MCP server, API key, or connector subscription. Any account, host, or tool requirements and charges belong to the services you choose. The skill cannot grant permissions or enable capabilities the host lacks. Without account access, it can prepare local materials and explain the manual steps.

## Privacy and boundaries

Provide your own current CV and authorized portfolio materials. Keep them, account details, preferences, trackers, and application history **outside this repository and the installed skill folder**. Do not submit personal documents or credentials in GitHub Issues.

The agent should use confirmed candidate evidence, leave unknown answers unresolved, ask you to complete credentials and personal declarations, and verify submissions before counting them. It does not bypass CAPTCHA or platform restrictions. Background checks require your scoped request and confirmed supported setup. No workflow guarantees replies, interviews, or employment. Review materials before sharing them.

## Files and validation

- `SKILL.md`: entrypoint and workflow boundaries.
- `agents/openai.yaml`: display metadata and invocation prompt.
- `references/`: onboarding, platform assistance, outreach, and tracking guidance.
- `examples/`: fictional CV, research packet, and walkthrough.
- `evals/`: repeatable fictional cases, comparison procedure, and release validation report.

See the [v0.3.0 validation report](evals/v0.3.0-results.md) for the tests actually run, observed results, and limitations, and the [v0.2.0 report](evals/v0.2.0-results.md) for earlier checks. The [evaluation guide](evals/README.md) describes how to repeat the cases. **Live execution against LinkedIn, other job platforms, Gmail, and scheduled monitors has not been verified.** Host capabilities and interfaces can change. Offline examples cannot establish reply rates or hiring outcomes.

For a small voluntary pilot, collect feedback privately: where users got stuck, substantial factual or voice edits, and observed conversation outcomes. Share only anonymous or fictional reproductions in [GitHub Issues](https://github.com/prasidhgautam/nextknock/issues). The skill contains no telemetry or background collection.

## License, credit, and commercial permission

The written skill materials are available under [CC BY-NC 4.0](LICENSE), with attribution to [@prasidhgautam](https://github.com/prasidhgautam). See [LICENSE-NOTICE.md](LICENSE-NOTICE.md) for the additional permission covering an individual's own job search, including paid employment.

Commercial use of the skill materials requires separate permission. To discuss commercial redistribution, paid services, or product integration, open a [commercial-permission inquiry](https://github.com/prasidhgautam/nextknock/issues). Opening an issue does not grant permission or establish a price. This is a public project with noncommercial licensing; it is not offered under an OSI-approved open-source license.

NextKnock is an independent community-created career skill and is not affiliated with similarly named recruiting firms, OpenAI, or the job platforms it may help you use.
