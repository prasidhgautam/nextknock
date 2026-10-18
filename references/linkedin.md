# LinkedIn opportunities and useful conversations

Use this workflow only after the user chooses LinkedIn and agrees the search brief. Read [platform assistance](platforms.md), [researched outreach](outreach.md), [private tracking](tracking.md), [agent coordination](coordination.md), and [monitoring](monitoring.md). Loading or installing this skill does not authorize applications, invitations, messages, purchases, or monitoring. A run needs an explicit scope: approved opportunities or search filters, allowed actions, selected account, time/volume limits, and any Premium credit budget. If sending was not requested, prepare the content for review.

## Check access and the actual account

Verify the chosen account before account actions. LinkedIn prohibits third-party software that automates activity on its site. Browser controls being available does not establish permission to automate LinkedIn. Default to user-performed LinkedIn submissions, invitations, messages, and acceptance checks, with specific prepared content and a clear handoff. Automate an operation only when an actual integration explicitly permits that particular operation for the account and the host allows it; ordinary browser UI access, an unofficial API, or the user's Premium subscription is insufficient. External applicant-tracking systems follow their own supported access and host action rules.

Do not scrape profiles, extract cookies, use hidden endpoints, bypass restrictions, evade rate limits, or invent a daily quota that supposedly makes prohibited automation safe. Research with permitted sources and user-supplied professional information. If profile information cannot be accessed appropriately, ask for the relevant profile link or context and record the coverage gap.

Check plan and current capabilities rather than inferring them from a badge. Observe whether a particular recipient can receive a regular direct message, Open Profile message, or InMail; whether that route is available for this account; and whether credits or other limits apply. Get the run's credit budget before any credit-consuming action. Never assume Premium means unlimited messaging or buy a subscription or credits.

## Complete each application independently

For each suitable opportunity in the authorized scope, record the actual company and job/requisition identity, current vacancy source, fit evidence, constraints, and chosen document version. An opportunity may use Easy Apply or an external employer/ATS form. Neither route is automatically better, and networking must not delay an otherwise ready application.

- **Easy Apply:** prepare role-specific materials and screening answers from candidate evidence. Hand off LinkedIn form entry and final submission when no explicitly permitted integration covers them. Provide the observed job reference and exact remaining steps. The user may confirm the result, but record `applied` only after an observed success screen, application record, or equivalent verifiable submission evidence; otherwise retain the confirmation as a report and use `needs_verification`.
- **External application:** follow the vacancy's actual employer/ATS destination through supported tools. Confirm the employer/requisition and current account, prepare the form, and submit only within the user's requested scope. Leave unknown personal facts, declarations, uploads, login, and verification blockers to the user as needed.

Use `application_prepared` when ready but unsent. Persist `submitting` before an authorized final action. Record `applied` only after observed confirmation, retaining its reference and time. An uploaded CV, review page, click, or interrupted session does not prove submission. Uncertain outcomes require `needs_verification` and inspection before retrying. Keep the networking state separate so an application can be confirmed while invitations remain prepared or blocked.

## Research the relevant people

For each opportunity, seek **2–3 people from the relevant functional department** and **1–2 relevant talent/HR people**, normally 3–5 unique contacts when enough evidence exists. Prefer seniority sufficient to plausibly influence this hire while staying close to the actual function, team, and geography. A team lead or department head may be more relevant than an unrelated executive. For talent contacts, look for evidence of responsibility for this function, location, business unit, or vacancy; a generic HR title does not prove recruiting ownership.

For each proposed person, save the verified professional profile reference, company identity, observed role/team, relevance to this opportunity, source/date, and a reason this person might care. Label hiring influence as an inference unless explicitly established. One person holding both functional and HR responsibilities counts once. Do not guess private email addresses or claim inside knowledge of hiring decisions.

These counts are research targets, not reasons to contact irrelevant people. Record how many suitable contacts were found and explain any shortfall; do not stall the application to fill the target. Tailor each approach to a distinct, evidenced connection. Do not ask several colleagues to arrange the same referral or forward the same message around a company.

Use one private contact record per verified professional profile, linked to all relevant opportunities. Canonicalize observed profile and company IDs/URLs without inventing missing IDs. Reconcile alternate profile URLs with evidence before merging. Deduplicate across jobs, recruiters, saved drafts, invitations, LinkedIn messages, Gmail, and other known channels. Repeated applications at one employer do not authorize repeated introductions to the same person.

## Select one initial contact route

Check current connection state, pending invitations, prior sent messages, replies, rejection/opt-out, and accessible cross-channel history before preparing an approach. Disclose unavailable history and resolve a material duplication risk with the user.

