# Project Notes

## API Provider Migration

All notebook labs in this repo should use **Anthropic Claude** models via `aisuite`, not OpenAI.

When modifying or creating notebooks:
- Use `anthropic:claude-sonnet-4-5-20250929` (or newer Claude models) instead of `openai:gpt-4.1`, `openai:gpt-4o`, etc.
- The `aisuite` library handles provider routing via the `provider:model` prefix format
- The only required API key is `ANTHROPIC_API_KEY` in the `.env` file
- Install the Anthropic provider: `pip install 'aisuite[anthropic]'`
