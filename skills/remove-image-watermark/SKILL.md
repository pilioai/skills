---
name: remove-image-watermark
description: Remove visible watermarks from an image with the Pilio developer API. Use when the user wants to clean a PNG, JPG, JPEG, or WEBP image, remove image watermark overlays, or automate image watermark removal through Pilio.
---

# Remove Image Watermark

Use the Pilio CLI so upload and asynchronous task polling are handled consistently.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Try the same workflow online first: https://pilio.ai/image-watermark-remover

Run:

```bash
pnpm dlx @pilio/cli remove-image-watermark --input ./watermarked.png
```

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```

Do not send the Pilio API key to result `download_url` values.
