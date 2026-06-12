---
name: agent-editable-video-pipeline
description: Turn raw video into agent-editable transcript, JSON EDL, ffmpeg/Remotion commands, render logs, and verification evidence.
status: draft
source_note: "[[Agent-Edited Video as Text and Code Pipeline]]"
---

# Agent Editable Video Pipeline

## When to use

Use when a repeatable video/content workflow should be edited by agents as text and code rather than through an opaque timeline editor.

## Steps

1. Collect raw footage/audio, script, design assets, and target duration.
2. Generate a word-level transcript.
3. Ask an agent to mark candidate cuts in a JSON edit decision list.
4. Convert EDL into `ffmpeg` cut/audio commands.
5. Add Remotion overlays or motion graphics for structured visuals.
6. Render the draft.
7. Verify duration, captions, audio clipping, visual defects, and rerenderability.
8. Save transcript, EDL, commands, render log, and verifier output as evidence.

## Promotion gate

Promote this to an installed Hermes skill only after one real clip is successfully rerendered from saved text/code artifacts.

## Pitfalls

- Do not claim validation from a template-only run.
- Keep large media outside the vault/repo; commit pointers, manifests, and logs.
- Require a verifier pass before treating the result as shippable.
