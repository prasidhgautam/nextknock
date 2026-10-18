# One skill, coordinated responsibilities

Use these roles within NextKnock when a run spans applications, company/contact research, and outreach. The coordinator retains responsibility for complete coverage, factual accuracy, current permissions, and the final report. Delegation reduces omissions; it does not guarantee correctness or exactly-once delivery.

## Host capabilities and roles

Discover whether the current host exposes actual subagent/delegation tools. If available, create bounded work assignments using those tools within this installed skill. Do not create separate user chats, install additional skills, or claim parallel execution when the host does not support it. Respect concurrency limits: combine roles or run them in stages; all roles need not run simultaneously.

If delegation is unavailable, perform the same roles sequentially with explicit checkpoints. Report that a single agent used a role checklist. Only say an independent agent reviewed work when a separate agent actually did so.

| Role | Bounded responsibility and handoff |
| --- | --- |
| Coordinator/intake | Confirm candidate, evidence version, search brief, accounts, scope, limits, and allowed channels. Assign IDs/tasks; reconcile proposals; own the canonical tracker and all external actions. |
| Application specialist | Assess each distinct vacancy, map requirements to candidate proof, prepare form answers/materials, flag missing declarations, and propose a submission/manual step with evidence. Never submit directly. |
| Company/contact researcher | Verify the opportunity, company developments, recipient identity, department and hiring relevance; return source/event dates and proposed contacts. Seek 2–3 relevant functional contacts and 1–2 HR contacts per LinkedIn opportunity, or explain shortfalls. |
| Message writer | Draft individual invitations, initial pitches, or replies using approved evidence, verified research, the user's voice, and channel limits. Explain privately why this recipient would care. Never send or save in an account directly. |
| Acceptance/reply watcher | Read only the authorized contact/thread scope when a check is due; propose observed acceptance/reply updates, suppressions, and eligible next drafts. Do not send, write the canonical tracker, or imply that a future date schedules a check. |
| Independent QA | Review claims, recipient relevance, messages, action eligibility and coverage. Return pass/repair/block decisions with reasons; propose corrections without executing account actions. |

Senior titles alone do not establish hiring influence. Prefer people whose current department and responsibilities relate to the role. Describe influence as inferred unless verified; do not choose unrelated executives merely for seniority.

## Narrow assignments and private outputs

Give each worker the approved task scope, opportunity/contact IDs, current evidence version, necessary source excerpts or evidence IDs, and only the account/history state required for that task. Avoid distributing an entire CV, portfolio, inbox or unrelated conversations when a relevant excerpt suffices. Candidate data and worker outputs belong in the user's private workspace, outside the installed skill and distributable archive.

Assign each worker a distinct private task output path. Workers may write only their assigned proposal output; the coordinator is the sole writer of the canonical tracker and ledger. Each handoff must include:

- Task, opportunity and contact IDs; candidate evidence/source version used.
- Claim-to-source mappings, with candidate ownership distinguished from team results and research interpretations.
- Prepared materials and proposed status; observed evidence and timestamps separated from recommendations.
- Uncertainties, blockers, omitted targets with reasons, and the next required step.

Do not let worker completion imply an application, invitation or message was sent. Reconcile every proposal against the current canonical state before accepting it. Preserve user edits; a change to candidate evidence/version, role, recipient, thread or source validity invalidates affected prepared text until rechecked.

## One external-action gate

Only the coordinator executes external mutations, including saved account drafts, form submission, invitations and messages. Do not run two browser writers or concurrent shared-account actions. Watcher proposals and other workers use the same gate; they cannot independently act on an acceptance.

For every proposed action, the coordinator must:

1. Reconcile current account identity, authorized scope, recipient/job identity, canonical records, actual platform state, relevant replies and cross-channel history. Confirm that this action is permitted through the selected integration. LinkedIn prohibits bots/automated website activity: default to manual LinkedIn completion unless an explicitly permitted integration for this exact action is verified. Browser control or a connected account alone is not permission. See [LinkedIn assistance](linkedin.md).
2. Check and claim a stable action key in the private ledger before acting: application = account + actual job/requisition; invitation = account + canonical recipient profile; initial pitch = account + canonical recipient profile across channels and opportunities. Distinct opportunities retain separate coverage rows, but do not earn duplicate invitations or initial pitches. Associate a shared contact/action with every relevant opportunity instead.
3. Persist the exact intent, current claim, permitted channel, prepared content/material versions and target before the action. Apply QA and scope checks to the final content; an earlier draft review does not cover later changes.
4. Execute the one permitted action, or hand the exact manual step and prepared materials to the user. Record observed confirmation afterward. Prepared text, a click, worker success or elapsed time does not prove an external result.

If a timeout, session interruption or worker crash leaves the result uncertain, record `needs_verification` and preserve the claim and intent. Do not assume failure and retry. On restart, reconcile outstanding claims, current records and actual application/invitation/message state before proceeding. If history cannot be checked, retain the blocker and ask for the precise manual verification. This workflow reduces duplicates; it cannot promise exactly-once actions across external platforms.

For simultaneous foreground and scheduled sessions, a read-then-write check is not an atomic lock. Use the host's supported exclusive ownership or transaction mechanism if available. Without one, monitoring remains read-only/proposal-only and the active coordinator serializes canonical updates and actions. Never treat expiry of a lock or claim as proof an external action did not happen.

## Review and complete coverage

QA must check candidate claims and ownership against approved evidence; company source/event recency; recipient identity, current role and hiring relevance; the reason this particular recipient would care; channel/content limits; account, scope and permission; current action claims and cross-channel duplicates; and whether reported results match actual verification. Uncertain influence, missing research, unavailable tools and unresolved facts stay explicit. Reject generic flattery, invented familiarity and unsupported promises.

Every opportunity needs separate application and networking records, even when blocked, skipped with a stated reason, or sharing existing contacts. Do not silently omit networking because the application is incomplete, or imply a sent invitation because it was prepared. End each run with a coverage matrix containing:

- Job/opportunity ID and application state with confirmation or manual blocker.
- Functional contacts: target 2–3, selected count and specific shortfall; HR contacts: target 1–2, selected count and shortfall.
- Per-contact invitation or permitted direct-message state, reused action references, acceptance state and last actual check.
- Research/pitch readiness, replies, exclusions/opt-outs, blockers and exact next steps.
- Next review dates and whether any supported monitoring was actually scheduled; a stored date alone schedules nothing.

Use [monitoring](monitoring.md) for active checks and separately authorized supported scheduling, [tracking](tracking.md) for canonical records and uncertain outcomes, and [outreach](outreach.md) for research, writing and follow-up rules. Report whether QA was independently reviewed or performed as the same agent's sequential checklist. Humanize messages through useful specificity and respect for the recipient's time, while keeping every claim supportable.
