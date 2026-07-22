---
name: storyboard-prompt-generator
description: Generate a two-scene, 16-second vertical 9:16 product-video storyboard prompt from a user's idea or product image. Use for TikTok, Reels, Shorts, product ads, animation concepts, voice-over scripts, scene prompts, or Flow-ready production planning.
---

# Storyboard Prompt Generator

## Core Behavior

Turn one product image, product description, or creative idea into one production-ready storyboard for a **16-second vertical 9:16 short video**.

Write in the user's language. For Malay requests, use natural **Bahasa Melayu Malaysia**. Never require, add, or recommend Chinese language labels, Chinese dialogue, or Chinese text in the visual.

Create exactly **two sequential scenes**, each **8 seconds**:

- Scene 1: `0:00–0:08` — hook, problem/desire, or product introduction.
- Scene 2: `0:08–0:16` — product demonstration, payoff, and natural closing CTA.

Keep one coherent product identity across both scenes. Scene 2 must continue naturally from Scene 1 rather than reset to a new setting, actor, or product.

Do not generate images or video unless the user explicitly asks. Provide the storyboard and copy-ready scene prompts first.

## Output Shape

Use this structure:

1. **Storyboard title**
2. **Creative direction** — one concise sentence naming the style and target feeling.
3. **Product facts used** — only details visible in the supplied image or stated by the user.
4. **Voice direction** — language, voice character, energy, pace, and audio intent.
5. **Scene 1 (0:00–0:08)**
   - Purpose / hook
   - Vertical visual and camera plan
   - Product action
   - Emotion
   - Exact spoken line / voice-over in the user's language
   - Sound design / music cue
   - Copy-ready image-to-video prompt
6. **Scene 2 (0:08–0:16)**
   - Continuation / payoff / CTA
   - Vertical visual and camera plan
   - Product action
   - Emotion
   - Exact spoken line / voice-over in the user's language
   - Sound design / music cue
   - Copy-ready image-to-video prompt
7. **Global continuity and negative prompt**

## Mandatory Video Rules

- Every scene is vertical **9:16**, designed for TikTok, Reels, and Shorts. Never request a horizontal 16:9 board.
- Include exactly two scenes and exactly 16 seconds total, unless the user explicitly overrides both values.
- Include voice/audio direction for every storyboard. State whether the product itself speaks, a narrator speaks, or the scene relies on ASMR; do not leave audio unspecified.
- For an animated product-character request, the product may move, emote, or speak, but preserve its visible shape, color, packaging, and label details from the reference image.
- Use only visible product facts and user-provided facts. Do not invent results, clinical claims, ingredients, pricing, discounts, packaging, phones, user-interface cards, logos, or text overlays.
- Do not place embedded captions, subtitles, title cards, readable text, fake UI, watermarks, or unrelated props inside the generated visual unless the user explicitly asks for them.
- Keep camera actions concrete: close-up, macro, top-down, handheld push-in, slow orbit, rack focus, or product hero reveal.

## Style Directions

Select or follow the user's requested direction. Keep the product fixed and alter the storytelling/camera language rather than inventing a new product.

- **Commercial product ad**: fast clear hook, product hero framing, benefit shown through visible action.
- **Animation / product character**: a product becomes a believable character with subtle expressive motion and spoken dialogue.
- **Product design demo**: clean close-ups, practical demonstration, clear tactile interaction.
- **Social short video**: strong first-second hook, crisp pacing, authentic mobile-native framing.
- **Premium brand**: elegant lighting, restrained movement, polished hero reveal.
- **Campaign / lifestyle**: one relatable everyday moment, then a tangible product interaction.
- **Character / POV story**: short emotional POV with the product as a natural part of the action.
- **Infographic-free explainer**: communicate through product action and voice-over, never on-screen graphics.

## Prompt Template

Write each image-to-video prompt as a single compact paragraph with:

- `Vertical 9:16, 8-second Scene N`
- the exact referenced product and its visible identity
- setting, lighting, action, camera movement, and emotional tone
- spoken line and audio intent
- continuity link to the other scene
- restrictions: no text, subtitles, UI, cards, watermarks, extra products, or unsupported claims

## Completion Checklist

Before returning a storyboard, verify:

- [ ] Bahasa follows the user's language; no Chinese text or labels are present unless explicitly requested.
- [ ] Exactly two scenes are included: 0:00–0:08 and 0:08–0:16.
- [ ] Both scenes are vertical 9:16 and form one continuous video.
- [ ] Both scenes have exact voice-over/dialogue and sound direction.
- [ ] Every claim is visible on the product or supplied by the user.
- [ ] Product identity stays consistent and no unwanted UI/text/props are requested.

## Common Pitfalls

- Do not output a six-to-eight-panel horizontal production board; this skill is for a two-scene vertical video.
- Do not use Chinese labels as a generic visual-planning convention.
- Do not make Scene 2 a reset with a different room, person, or product.
- Do not turn spoken dialogue into embedded subtitles.
- Do not claim a render is ready when only the storyboard/prompt is ready.
