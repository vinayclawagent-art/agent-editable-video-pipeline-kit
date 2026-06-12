# One-Minute Agent Video Trial Packet

Source: [[Agent-Edited Video as Text and Code Pipeline]]

A smallest-useful trial for proving that an agent can edit video as text/code without fabricating success.

## Inputs

- Raw clip path:
- Desired final length: 60 seconds
- Transcript path:
- Brand/design assets:
- Output format:

## Pipeline checklist

- [ ] Generate word-level transcript.
- [ ] Mark best takes / cuts in a JSON edit decision list.
- [ ] Produce `ffmpeg` cut commands.
- [ ] Add one Remotion lower-third or motion graphic.
- [ ] Render draft MP4.
- [ ] Run verifier: duration, captions, jump cuts, audio clipping, visual defects.
- [ ] Save the EDL, commands, and render log as review evidence.

## JSON EDL skeleton

```json
{
  "source": "raw/input.mp4",
  "target_duration_seconds": 60,
  "clips": [
    {"start": 0.0, "end": 8.5, "reason": "hook"}
  ],
  "overlays": [
    {"type": "lower-third", "text": "Product demo", "start": 1.0, "end": 5.0}
  ],
  "verification": {
    "duration_ok": null,
    "captions_ok": null,
    "audio_ok": null,
    "visual_defects": []
  }
}
```

## Pass/fail gate

Pass only if another agent/operator can rerender or revise the video from the saved text/code artifacts without opening a timeline editor.
