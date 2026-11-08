---
name: ai-game-media-studio
description: "Coordinate end-to-end ai game & media studio workflows from one master skill, loading specialist playbooks as needed."
---

# AI Game & Media Studio

## Mission
Create playable and media-rich experiences with a coherent art direction, predictable real-time or offline pipelines, measurable performance, and accessible controls.

## Use this skill when
The user asks to create, extend, analyze, or deliver a ai game & media studio project and expects one coordinated workflow rather than manually selecting individual specialist skills.

## Invocation contract
This is the only selectable skill in this repository. The specialist modules below are internal reference playbooks, not separate skills to invoke. Start from the user's brief, load only relevant references, and coordinate the complete workflow.

## Required inputs
Infer what is clear from the user's brief and repository. Identify only essential missing information. Typical inputs include goal, target users/platform, scope, references, constraints, existing stack, output format, budget, deadline, and acceptance criteria. Ask one concise clarification only when a missing fact blocks safe or correct execution; otherwise state reasonable assumptions and proceed.

## Operating protocol
1. Inspect the current repository, project instructions, files, configuration, and existing conventions before editing.
2. Translate the request into deliverables, explicit assumptions, non-goals, acceptance criteria, and risks.
3. Build a short phased plan. Prefer a working vertical slice over broad scaffolding that does not run.
4. Read the relevant internal references from the map below. Do not load unrelated modules or duplicate work.
5. Discover the actual tools, dependencies, APIs, providers, and runtime capabilities available in the current environment. Never invent tool names, provider availability, model IDs, endpoints, test results, or completed outputs.
6. Implement the requested outcome in the existing project. Preserve working behavior and avoid unnecessary rewrites.
7. Validate with the strongest available automated and manual checks. Fix issues found, then re-run the relevant checks.
8. Report exact files changed, commands/tests executed and results, deliverables created, unresolved issues, and what remains unverified.

## Internal specialist reference map
- `game-engine-engineer` — read `references/game-engine-engineer.md` when this capability is needed.
- `3d-rendering-engineer` — read `references/3d-rendering-engineer.md` when this capability is needed.
- `graphics-engineer` — read `references/graphics-engineer.md` when this capability is needed.
- `audio-engineer` — read `references/audio-engineer.md` when this capability is needed.
- `video-processing-engineer` — read `references/video-processing-engineer.md` when this capability is needed.
- `human-centered-product-design` — read `references/human-centered-product-design.md` when this capability is needed.
- `design-quality-critic` — read `references/design-quality-critic.md` when this capability is needed.
- `product-experience-engineer` — read `references/product-experience-engineer.md` when this capability is needed.

## Coordinated workflow
1. Clarify target platform, game/media type, engine, assets, performance budget, and interaction model.
2. Inspect project engine, scene graph, asset pipeline, rendering backend, and build configuration.
3. Define art direction, experience flow, input model, accessibility, and content requirements.
4. Design game loop, scene architecture, rendering, shaders, audio, and media pipelines.
5. Implement incrementally with test scenes and representative media fixtures.
6. Profile frame time, memory, load time, render time, and audio/video synchronization.
7. Validate target devices, controls, visual quality, and asset rights.
8. Document build, export, optimization, and known platform limitations.

## Expected deliverables
- game/media architecture
- scene and rendering implementation
- asset and audio pipeline
- performance and visual QA report
- build/export documentation

## Quality gates
- Requirements map to implemented behavior or clearly documented non-goals.
- The project builds/runs with available dependencies, or blockers are stated with evidence.
- Tests cover critical user flows or critical subsystem invariants.
- Security, privacy, accessibility, performance, and failure states are considered where relevant.
- Documentation matches the delivered implementation.
- No capability is described as complete unless the corresponding artifact exists and has been checked.

## Human-centered quality requirement
For any user-facing interface, load the human-centered design, design critique, and product-experience references. Apply them as quality gates throughout the work, not as a last-minute decoration pass. The result should be distinctive and fit the product domain, not a generic AI template.


## Security, privacy, and rights
- Protect secrets and personal data. Never place API keys, access tokens, passwords, signing keys, or private credentials in source files, prompts, examples, or logs.
- Use only dependencies, media, datasets, and assets with verified rights and compatible licenses.
- Do not claim external APIs, models, services, or tools are configured unless verified in the current environment.

## Approval gates
Ask before paid API/service usage, production deployment, public publication, destructive changes, external account actions, large cloud jobs, or changes that can incur charges. Do not ask for approval for ordinary reversible local edits within the user's requested scope.

## Stop conditions
Stop and explain the blocker when required permissions, credentials, source material, tools, dependencies, or target hardware are unavailable. Continue with independent work where possible, but do not simulate unavailable external generation or claim a final build succeeded.

## Final response format
Summarize: outcome; key implementation; files/artifacts; validation results; required user actions; known limitations. Be explicit about partial completion.
