---
name: gpt-image-2
description: Create or edit images with Pilio GPT Image 2 through the unified Pilio developer API. Use when the user wants text-to-image generation, prompt-based image editing, restyling, product-photo transformation, or composition from one or more local reference images.
---

# GPT Image 2

Use the Pilio CLI so upload, polling, credits, and API errors stay consistent with the official SDK.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Try the same workflow online first: https://pilio.ai/

Generate from text:

```bash
pnpm dlx @pilio/cli gpt-image-2 --prompt "<prompt>" --aspect-ratio "1:1"
```

Edit or compose from one or more references:

```bash
pnpm dlx @pilio/cli gpt-image-2 --input ./reference.png --prompt "<edit prompt>"
```

Common options:

- `--input`: local reference image path. Repeat for multiple references.
- `--aspect-ratio`: `1:1`, `3:2`, `2:3`, `3:4`, `4:3`, `4:5`, `5:4`, `16:9`, `9:16`, `21:9`, or `auto`.
- `--quality`: `low`, `medium`, or `high`.
- `--resolution`: `0.5K`, `1K`, `2K`, or `4K`.

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```
