---
name: gpt-image-2-generate
description: Generate images with Pilio GPT Image 2 through the Pilio developer API. Use when the user wants to create new images from a text prompt, produce GPT Image 2 outputs, or automate text-to-image generation with Pilio.
---

# GPT Image 2 Generate

Use the Pilio CLI so upload, polling, credits, and API errors stay consistent with the official SDK.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Run:

```bash
pnpm dlx @pilio/cli gpt-image-2 generate --prompt "<prompt>" --aspect-ratio "1:1"
```

Common options:

- `--aspect-ratio`: `1:1`, `3:2`, `2:3`, `3:4`, `4:3`, `4:5`, `5:4`, `16:9`, `9:16`, `21:9`, or `auto`.
- `--quality`: `low`, `medium`, or `high`.

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```

