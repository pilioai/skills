# Pilio Skills

Agent skills for Pilio developer API workflows.

Install one function at a time:

```bash
pnpm dlx skills add pilioai/skills --skill gpt-image-2
pnpm dlx skills add pilioai/skills --skill nano-banana-pro
pnpm dlx skills add pilioai/skills --skill remove-background
```

Each skill is intentionally small and delegates API execution to `@pilio/cli`:

```bash
pnpm dlx @pilio/cli <command>
```

Set `PILIO_API_KEY` in the local environment before running the CLI. Do not paste real API keys into prompts or skill files.

## Try online

Use the hosted Pilio tools to test the same workflows in a browser before delegating them to an agent:

- [GPT Image 2](https://pilio.ai/)
- [Nano Banana Pro](https://pilio.ai/nano-banana-pro)
- [Image watermark remover](https://pilio.ai/image-watermark-remover)
- [Background remover](https://pilio.ai/background-remover)
- [Image upscaler](https://pilio.ai/image-upscaler)
- [PDF watermark remover](https://pilio.ai/pdf-watermark-remover)
- [Developer documentation](https://pilio.ai/developers)
