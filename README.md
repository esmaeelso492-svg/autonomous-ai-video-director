# Autonomous AI Video Director

An Antigravity skill repository for turning a script + chosen visual style into a fully directed video.

## User input
- Script / narration
- Visual style (Stickman, 2D, 3D, Whiteboard, Realistic Cinematic, etc.)

The agent independently handles visual storytelling, shot selection, assets, animation, camera direction, transitions, editing, synchronization, and quality control using the actual tools in the target project.

## Layout
- `SKILL.md` — agent role and production workflow
- `styles/<style>/STYLE.md` — visual language and direction rules
- `styles/<style>/example/shot-plan.example.json` — sample shot-plan schema
- `scripts/setup.sh` — checks local prerequisites
- `scripts/selftest.sh` — validates repository structure
- `scripts/new_video.sh` — creates an input workspace
- `scripts/render.sh` — calls an actual render/build/export script in a project

## Install
1. Put this repository folder in the skills directory used by Antigravity.
2. Reload Antigravity so it discovers `SKILL.md`.
3. Run `bash scripts/setup.sh` and `bash scripts/selftest.sh` in Git Bash on Windows or a Bash terminal.
4. Start a session and provide a script and style, e.g. `Style: 2D Animation`.

## Important
This repository provides the skill, style guides, and a lightweight project handoff. It does not bundle a proprietary rendering engine or claim to provide image/video generation by itself. The agent must inspect and use the rendering capabilities in your existing project (for example, your motion starter kit), implementing missing production logic there.

## New production folder
`bash scripts/new_video.sh 2d-animation my-first-video`

Add the narration to `input/script.txt` and optional voice-over audio to `input/`.

## Render
`bash scripts/render.sh /path/to/your/video-project`

The helper detects common npm scripts (`render`, `build`, `export`). It never invents a renderer.
