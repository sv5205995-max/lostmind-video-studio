# LOSTMIND Video Studio

A modular, free-first project for planning and building AI-assisted video editing and Reels automation.

## Project Goal
Build a system that can help prepare vertical videos through reusable workflows, shared rendering tools, and human review.

## Core Workflows

### 1. Raw Video Editing
- Transcribe recorded video
- Plan cuts and captions
- Organize B-roll and sound design
- Render a vertical MP4

### 2. Faceless AI Reels
- Develop a topic and script
- Prepare scenes and visual assets
- Add voiceover, captions, and audio
- Render a vertical MP4

### 3. Cinematic Explorer Reels
- Establish the environment before revealing a mystery
- Use believable explorer-style footage and natural camera movement
- Build suspense gradually with environmental sound
- Render a vertical MP4

## Planned Architecture
Telegram Bot → n8n Automation → LOSTMIND Core → Selected Workflow → Shared Renderer → Human Review

## Repository Structure
- `docs/` — project documentation
- `modules/raw-video/` — raw-video workflow plan
- `modules/faceless-reels/` — faceless Reels workflow plan
- `modules/cinematic-explorer/` — cinematic explorer workflow plan
- `renderer/` — shared rendering plan using HyperFrames and FFmpeg
- `automation/` — Telegram and n8n automation plan

## Planned Technology
- GitHub — source control and project documentation
- Telegram Bot — command interface
- n8n — workflow orchestration
- HyperFrames — video composition and graphics
- FFmpeg — video and audio processing
- Optional AI services — transcription, script generation, voiceover, and visual assets

## Design Principles
- Start with free or low-cost tools where practical
- Keep the modules separate and reusable
- Protect API keys and credentials
- Use properly licensed or user-owned media
- Require human review before publishing

## Current Status
Documentation and project planning stage. The modules, integrations, rendering scripts, and automated publishing are not yet implemented or verified.

## Development Roadmap
1. Finish the project structure and documentation.
2. Prepare the development PC and install required tools.
3. Build and test a minimal rendering workflow.
4. Connect Telegram to n8n.
5. Implement and test each video workflow separately.
6. Add output validation and human approval.
7. Add publishing integrations only after successful tests.

## Security
Never commit API keys, bot tokens, passwords, or private credentials to this repository.
