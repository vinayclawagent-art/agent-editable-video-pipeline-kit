# Video Evidence Attachment Manifest

Source: [[Agent-Edited Video as Text and Code Pipeline]]
Related packet: [[One-Minute Agent Video Trial Packet]]

Use this manifest after the first one-minute video edit trial. It prepares the evidence bundle without claiming the trial has happened.

## Trial identity

- Trial date:
- Raw clip path / source:
- Target output:
- Agent or operator:
- Renderer / runtime:

## Required attachments

| Evidence item | File/link | Reviewer note | Ready? |
|---|---|---|---|
| Source clip metadata | | | [ ] |
| Word-level transcript | | | [ ] |
| JSON edit decision list | | | [ ] |
| `ffmpeg` cut command log | | | [ ] |
| Remotion or overlay code diff | | | [ ] |
| Render log | | | [ ] |
| Draft MP4 path | | | [ ] |
| Verifier notes: duration/captions/audio/visual | | | [ ] |
| Re-render or revision attempt notes | | | [ ] |

## Reproducibility gate

| Gate | Evidence to inspect | Pass / fail / unknown | Patch needed |
|---|---|---|---|
| Another operator can rerender from text/code | EDL + commands + render log | | |
| Captions align with final cut | transcript + verifier notes | | |
| Audio is not clipped | verifier notes | | |
| Visual edits match intent | MP4 + EDL reasons | | |
| Timeline editor was not required for revision | revision attempt notes | | |

## Decision handoff

- Promote / iterate / hold:
- One README, skill-draft, or prototype patch justified by evidence:
- One thing not proven yet:
- Link to filled trial packet:
