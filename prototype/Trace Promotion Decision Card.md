# Trace Promotion Decision Card

Status: template-ready; no validation proof recorded yet.

Package: [[Browser Debug Trace Harness]]  
Source packet: [[Browser Debug Trace Harness/Browser Debug Trace Packet]]

## When to fill this
Use this card only after the Browser Debug Trace Packet has been filled on one real broken local web page or app surface. Do not infer success from the template alone.

## Evidence links
| Required proof | Link / path | Notes |
|---|---|---|
| Broken page/app URL or repo path |  |  |
| Repro steps and baseline console/network/performance evidence |  |  |
| Patch diff or agent transcript |  |  |
| After-state console/network/performance evidence |  |  |
| Screenshot, trace export, or screen recording |  |  |
| Human reviewer note |  |  |

## Decision gate
Choose exactly one after evidence is attached.

- [ ] **Promote skill draft** — repeatable setup, clear browser evidence, and lower debugging time on a real issue.
- [ ] **Pilot-only** — useful for one class of bugs, but needs narrower triggers or safer guardrails.
- [ ] **Iterate packet** — evidence was incomplete, setup was brittle, or scorecard missed a critical failure mode.
- [ ] **Hold** — browser trace access did not materially improve the debugging workflow.

## Promotion criteria
| Criterion | Pass/Fail | Evidence link |
|---|---|---|
| CDP/browser setup was reproducible from the packet |  |  |
| Before/after state is independently inspectable |  |  |
| Agent/operator stayed within allowed files and app scope |  |  |
| The trace changed the debugging decision, not just the writeup |  |  |
| Skill draft has clear triggers and pitfalls after the trial |  |  |

## Follow-up patch queue
- [ ] Patch `Artifacts/Skills/agent-browser-debugging-harness/SKILL.md` with trial-backed pitfalls.
- [ ] Update the package README with the real evidence summary.
- [ ] Add a filled example only if all source links are present.
- [ ] Update [[Browser Debug Trace Harness Loop]] with the final promote / pilot-only / iterate / hold result.

## Guardrail
Do not mark the harness validated, proven, or promotion-ready until every claim above points to a packet row, log, screenshot, trace export, repo diff, or reviewer note.
