---
name: remotion-video-toolkit
description: Complete toolkit for programmatic video creation with Remotion + React. Covers animations, timing, rendering (CLI/Node.js/Lambda/Cloud Run), captions, 3D, charts, text effects, transitions, and media handling. Use when writing Remotion code, building video generation pipelines, or creating data-driven video templates.
---

## When to use

Use this skill when working with Remotion — writing compositions, animating scenes, rendering videos, or building video generation infrastructure.

## How to use

Read individual rule files for detailed explanations and code examples:

### Core
- [rules/compositions.md](rules/compositions.md) - Defining compositions, stills, folders, default props and dynamic metadata
- [rules/rendering.md](rules/rendering.md) - **Rendering videos** — CLI, Node.js API, Lambda, Cloud Run, Express server patterns
- [rules/calculate-metadata.md](rules/calculate-metadata.md) - Dynamically set composition duration, dimensions, and props

### Animation & Timing
- [rules/animations.md](rules/animations.md) - Fundamental animation techniques
- [rules/timing.md](rules/timing.md) - Interpolation curves — linear, easing, spring animations
- [rules/sequencing.md](rules/sequencing.md) - Sequencing — delay, trim, limit duration
- [rules/transitions.md](rules/transitions.md) - Scene transitions
- [rules/trimming.md](rules/trimming.md) - Trimming — cut beginning or end of animations

### Text & Typography
- [rules/text-animations.md](rules/text-animations.md) - Typography and text animation patterns
- [rules/fonts.md](rules/fonts.md) - Loading Google Fonts and local fonts
- [rules/measuring-text.md](rules/measuring-text.md) - Measuring text, fitting text to containers, overflow detection

### Media
- [rules/videos.md](rules/videos.md) - Embedding videos — trimming, volume, speed, looping, pitch
- [rules/audio.md](rules/audio.md) - Audio and sound — importing, trimming, volume, speed, pitch
- [rules/images.md](rules/images.md) - Embedding images
- [rules/gifs.md](rules/gifs.md) - GIFs synchronized with timeline
- [rules/assets.md](rules/assets.md) - Importing images, videos, audio, and fonts
- [rules/can-decode.md](rules/can-decode.md) - Check video decode compatibility

### Captions & Subtitles
- [rules/transcribe-captions.md](rules/transcribe-captions.md) - Transcribing audio to generate captions
- [rules/display-captions.md](rules/display-captions.md) - TikTok-style captions with word highlighting
- [rules/import-srt-captions.md](rules/import-srt-captions.md) - Importing .srt subtitle files

### Data Visualization
- [rules/charts.md](rules/charts.md) - Chart and data visualization patterns

### Advanced
- [rules/3d.md](rules/3d.md) - 3D content with Three.js and React Three Fiber
- [rules/lottie.md](rules/lottie.md) - Lottie animations
- [rules/tailwind.md](rules/tailwind.md) - TailwindCSS integration
- [rules/measuring-dom-nodes.md](rules/measuring-dom-nodes.md) - Measuring DOM element dimensions

### Media Utilities
- [rules/get-video-duration.md](rules/get-video-duration.md) - Get video duration in seconds
- [rules/get-video-dimensions.md](rules/get-video-dimensions.md) - Get video width/height
- [rules/get-audio-duration.md](rules/get-audio-duration.md) - Get audio duration in seconds
- [rules/extract-frames.md](rules/extract-frames.md) - Extract frames from videos at specific timestamps

---

**GitHub:** https://github.com/zone99-llc/remotion-video-toolkit — PRs welcome! Submit new features and improvements.
