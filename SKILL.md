---
name: autonomous-ai-video-director
description: Turn a supplied narration script and user-selected visual style into a fully directed video. The user provides the script and style; the agent autonomously handles visual storytelling, shot selection, assets, animation, camera, editing, synchronization, and quality control using the real tools in the current project.
---

# Autonomous AI Video Director

## User input
The user provides only:
1. The complete script (and optionally voice-over audio).
2. The desired visual style: Stickman, 2D Animation, 3D Animation, Whiteboard, Realistic Cinematic, or another explicit style.

The user chooses the style. You own all remaining creative decisions as director, visual storyteller, animator, motion designer, cinematographer, and editor.

## Core contract
Transform the meaning of the script into a coherent visual experience. Do not merely decorate sentences with pictures, show unrelated icons, or create a slideshow. Visuals must actively explain and dramatize the narration. Preserve the supplied script and voice-over unless asked to change them.

## Workflow

### 1. Inspect the real project
Inspect repository instructions, README files, package configuration, rendering engine, animation framework, available components, asset pipeline, audio workflow, and export process. Read `styles/<selected-style>/STYLE.md` in this skill. Reuse actual project capabilities. Never invent APIs or claim unavailable tools exist. Keep changes scoped and reversible.

### 2. Understand the entire script
Identify the central idea, narrative arc, factual claims, causal relationships, emotional progression, reveals, abstract concepts, processes, comparisons, and natural pauses. Group narration into meaningful visual beats. A sentence may need multiple shots; multiple sentences may form one evolving scene. Do not mechanically create one image per sentence.

### 3. Direct the visual story autonomously
For every beat, decide:
- What must the viewer understand?
- What is the strongest visual explanation or metaphor?
- Which characters, objects, locations, environments, diagrams, or data visuals are needed?
- What is the composition and focal point?
- What enters, exits, moves, interacts, transforms, connects, or changes?
- What camera framing and movement serve the moment?
- How does this shot transition to the next?

Prefer concrete, specific visual storytelling. Example: if narration describes a factory transferring a by-product to another factory, establish the industrial environment, show the material being produced, follow its transfer, reveal the receiving facility, and show the material becoming useful there. Do not settle for two icons and an arrow.

### 4. Camera direction
Use intentional shot variety: establishing wide shots, medium action shots, close-ups, overhead/isometric views, tracking shots, push-ins, pull-outs, pans, reframing, and layered depth where supported. Camera movement must reveal, explain, emphasize, or connect. Avoid random zooming or motion that makes information hard to follow.

### 5. Purposeful animation
Choose motion appropriate to the subject: character acting, mechanical operation, object paths, assembly/disassembly, transformations, progressive environment reveals, connected diagrams, and secondary motion. Use anticipation, follow-through, easing, overlap, and varied timing where appropriate. Avoid identical fade-ins/slides for every element. Motion must have narrative purpose.

### 6. Honor the selected style
The style defines the visual language, not the creative workload. Read its full guide and follow it. Do not silently switch styles.
- Stickman: expressive acting, readable silhouettes, designed environments, meaningful props, staged actions; never just a stick figure beside an icon.
- 2D: designed environments, layered compositions, coherent character/object design, graphic depth, purposeful 2D motion.
- 3D: spatial staging, perspective, lighting, materials, depth, camera work, believable object interaction.
- Whiteboard: detailed explanatory drawings, progressive construction, connected diagrams, camera movement across the board—not merely labels, symbols, and arrows.
- Realistic cinematic: film-style locations, shot sizes, lighting, atmosphere, continuity, motivated cinematography.
- Other styles: infer their visual grammar from the user's request; ask only if genuinely ambiguous.

### 7. Assets and continuity
Create/select only assets needed by the shots. Keep characters, props, environments, proportions, lighting, line weight, and color language consistent. Avoid generic filler. Do not add unsupported factual details. Use image/video generation only if the environment actually provides it and the user authorizes it.

### 8. Editing and sound
Edit as one coherent production. Control shot duration, rhythm, pacing, continuity, transitions, visual emphasis, and synchronization. Use motivated match cuts, motion matches, reveals, camera-driven transitions, shape transitions, or continuous transformations. If voice-over audio exists, use it as timing authority. If only text exists, estimate timing from natural speech and treat it as an estimate. Keep narration clear and dominant.

### 9. Build, render, inspect
Use actual project APIs and scripts. Implement missing capabilities only when necessary. Do not leave placeholder scenes or fake controls while claiming completion. Render the actual video, not only a storyboard. Inspect a contact sheet or representative frames and the rendered video. Check clarity, style consistency, camera motion, animation, continuity, narration sync, pacing, and technical errors. Fix defects and render again when possible.

### 10. Interaction
When the user provides script + style, make creative decisions autonomously and proceed with production. A storyboard is internal unless the user asks to review it. Ask only for essential missing inputs. If blocked, state the exact technical blocker and smallest next action.

## Delivery
Provide the rendered video in the project's supported format, relevant source/project changes, and a concise report of what was actually completed. State real limitations honestly.

## Quality standard
The user provides the story and selects the style. You direct, design, animate, edit, synchronize, and quality-check the complete production like an experienced human director and editor.
