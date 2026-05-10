---
name: storyboard-prompt-generator
description: Generate a set of storyboard style image prompts from a user's idea. Use when the user asks for visual planning prompts, storyboard prompts, advertising storyboard prompts, director boards, concept boards, preproduction boards, visual proposal prompts, or says they have an idea and want multiple prompt options in the same style as a professional storyboard or visual planning table.
---

# Storyboard Prompt Generator

## Core Behavior

Turn the user's idea into a group of complete, copy ready image generation prompts.

Default to Chinese output when the user writes in Chinese. Default to 8 prompts unless the user asks for a different number.

Do not make a long plan. Give the prompt set directly. Ask a question only when there is no usable idea.

Do not generate images unless the user explicitly asks to generate images.

## Output Shape

Use this structure:

1. Short title for the prompt set.
2. One sentence describing the chosen creative direction.
3. Numbered prompt blocks.

Each prompt block should include:

Prompt name.

Full prompt text in one copy ready paragraph.

Optional use case label such as advertising storyboard, product planning board, animation storyboard, game concept board, event visual board, social content board, or brand proposal board.

## Prompt Requirements

Each prompt must ask for a 16:9 horizontal visual planning image.

Each prompt must feel like a professional production board, director storyboard, brand proposal board, or advertising visual plan.

Each prompt should include:

Top title area.

Clear divided information board layout.

Main concept or art direction area.

Product, character, service, place, or scene reference area.

Storyboard area with multiple panels.

Color palette or material samples.

Scene movement map or shot route when useful.

Lighting, mood, keywords, audio tone, and camera type areas when useful.

Short readable Chinese text inside the image.

Specific visual materials such as glass, ice, water, metal, paper, fabric, neon, smoke, sunlight, rain, dust, food texture, screen glow, or other context relevant details.

Avoid true brand logos, messy unreadable small text, excess characters, and generic placeholder scenes.

## Variation Strategy

When the user gives one idea, produce varied prompts from different angles:

Commercial advertising board.

Animation or comic storyboard board.

Product and scene design board.

Social media or short video planning board.

Premium brand proposal board.

Event or campaign visual board.

Character or worldbuilding reference board.

Information graphic or service flow board.

Pick the most relevant mix for the user's idea.

## Direct Expansion Rules

If the user asks for more prompts, continue with new directions and avoid repeating earlier variants.

If the user asks to save the prompts, create a Markdown file in the current workspace and include prompt titles, use cases, and full prompt text.

If the user asks for a specific style, keep the user's subject fixed and vary the visual language around that style.

If the user asks for a specific industry, keep all prompts tied to that industry and vary audience, channel, format, and art direction.

## Reference

For broader category ideas and reusable prompt patterns, read `references/prompt-patterns.md`.
