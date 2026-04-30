---
name: gpt-image-2-edit
description: Edit one or more reference images with Pilio GPT Image 2 through the Pilio developer API. Use when the user wants image-to-image editing, restyling, product-photo transformation, or prompt-based edits using local reference images.
---

# GPT Image 2 Edit

Use the Pilio CLI so file upload, task creation, polling, and result handling use the official SDK path.

Require `PILIO_API_KEY` in the environment. Do not ask the user to paste API keys into the conversation.

Run with one or more `--input` files:

```bash
pnpm dlx @pilio/cli gpt-image-2 edit --input ./reference.png --prompt "<edit prompt>"
```

For multiple references:

```bash
pnpm dlx @pilio/cli gpt-image-2 edit --input ./a.png --input ./b.png --prompt "<edit prompt>"
```

The CLI must send the API key only to Pilio `/v1` endpoints. Presigned upload URLs are handled internally without the Pilio API key.

