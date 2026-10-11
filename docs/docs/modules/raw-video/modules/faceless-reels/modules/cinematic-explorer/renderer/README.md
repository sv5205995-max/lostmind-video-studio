# LOSTMIND Shared Renderer

## Purpose
Provide a shared video-rendering layer for all LOSTMIND video workflows.

## Supported Workflows
- Raw recorded video editing
- Faceless AI Reels
- Cinematic explorer and mystery Reels

## Planned Responsibilities
1. Receive a validated edit plan and media assets.
2. Arrange video clips, images, voiceover, music, sound effects, and captions.
3. Create a vertical 9:16 composition.
4. Render the final video as MP4.
5. Validate output dimensions, duration, audio, and file integrity.
6. Save the finished video for human review before publishing.

## Planned Tools
- HyperFrames: video composition and graphics.
- FFmpeg: video encoding, audio processing, and format validation.
- Node.js: runtime for the planned HyperFrames workflow.

## Expected Output
- MP4 video in 9:16 format.
- Captions synchronized with speech.
- Mixed voiceover, music, and sound effects.
- Render report containing output path, duration, and validation status.

## Design Principles
- Reuse the renderer across all three modules.
- Keep source files separate from rendered outputs.
- Use configurable resolution, frame rate, and audio levels.
- Do not publish automatically without the configured review and approval step.
- Use properly licensed or user-owned media assets.

## Current Status
Planning and documentation only. Rendering scripts, dependencies, and tests still need to be implemented and verified on the target PC.

## Next Steps
1. Set up Node.js and FFmpeg on the PC.
2. Verify the installed versions.
3. Create a minimal test project.
4. Render and validate one short 9:16 MP4.
5. Connect the renderer to the three LOSTMIND workflows.
