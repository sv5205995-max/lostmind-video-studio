# LOSTMIND Automation

## Purpose
Plan the automation layer connecting Telegram, n8n, and the LOSTMIND core engine.

## Planned Components
- Telegram Bot: receive commands and return status messages.
- n8n: orchestrate workflows and connect services.
- LOSTMIND Core: validate requests and route them to the correct module.
- Shared Renderer: produce the final video when the required assets are available.
- Human Review: approve the output before publishing.

## Planned Commands
- /start — show the welcome message and available commands.
- /help — explain how to use the bot.
- /rawvideo — start the raw-video editing workflow.
- /faceless — start the faceless Reels workflow.
- /explorer — start the cinematic explorer workflow.
- /status — show the current job status.

## Workflow Outline
1. Receive a Telegram command.
2. Validate the command and required inputs.
3. Start the corresponding n8n workflow.
4. Track the job and report progress.
5. Send the generated video or a result link when available.
6. Require human approval before publishing.

## Security
- Keep bot tokens, API keys, and passwords out of GitHub files.
- Store credentials in n8n credentials or environment variables.
- Validate user input and restrict bot access where needed.
- Do not publish or spend money without the configured approval rules.

## Current Status
Planning only. The Telegram Bot, n8n workflows, credentials, and integrations have not yet been implemented or tested.

## Next Steps
1. Create a Telegram bot using BotFather.
2. Set up an n8n instance.
3. Connect Telegram to n8n.
4. Test a simple /start or /help workflow.
5. Add LOSTMIND module routing and job-status updates.
