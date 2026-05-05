---
name: remove-pdf-watermark
description: Remove watermarks from a PDF with the Pilio developer API. Use when the user wants PDF watermark removal, editable PDF cleanup, AI PDF page reconstruction, or automated PDF watermark processing through Pilio.
---

# Remove PDF Watermark

Use the Pilio CLI so PDF upload, asynchronous task creation, and polling use the official SDK path.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Try the same workflow online first: https://pilio.ai/pdf-watermark-remover

Run:

```bash
pnpm dlx @pilio/cli remove-pdf-watermark --input ./watermarked.pdf
```

Optional mode:

```bash
pnpm dlx @pilio/cli remove-pdf-watermark --input ./watermarked.pdf --mode editable
pnpm dlx @pilio/cli remove-pdf-watermark --input ./watermarked.pdf --mode ai
```

The command returns a task payload. If the task is still pending or processing, wait for it:

```bash
pnpm dlx @pilio/cli task wait <task_id>
```
