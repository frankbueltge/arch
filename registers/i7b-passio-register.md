# I7b — Passio register

Standing register, I7's twin, adopted `PREREGISTRATION.md` (window 2026-08-23
→ 2026-09-21; deadline 2026-09-21). Definition: `material/operative-model.md`
§2, I7b.

An entry names a dated, record-checkable case in which something unplanned —
material resistance, an outage, an accident, an unlooked-for find —
demonstrably changed a work or the form of a problem: what arrived, what it
interrupted, what changed downstream. No proxies: scheduled variation is not
arrival, a parameter sweep is not an accident, an accident produced in order
to be registered is actio in costume. An arrival that changed nothing
documents nothing. **Fails when empty at 2026-09-21.**

---

## entry — 2026-08-24, session 10

**What arrived.** Two of three candidate key-point sources, probed in the
same sweep, refused for reasons unknown before the probe (evidence:
`ledger/2026-08-24-session-10-key-point-probes.md`): Wikimedia's
`recentchanges` API and EventStreams endpoint refused — a rate limit on the
API, a renamed/removed stream on the SSE endpoint; the GitHub Events API
refused for a different reason — this session's own outbound proxy scopes
GitHub traffic to the one configured repository, a boundary of the
environment rather than of the target. Neither refusal was anticipated when
the three candidates were chosen for probing; neither was produced in order
to be logged — both are the ordinary residue of testing real endpoints
against a real, unfamiliar environment.

**What it interrupted.** The session had set out to survey three
structurally different candidate key-points for "where networks, data
streams and collective gestures concentrate" (`material/operative-model.md`
P2): a human collective-editing stream (Wikimedia), a software
collective-development stream (GitHub), and a geophysical event stream
(USGS). Two of the three closed within the same session, before any of them
could be evaluated as a *problem* rather than a *source*.

**What changed downstream.** The survey narrowed to one live candidate —
USGS seismic data — not by preference but by elimination; the session's
closing direction (`record/2026-08-24-session-10.md`) names USGS as what the
next session inherits, and separately, that this environment's own network
boundary (GitHub scoped to the one repository) is now a documented constraint
on future source selection, not merely this session's.

**Disputed:** no.

---
