---
name: nano-banana-pro
description: Create or edit premium images with Pilio Nano Banana Pro through the unified Pilio developer API. Use when the user wants high-quality text-to-image generation, reference-image editing, product posters, campaign visuals, or image composition from one or more local reference images.
---

# Nano Banana Pro

Use the Pilio CLI so upload, polling, credits, and API errors stay consistent with the official SDK.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Try the same workflow online first: https://pilio.ai/nano-banana-pro

Generate from text:

```bash
pnpm dlx @pilio/cli nano-banana-pro --prompt "<prompt>" --aspect-ratio "1:1" --resolution "4K"
```

Edit or compose from one or more references:

```bash
pnpm dlx @pilio/cli nano-banana-pro --input ./reference.png --prompt "<edit prompt>"
```

Common options:

- `--input`: local reference image path. Repeat for multiple references.
- `--aspect-ratio`: `1:1`, `3:2`, `2:3`, `3:4`, `4:3`, `4:5`, `5:4`, `16:9`, `9:16`, or `21:9`.
- `--resolution`: `1K`, `2K`, or `4K`.
- `--output-count`: `1`, `2`, or `4`.

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```