- **Already connected or direct messaging available:** prepare a relevant direct message for the actual context; no invitation is needed.
- **Premium/InMail/Open Profile route available:** prefer the supported direct route when appropriate and within the approved credit budget. Prepare one individual message, then perform the permitted action or hand off to the user. Record the actual route and confirmed credit use when visible. If eligibility or credits are unknown, resolve them before sending; do not assume a message went through.
- **Invitation needed:** prepare a lighter, personal connection note within the currently observed interface limits. Say why connecting is relevant without squeezing a full sales pitch into the note. Do not hard-code note length, invitation limits, or entitlement rules. If a note is unavailable, report that limitation and let the user choose an unnoted invitation or another permitted route.

Do not send an invitation, InMail, and email containing duplicate pitches to the same person. A pending invitation is not a reason to pursue the person through another channel without reconciling history and the user's scope. Record the selected route and prepared alternatives; alternatives are not additional scheduled sends.

Persist `invitation_prepared` before handoff; use `inviting` only when an authorized invitation action starts, and `invitation_sent` only after observed sent/pending state. Persist `message_prepared` before handoff, `messaging` before an authorized send, and `message_sent` only after observed sent evidence. If a user reports sending without verifiable state, retain that report, set `needs_verification`, and prevent duplicate retry. A prepared message, button click, or notification does not establish sending.

## Respond to an accepted connection

Keep watch only through the separate, explicit setup in [monitoring](monitoring.md); a tracker review date or a promise in conversation does not create a running watcher. At review time, check acceptance through an explicitly permitted source or ask the user to check LinkedIn manually.

A notification or user-provided acceptance alert is a signal: record `acceptance_reported` and its provenance until reconciled with the contact. Ambiguous identity stays in an unassigned event; do not pick a namesake, attach it to a guessed contact, or write an addressed acceptance pitch before matching the person. Unaddressed research notes may continue. Record `connection_accepted` after observed current connection state or the user's explicit confirmation of that specific accepted connection; retain the evidence type so a manual confirmation is distinguishable from observed state. Never mark acceptance from elapsed time or an invitation no longer appearing alone.

Before preparing a post-acceptance introduction, recheck messages and all linked opportunities. If an initial InMail, direct message, or email already introduced the candidate, acceptance must not trigger a second introduction. Read any reply first. If there has been no initial pitch, research the recipient and company and prepare a personal pitch. Reuse an existing scoped send authorization when it covers this contact, channel, and budget; ask only for genuinely missing scope. Sending still requires a permitted operation, otherwise hand it to the user. Acceptance itself does not expand the agreed scope.

Aim for roughly 60–120 words when useful; shorter messages may serve the conversation better. Use the candidate's voice and relevant evidence. Follow the research standard in [outreach](outreach.md): verify a meaningful company development from the preceding 12 months, including event date, or use a verified relevant product/business/role observation and disclose the research limitation to the user. Connect that observation to the recipient's work and one supported candidate example. A tentative idea must be labelled as such.

Every two or three lines, revise privately: **Why would this recipient care? What relevant proof or useful thought makes a reply worthwhile? Is the ask easy to answer?** Remove generic praise, copied introductions, pressure, exaggerated promises, fake familiarity, and irrelevant company news. Close with one simple question or invitation to talk. A departmental leader and a recruiter need different reasons to care; do not reuse the same finished pitch with only the name changed.

## Replies, follow-ups, and continuity

Handle substantive replies using [conversation support](conversations.md). Ask for missing availability, commitments, compensation, or documents rather than inventing them. A reply is a conversation signal, not proof of hiring interest.

Use the existing follow-up policy across channels and all linked opportunities: only an actual sent initial message starts the clock; check current replies first; respect a promised response date; stop after rejection, opt-out, or two unanswered sent follow-ups. Default review intervals are five business days after the sent initial message and seven after the sent first follow-up. An invitation alone, unsent pitch, or acceptance does not start a follow-up sequence. Apply a stop to its evidenced person, vacancy, or employer scope: a person's opt-out does not automatically represent the whole employer, but never approach colleagues to route a message back to that person or evade their request.

Maintain separate application, invitation/connection, and message actions under the opportunity/contact records. Preserve reported versus observed evidence, selected route, message text, actual timestamps, thread/reference, credit budget/use when applicable, blockers, and next review. Uncertain external actions always use `needs_verification`; verify before retrying. Report verified applications, prepared application handoffs, suitable contact coverage, prepared/sent invitations, reported/confirmed acceptances, prepared/sent messages, and manual steps separately.

## Platform references

Policy and feature guidance checked for this release on **18 October 2026**. Recheck current official guidance and the observed account interface when using the skill; eligibility, notes, and messaging entitlements can change.

- [LinkedIn official help: prohibited software and extensions](https://www.linkedin.com/help/linkedin/answer/a1341387)
- [LinkedIn official help: send an InMail message](https://www.linkedin.com/help/linkedin/answer/a546814)
- [LinkedIn official help: personalize invitations to connect](https://www.linkedin.com/help/linkedin/answer/a563153)
- [LinkedIn official help: messaging guidance](https://www.linkedin.com/help/linkedin/answer/a554575)
