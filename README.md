# Pilio Skills

Agent skills for Pilio developer API workflows.

Install one function at a time:

```bash
pnpm dlx skills add pilioai/skills --skill gpt-image-2-generate
pnpm dlx skills add pilioai/skills --skill remove-background
```

Each skill is intentionally small and delegates API execution to `@pilio/cli`:

```bash
pnpm dlx @pilio/cli <command>
```

Set `PILIO_API_KEY` in the local environment before running the CLI. Do not paste real API keys into prompts or skill files.

