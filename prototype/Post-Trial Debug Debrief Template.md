# Post-Trial Debug Debrief Template

Status: template-ready; no browser-debugging validation proof recorded yet.

Package: [[Browser Debug Trace Harness]]  
Inputs: [[Browser Debug Trace Harness/Browser Debug Trace Packet]] + [[Browser Debug Trace Harness/Trace Promotion Decision Card]]

## When to fill this
Use this after a real broken local web page or app-screen debugging trial has been run and the trace packet plus promotion card contain evidence links. The goal is to convert proof into specific patch decisions, not to invent a success story.

## Trial evidence snapshot
| Field | Filled value / link |
|---|---|
| Broken page/app and repo path |  |
| Baseline console/network/performance artifacts |  |
| Patch diff or agent transcript |  |
| After-state console/network/performance artifacts |  |
| Screenshot, trace export, or recording |  |
| Reviewer verdict |  |

## What changed because browser traces existed?
| Question | Evidence-backed answer |
|---|---|
| Which trace signal changed the debugging decision? |  |
| Which symptom would have been missed without browser access? |  |
| What was slower or brittle in the packet? |  |
| Which claim is now safe to make in README/prototype/skill text? |  |
| Which claim must stay unmade until another trial? |  |

## Patch decisions
Check only items backed by the evidence above.

- [ ] Update `Artifacts/Generated-Packages/Browser Debug Trace Harness/README.md` with a concise evidence summary.
- [ ] Patch `Artifacts/Prototypes/Browser Debug Trace Harness/Browser Debug Trace Packet.md` if fields were missing or confusing.
- [ ] Patch `Artifacts/Skills/agent-browser-debugging-harness/SKILL.md` with trial-backed triggers and pitfalls.
- [ ] Add a filled example note with all source links attached.
- [ ] Keep the artifact template-only; evidence was insufficient for any claim changes.

## Decision record
- Final decision: promote / pilot-only / iterate / hold
- Evidence links supporting the decision:
  - 
- Follow-up owner / next run action:
  - 

## Guardrail
If the trial lacks before/after trace artifacts, a patch diff/transcript, and a human or replay verdict, this debrief may only record gaps. It must not upgrade the package status or skill claims.
