# AI Content Disclosure CG Minutes

## 10 August 2026

### Meeting Information
Scribe: David Weekly (compiled from Grain AI notes and transcript)

Attendees:
- David Weekly (co-chair)
- Anthony Allen (Comcast; first-time attendee, joined without prior context on the group)

Regrets/absent:
- Doğu Abaris (co-chair)
- Prof. Kalina Bontcheva (University of Sheffield; confirmed attendance the prior week per [#29](https://github.com/w3c-cg/ai-content-disclosure/issues/29), did not join)
- Sydney Cohen
- Luke Swartz
- Elijah

Attendance was very light — effectively an informal two-person conversation rather than a working session. None of the [posted agenda](https://github.com/w3c-cg/ai-content-disclosure/issues/35) items beyond a general walkthrough of the spec were reached. All substantive agenda items are being pushed to the mailing list for async discussion (see Action Items).

### Agenda review

As posted in [#35](https://github.com/w3c-cg/ai-content-disclosure/issues/35). With only one outside participant present — and one who arrived without background on the CG — the chair used the time to walk Anthony through the proposal from scratch rather than work the planned agenda.

### Spec walkthrough with Anthony Allen (Comcast)

- Covered the core proposal: an HTML attribute (`div`-level and similar) with three values — fully human-authored, AI-assisted (human reviewed), and AI-autonomous (no human review) — plus optional attributes for model/prompt provenance.
- **EU AI Act Article 50** framed as the key external driver: it requires AI-content identification but names no technical standard, leaving the gap this CG is trying to fill.
- Discussed **responsibility for attestation**: sits with the site author/publisher, not with W3C enforcement. CMS platforms would need to integrate the attribute into publishing workflows as a required field; MCP servers/agents assisting with CMS publishing should be guided to candidly self-identify the correct value.
- Revisited the **degree-of-involvement** question (percentage vs. primary-authorship framing) as still unresolved from prior calls — no new ground broken; the denominator problem (per character? per token? per "clever thought" in the prompt?) remains unanswered. See [#25](https://github.com/w3c-cg/ai-content-disclosure/issues/25).
- Discussed **verification vs. self-attestation boundaries**: the spec is deliberately arm's-length from verifying claims (e.g., proving "fully human" is algorithmically hard). Broader document-level provenance/confidence-in-claims is a related but explicitly separate problem the CG is not trying to solve.
- Discussed the **"slop era" framing**: AI content quality is improving quickly enough that intuitive detection will stop working, raising the stakes for machine-readable disclosure; also flagged the risk of circular evidence chains (human articles citing AI-generated sources that themselves cite AI-generated content) without traceable provenance markers.
- Anthony engaged substantively for a first-time, unprepared attendee; invited to join the mailing list and the W3C WebAI Interest Group.

### Not reached (carried to mailing list / September)

- EU AI Act Article 50 & Code of Practice discussion with Prof. Bontcheva — she did not attend despite confirming; re-engagement needed ([#28](https://github.com/w3c-cg/ai-content-disclosure/issues/28), [#29](https://github.com/w3c-cg/ai-content-disclosure/issues/29)).
- Governance: formalizing the Dogu → Sydney co-chair rotation.
- Ratification of [#31](https://github.com/w3c-cg/ai-content-disclosure/issues/31) (`ai-assisted` ⇒ human review & responsibility) — now unresolved across two consecutive calls; needs to move to async ratification regardless of meeting attendance.
- Boundary scenarios in [#34](https://github.com/w3c-cg/ai-content-disclosure/issues/34) (spell-check no-op, ignored AI suggestions, chat-then-manual-edit).
- Open PRs: [#20](https://github.com/w3c-cg/ai-content-disclosure/pull/20) author decision guide, [#21](https://github.com/w3c-cg/ai-content-disclosure/pull/21) `ai-evidence-url`.
- IETF companion draft `draft-abaris-aicdh` — expired 3 August 2026, still no path forward decided; its sole author (Dogu) is the co-chair who resigned.
- Outreach & tooling updates (IPTC, UL, Google/broader network, browser extension / CMS plugin work).

### Action items

- [ ] Chairs: post a mailing-list thread carrying the full 10 Aug agenda items (#28/#29 Bontcheva re-engagement, co-chair rotation, #31 ratification, #34 boundary scenarios, PR #20/#21 status, IETF draft path forward, outreach/tooling) for async discussion given two low-attendance calls in a row.
- [ ] Chairs: directly re-engage Prof. Bontcheva on the missed call and re-propose a date.
- [ ] Chairs: run async ratification of [#31](https://github.com/w3c-cg/ai-content-disclosure/issues/31) via the mailing list / issue comments rather than waiting on a call.
- [ ] Chairs: decide on the IETF draft (`draft-abaris-aicdh`) — refresh with new author(s) or let it lapse deliberately.
- [ ] David: follow up with Anthony Allen (Comcast) re: mailing list and WebAI IG introduction.
- [ ] Chairs: publish these minutes and send the mailing-list thread with open questions.

### Closing

- Adjourned. Given two consecutive under-attended calls, the chairs will shift primary decision-making to the mailing list/GitHub issues and treat the next monthly call as a checkpoint rather than the sole venue for progress.

