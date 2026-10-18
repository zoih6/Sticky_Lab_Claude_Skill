---
name: sticky-lab-motion
description: Creates consistent Sticky Lab-style vertical motion-graphics reels from a script and optional voiceover. Use when the user asks for a Sticky Lab video, paper-note explainer, hand-drawn marker infographic, scene breakdown, motion plan, or production package.
---

# Sticky Lab Motion Graphics Skill

## Mission
Create short-form motion-graphics reels in the fixed **Sticky Lab** visual identity: a warm notebook/paper world, sticky notes, hand-drawn marker doodles, tape, paper cutouts, and tactile stop-motion-inspired movement. The topic may change; the visual system must not drift.

This skill plans and specifies the video. Do not claim to have rendered a finished video unless the available tools actually generated and assembled it. If direct video generation is unavailable, produce a production-ready package: scene plan, visual prompts, timing, voiceover alignment, asset list, and implementation notes.

## Required workflow
1. **Inspect inputs.** Identify the script, target duration, language/dialect, voiceover file (if any), platform, aspect ratio, resolution, FPS, and available image/video/audio tools. Do not ask for information already supplied.
2. **Establish the source of truth.** Use `references/STYLE_BIBLE.md` for visual rules, `references/SCRIPT_AND_VOICE_WORKFLOW.md` for narration handling, and `references/MOTION_LANGUAGE.md` for animation rules. Treat uploaded reference sheets in `assets/reference-sheets/` as visual references, not as permission to copy unrelated details.
3. **Analyze the script.** Preserve the user's meaning and wording unless asked to rewrite. Identify hook, key idea, explanation beats, example/analogy, and payoff/CTA. For a short reel, prefer one clear idea per scene.
4. **Handle voiceover.**
   - If audio is supplied, use its actual duration and, when tools permit, inspect pauses and speech boundaries. Do not invent exact word timestamps without audio analysis or a supplied transcript/timing file.
   - If only text is supplied, estimate narration duration using the selected language and delivery pace; label timings as estimates.
   - If both script and audio are supplied, audio timing is authoritative for total duration. Flag meaningful script/audio mismatches rather than silently changing the narration.
5. **Build the scene map.** Create a continuous sequence with scene ID, time range, spoken line, visual metaphor, on-screen text, paper assets, motion, transition, and sound cues. The visuals should explain the spoken idea, not merely decorate it.
6. **Design each scene.** Keep the palette, paper materials, outline treatment, typography, and movement consistent. Vary composition and visual metaphor to avoid repeating the same card layout.
7. **Check feasibility.** Distinguish assets that exist from assets that must be generated. Do not assume an icon, character, or voiceover exists unless provided or created with an available tool.
8. **Run the consistency audit** in `references/QUALITY_CHECKLIST.md`. Fix drift before delivering.
9. **Deliver concise outputs.** Unless the user requests another format, provide:
   - a short creative direction;
   - scene-by-scene production table;
   - ready-to-use visual prompts per scene;
   - on-screen text and voiceover alignment;
   - asset and audio requirements;
   - technical export settings;
   - a short list of unresolved assumptions.

## Default technical settings
- Format: vertical Reel, **9:16**
- Master resolution: **1080 × 1920**
- Frame rate: **30 fps**
- Default duration: as requested; if unspecified, ask only if it materially affects the deliverable. For a quick demo, default to 15 seconds.
- Safe area: keep important text and key objects away from platform UI zones; use approximately 8% side margins and 12% top/bottom margins as a starting point.
- Audio: voiceover clear and intelligible; music and effects remain subordinate.
- Export: H.264 MP4 for final delivery when a renderer is available. Do not promise a file unless it is actually created.

## Non-negotiable visual invariants
- Warm cream notebook/paper environment.
- Core palette: cream `#FFF4DF`, sticky yellow `#FFD84D`, orange `#FF783E`, ink black `#25231F`.
- Supporting colors: paper white `#FFFEF8`, kraft brown `#B58A60`, warm gray `#D9D1C3`.
- Thick, slightly imperfect black marker outlines; white/off-white sticker border when using sticker-like icons.
- Matte paper, visible but subtle fibers, cut edges, paper layers, tape, and soft contact shadows.
- Hand-drawn, simplified icons and arrows; no glossy 3D iconography.
- Arabic typography must render right-to-left correctly. Prefer Cairo ExtraBold/Bold and Tajawal Bold/Medium. Never ask an image model to render final Arabic copy when reliable text rendering is available.
- Stop-motion-inspired object motion: tactile, intentional, controlled. Do not make every element bounce.
- Maintain the same visual identity across topics. Change the metaphors and layout, not the style.

## Disallowed drift
Do not introduce gradients, neon, cyber/futuristic styling, glassmorphism, glossy plastic, generic corporate templates, random floating cards, excessive zooms, decorative particles, unrelated character styles, or a new palette without explicit user approval. Avoid excessive negative-prompt walls; state the positive visual target and only the few critical exclusions.

## Response behavior
- Be specific, not vague: give exact color codes, motion actions, durations, and text.
- Separate **confirmed input**, **assumption**, and **recommendation** where relevant.
- Do not fabricate source rules, timing measurements, assets, or tool capabilities.
- If the request is underspecified, make reasonable defaults and label them instead of blocking progress with many questions.
- The user prefers direct, self-contained production prompts over sprawling storyboard prose. Keep each scene prompt usable on its own, while repeating only the style invariants needed for consistency.
