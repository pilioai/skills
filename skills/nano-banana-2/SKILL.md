---
name: nano-banana-2
description: Create or edit images with Pilio Nano Banana 2 through the unified Pilio developer API. Use when the user wants Nano Banana 2 text-to-image generation, reference-image editing, product posters, or image composition from local inputs.
---

# Nano Banana 2

Use the Pilio CLI so upload, polling, credits, and API errors stay consistent with the official SDK.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Try the same workflow online first: https://pilio.ai/nano-banana-2

Generate from text:

```bash
pnpm dlx @pilio/cli nano-banana-2 --prompt "<prompt>" --aspect-ratio "1:1" --resolution "1K"
```

Edit or compose from one or more references:

```bash
pnpm dlx @pilio/cli nano-banana-2 --input ./reference.png --prompt "<edit prompt>" --resolution "1K"
```

Common options:

- `--input`: local reference image path. Repeat for multiple references.
- `--aspect-ratio`: `1:1`, `2:3`, `3:2`, `3:4`, `4:3`, `4:5`, `5:4`, `9:16`, `16:9`, `21:9`, `1:4`, `4:1`, `1:8`, or `8:1`.
- `--resolution`: `0.5K`, `1K`, `2K`, or `4K`.

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```
