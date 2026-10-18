# Private continuity and verified outcomes

## Storage and candidate separation

Use a private `job-search` directory in the user's active workspace, outside the installed skill, as the default. If that path would fall inside the skill/package, or no writable workspace exists, ask for a suitable location; keep the current report in the conversation meanwhile. For more than one candidate, use separate user-selected directories and account contexts. Do not automatically import another person's state or unrelated inbox history.

Keep a local Markdown tracker plus an append-only JSONL activity ledger. Add a compact preferences/evidence record as needed. Save only the candidate facts, sources, confirmed preferences, account choice, and action records needed to resume. Unknowns stay unknown. Never save credentials, cookies, verification codes, or unrelated mail. Do not copy full candidate files unless needed and authorized; reference the current supplied source and version instead.

Use the [evidence bank and voice preferences](evidence-and-voice.md) as the reusable candidate context. Link opportunity assessments and private draft notes to evidence IDs. On resume, confirm changed source versions, direction, and material constraints; do not repeat settled intake or treat stale sources as current.

A user may select a connected tracker. Use that exact tracker and preserve their edits. Local snapshots do not override its current state. Do not require a particular spreadsheet provider, hard-coded URL, approval column, or external helper script. When exporting the reusable skill, exclude all runtime state and candidate materials.

For delegated work, follow [coordination](coordination.md): workers write separate private proposals, and one coordinator owns the canonical tracker/ledger and external actions. Record source versions, stable action keys, claim owner/state, intended content, confirmation, and unresolved operations. An interrupted worker or elapsed claim is not evidence an operation failed. Concurrent sessions need supported exclusive ownership/atomic coordination; if unavailable, scheduled workers return read-only proposals and the active coordinator reconciles them sequentially.

## Minimum useful records

For each opportunity, keep a stable ID, observed job ID/URL when available, company, role, location/work mode, fit and reason, research sources/dates, current status, application confirmation, contact/draft/thread references, latest received reply, last actual outbound contact, sent follow-up count, next review date, and unresolved facts/manual steps.

For LinkedIn opportunities, keep application state separate from contact coverage (2–3 functional and 1–2 recruiting/HR targets, actual unique contacts, role labels and shortfalls). One person may hold two roles but counts once in the unique total. A shared person has one account/profile-keyed contact record linked to multiple opportunities. Record company, observed role, hiring-relevance evidence/inference, sources, selected messaging route, current connection/pending-invite state, prior initial-pitch action, credit requirement/use, stop reason, and last reconciliation. Do not sum overlapping category counts into a fabricated unique total.

For [monitoring](monitoring.md), record the private watchlist, verified data source/account, actual scheduler/task reference, cadence, timezone, end time, confirmed action/notification scope, last attempted check, last successful check, next due check, and access blockers. Preserve acceptance signal provenance (`acceptance_reported`) separately from confirmed connection state (`connection_accepted`). Ambiguous signals stay as unassigned events, without selecting a contact or preparing an addressed acceptance pitch. A direct manual confirmation from the user is labelled user-confirmed, not independently observed. Missing pending invitations, elapsed time, and notification text alone do not prove current connection state. A real human reply takes precedence over a new pitch.

For each message, keep a stable ID, associated opportunity, action type, verified account and recipient, subject, exact current draft text, intended attachments/version, draft/thread references, status, and observed timestamps. Mark summaries of received messages as summaries; never present generated text as a verbatim reply.

Append meaningful transitions with an ISO timestamp including timezone, record ID, action, previous/new status, observed evidence, and next step. Preserve historical sent text and actual received replies. Update unsent draft records without rewriting history or user notes. Reconcile draft IDs, account identity, relevant history, and external state before resuming.

## Status meanings

| Status | Meaning |
| --- | --- |
| `researched` / `skipped` | Reviewed opportunity; no application implied. |
| `application_prepared` | Form/materials ready; submission unconfirmed. |
| `submitting` | Final submission is about to occur or is in progress. |
| `applied` | Observed success screen or application record. |
| `draft_prepared` | Complete message exists locally; not saved in Gmail. |
| `drafting` | Gmail draft creation is about to occur or is in progress. |
| `draft_saved` | Confirmed Gmail draft; still unsent. |
| `needs_user_input` | A required candidate answer is missing. |
| `needs_manual_intervention` | A recorded step requires the user's action. |
| `needs_verification` | External result is uncertain; inspect before retrying. |
| `failed` | Failure confirmed; record whether/how it can be resumed. |
| `sent` | Actual sent state observed, including messages sent manually. |
| `replied` | Human reply observed; record content/context and next action. |
| `contact_researched` | A role-relevant contact is supported by identified sources; no invitation/message implied. |
| `invitation_prepared` / `inviting` | Connection request ready / one authorized permitted invitation action in progress. |
| `invitation_sent` | Actual pending/sent invitation confirmed; still not an accepted connection. |
| `acceptance_reported` | Acceptance signal recorded with provenance; identity/current connection reconciliation pending. |
| `connection_accepted` | Connection acceptance established through a permitted observation or explicit user confirmation, with evidence type retained. |
| `message_prepared` / `messaging` | Local LinkedIn message ready / one authorized permitted send in progress. |
| `message_sent` | Actual sent LinkedIn/InMail message confirmed; record channel, content, and thread. |
| `stopped` | Contact excluded by rejection, opt-out, closure, or exhausted follow-ups; retain the reason. |

Retain the underlying prepared/draft status when an item has a manual blocker, so a saved draft with a missing attachment is visible as both saved and incomplete. Record rejection, closure, withdrawal, opt-out, and conversation/interview stages as observed outcomes. An automated acknowledgement is not a human reply or shortlist.

`submitting`, `drafting`, `inviting`, `messaging`, and `needs_verification` require checking external state before repetition. Persist intent before the external action and confirmation afterward; an interrupted session is never evidence of failure. Deduplicate by actual job/requisition, company/role/location, recipient, and cross-channel history without merging distinct vacancies.

## End-of-run report

Report verified applications, confirmed Gmail drafts, locally prepared messages, observed replies/conversations, and incomplete steps separately. Include useful sources and real references, a few skip reasons, and one bundled request for missing facts if necessary. State any limits in access or history coverage. Future review dates are reminders in the tracker, not automatic monitoring or scheduled sends.

## Learn from use when requested

Keep feedback private and optional. Record where the user needed help, substantial factual or voice edits, and their own estimate of time saved if supplied. Do not invent time savings or upload analytics. Ask whether a wording edit should become a recurring preference before applying it broadly when that is unclear.

When reviewing outreach outcomes, distinguish automated acknowledgements, human replies, relevant conversations, interviews, and rejections. If a reply rate is useful, report the observation window and numerator/denominator: unique initial outreach threads with a human reply divided by unique verified sent initial outreach threads in the same cohort. Do not count unsent drafts, follow-ups as new initial contacts, or duplicates. Unknown sent/history coverage means the rate is incomplete. Show counts and avoid conclusions from a small or unevenly aged sample. Outcomes alone do not prove the skill caused an improvement.
