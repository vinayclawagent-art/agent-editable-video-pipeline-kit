# Post-Trial Promotion Decision Card

Source: [[Agent-Edited Video as Text and Code Pipeline]]
Related packet: [[One-Minute Agent Video Trial Packet]]
Evidence manifest: [[Video Evidence Attachment Manifest]]

Use this card after the first real short-clip trial evidence is attached. It is a template-ready decision gate, not a validation claim.

## Decision inputs

- Filled trial packet:
- Filled evidence manifest:
- Reviewer / operator:
- Trial date:
- GitHub commit or artifact bundle:

## Evidence sufficiency check

| Question | Evidence link | Pass / fail / unknown | Notes |
|---|---|---|---|
| Can another operator rerender from text/code artifacts? | | | |
| Does the EDL explain every cut/overlay decision? | | | |
| Are `ffmpeg` / render commands captured enough to replay? | | | |
| Did verifier notes cover duration, captions, audio, and visuals? | | | |
| Was at least one revision possible without opening a timeline editor? | | | |

## Promotion decision

Choose one:

- [ ] **Promote** — repeatable enough to turn into an installed skill or scripted kit.
- [ ] **Pilot-only** — useful for VinClawLabs content, but needs one more constrained trial.
- [ ] **Iterate** — prototype works conceptually but evidence exposes missing steps.
- [ ] **Hold** — not enough proof or too much manual timeline work remains.

## Required follow-up patch

- README change justified by evidence:
- Prototype change justified by evidence:
- Skill-draft change justified by evidence:
- One open risk to preserve in backlog:

## Decision log entry to copy

```markdown
- YYYY-MM-DD: Completed first real short-clip trial decision. Outcome: <promote / pilot-only / iterate / hold>. Evidence bundle: <link>. Follow-up patch: <link or summary>.
```
