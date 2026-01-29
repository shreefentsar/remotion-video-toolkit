---
name: remotion-video-toolkit
description: Complete toolkit for programmatic video creation with Remotion + React. Covers animations, timing, rendering (CLI/Node.js/Lambda/Cloud Run), captions, 3D, charts, text effects, transitions, and media handling. Use when writing Remotion code, building video generation pipelines, or creating data-driven video templates.
---

# Remotion Video Toolkit

Write React components, get real MP4 videos. This skill teaches your AI agent how to build with Remotion — from a first animation to a production rendering pipeline.

29 rules. Every major Remotion feature covered.

## What you can build with this

**Personalized video at scale.** Feed user data as JSON props, render a unique video per user. Think Spotify Wrapped, GitHub Unwrapped, onboarding walkthroughs — one template, thousands of outputs.

**Automated social media clips.** Pull live data (stats, leaderboards, product metrics) and render daily or weekly video posts without anyone touching a timeline editor.

**Dynamic ads and marketing videos.** Swap in customer name, product image, pricing. Same template, infinite variations. Render server-side via API or Lambda.

**Animated data visualizations.** Turn dashboards and KPI reports into shareable video clips with animated charts and transitions.

**TikTok and Reels captions.** Transcribe audio, display word-by-word highlighted subtitles, export ready for upload.

**Product showcase videos.** Auto-generate from your database — images, specs, pricing — straight to MP4.

**Educational and explainer content.** Animated course materials, certificate videos, step-by-step walkthroughs — all driven by code.

**Video generation as a service.** Expose rendering as an HTTP endpoint. Your app sends JSON, gets back a video file.

## Requirements

- Node.js 18+
- React 18+ (Remotion renders React components frame-by-frame)
- Remotion — scaffold with `npx create-video@latest`
- FFmpeg — ships with `@remotion/renderer`, no separate install needed
- For serverless rendering: AWS account (Lambda) or GCP account (Cloud Run)

## What's inside

### Core
- [Compositions](rules/compositions.md) — define videos, stills, folders, default props, dynamic metadata
- [Rendering](rules/rendering.md) — CLI, Node.js API, AWS Lambda, Cloud Run, Express server patterns
- [Calculate metadata](rules/calculate-metadata.md) — set duration, dimensions, and props dynamically at render time

### Animation and timing
- [Animations](rules/animations.md) — fade, scale, rotate, slide
- [Timing](rules/timing.md) — interpolation curves, easing, spring physics
- [Sequencing](rules/sequencing.md) — delay, chain, and orchestrate scenes
- [Transitions](rules/transitions.md) — scene-to-scene transitions
- [Trimming](rules/trimming.md) — cut the start or end of any animation

### Text and typography
- [Text animations](rules/text-animations.md) — typewriter, word highlight, reveal effects
- [Fonts](rules/fonts.md) — Google Fonts and local font loading
- [Measuring text](rules/measuring-text.md) — fit text to containers, detect overflow

### Media
- [Videos](rules/videos.md) — embed, trim, speed, volume, loop, pitch shift
- [Audio](rules/audio.md) — import, trim, fade, volume and speed control
- [Images](rules/images.md) — the Img component
- [GIFs](rules/gifs.md) — timeline-synced GIF playback
- [Assets](rules/assets.md) — importing any media into compositions
- [Decode check](rules/can-decode.md) — validate browser compatibility

### Captions and subtitles
- [Transcribe captions](rules/transcribe-captions.md) — audio to captions via Whisper, Deepgram, or AssemblyAI
- [Display captions](rules/display-captions.md) — TikTok-style word-by-word highlighting
- [Import SRT](rules/import-srt-captions.md) — load existing .srt files

### Data visualization
- [Charts](rules/charts.md) — animated bar charts, line graphs, data-driven visuals

### Advanced
- [3D content](rules/3d.md) — Three.js and React Three Fiber
- [Lottie](rules/lottie.md) — After Effects animations via Lottie
- [TailwindCSS](rules/tailwind.md) — style compositions with Tailwind
- [DOM measurement](rules/measuring-dom-nodes.md) — measure element dimensions at render time

### Media utilities
- [Video duration](rules/get-video-duration.md) — get length in seconds
- [Video dimensions](rules/get-video-dimensions.md) — get width and height
- [Audio duration](rules/get-audio-duration.md) — get audio length
- [Extract frames](rules/extract-frames.md) — pull frames at specific timestamps

## Quick start

```bash
# Scaffold a project
npx create-video@latest my-video

# Preview in browser
cd my-video && npm start

# Render to MP4
npx remotion render src/index.ts MyComposition out/video.mp4

# Pass dynamic data
npx remotion render src/index.ts MyComposition out.mp4 --props '{"title": "Hello"}'
```

## Contribute

Source: [github.com/shreefentsar/remotion-video-toolkit](https://github.com/shreefentsar/remotion-video-toolkit)

Missing something? Found a better approach? Open a PR — new rules, improved examples, bug fixes all welcome.

Built by [Zone 99](https://99.zone)
