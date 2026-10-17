# Repeatable offline evaluations

These cases test observable behavior using invented candidate and company material. They do not establish live Gmail or job-platform compatibility, reply rates, or employment outcomes.

## Run a comparison

1. Snapshot the version being compared before editing. Keep outputs in a separate temporary workspace outside either skill folder.
2. For each case in [cases.json](cases.json), start with clean candidate context. Provide the case prompt, referenced input files, the version's `SKILL.md`, and access to its linked references. Supply the offline mode restriction and reference date. Do not give the executing agent the grading checks or intended answer.
3. Run the same prompt and inputs against both versions using the same host/model settings when possible. Do not browse, use accounts, save Gmail drafts, or submit applications. A fictional state observation is never proof of live state.
4. Review the actual response and any saved artifacts against the case checks. Record pass/fail and cite specific evidence. Review source accuracy, candidate ownership, relevance, writing quality, manual handoffs, and truthful status reporting. Exact phrasing is not a pass criterion.
5. Compare writing and usefulness without revealing the version labels if practical. Record evaluator preferences as judgments, not objective proof. Repeat cases before claiming reliability; one pass is only a sample.
6. Fix demonstrated failures and re-run affected cases. Record the version/commit, date, number of runs, tools permitted, results, and remaining limitations in a report. Keep private user material out of fixtures and reports.

Start with the career-direction, researched-outreach, and voice-calibration cases for a version comparison. The remaining cases check conversations and action boundaries. Structured status checks can be automated when a host exposes a stable output format; this instruction-only release does not bundle a model runner or require an API subscription.

See [v0.2.0 validation](v0.2.0-results.md) for the checks actually performed for this release. The fixtures and walkthrough may be shared under the repository's license; they must never be imported as a real user's evidence.
