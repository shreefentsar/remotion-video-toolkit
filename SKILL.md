---
name: remotion-video-toolkit
description: Complete toolkit for programmatic video creation with Remotion + React. Covers animations, timing, rendering (CLI/Node.js/Lambda/Cloud Run), captions, 3D, charts, text effects, transitions, and media handling. Use when writing Remotion code, building video generation pipelines, or creating data-driven video templates.
---

# 🎬 Remotion Video Toolkit

Turn React components into real MP4 videos. This skill gives your AI agent deep knowledge of Remotion — from basic animations to production rendering pipelines.

**29 comprehensive rules** covering every aspect of programmatic video creation.

## 🚀 Use Cases

- **Personalized videos at scale** — Generate unique videos per user (Year in Review, onboarding, reports). Pass JSON data in, get MP4 out.
- **Automated social content** — Daily/weekly video posts from live data — stats, leaderboards, product updates — zero manual editing.
- **Dynamic marketing videos** — Customer name, product, pricing baked into video. One template, infinite variations.
- **Data-driven visualizations** — Animated charts, dashboards, KPI reports as shareable video clips.
- **E-commerce product videos** — Auto-generate product showcases from images + specs in your database.
- **TikTok/Reels captions** — Transcribe audio, display word-by-word highlighted captions, export ready for social.
- **Educational content** — Programmatic explainer videos, animated course materials, certificate generation.
- **Video rendering APIs** — Expose video generation as an HTTP endpoint for your app or SaaS.

## 📋 Requirements

- **Node.js** 18+
- **React** 18+ (Remotion uses React as its rendering engine)
- **Remotion** — `npx create-video@latest` to scaffold a project
- **FFmpeg** — bundled with `@remotion/renderer` (auto-installed)
- Optional: AWS account (for Lambda rendering), GCP account (for Cloud Run)

## 🎯 What's Covered

### Core
- [Compositions](rules/compositions.md) — Define videos, stills, folders, default props, dynamic metadata
- [Rendering](rules/rendering.md) — **CLI, Node.js API, AWS Lambda, Cloud Run, Express server** patterns
- [Calculate Metadata](rules/calculate-metadata.md) — Dynamic duration, dimensions, and props at render time

### Animation & Timing
- [Animations](rules/animations.md) — Fade, scale, rotate, slide — all the fundamentals
- [Timing](rules/timing.md) — Interpolation curves, easing, spring physics
- [Sequencing](rules/sequencing.md) — Delay, chain, and orchestrate scenes
- [Transitions](rules/transitions.md) — Smooth scene-to-scene transitions
- [Trimming](rules/trimming.md) — Cut beginning or end of any animation

### Text & Typography
- [Text Animations](rules/text-animations.md) — Typewriter, word highlight, reveal effects
- [Fonts](rules/fonts.md) — Google Fonts + local font loading
- [Measuring Text](rules/measuring-text.md) — Fit text to containers, detect overflow

### Media
- [Videos](rules/videos.md) — Embed, trim, speed, volume, loop, pitch shift
- [Audio](rules/audio.md) — Import, trim, fade, control volume and speed
- [Images](rules/images.md) — Embed with the `<Img>` component
- [GIFs](rules/gifs.md) — Timeline-synced GIF playback
- [Assets](rules/assets.md) — Import any media into your composition
- [Decode Check](rules/can-decode.md) — Validate browser compatibility before playback

### Captions & Subtitles
- [Transcribe Captions](rules/transcribe-captions.md) — Audio → captions (Whisper, Deepgram, AssemblyAI)
- [Display Captions](rules/display-captions.md) — TikTok-style word-by-word highlighting
- [Import SRT](rules/import-srt-captions.md) — Load existing `.srt` subtitle files

### Data Visualization
- [Charts](rules/charts.md) — Animated bar charts, line graphs, data-driven visuals

### Advanced
- [3D Content](rules/3d.md) — Three.js + React Three Fiber integration
- [Lottie](rules/lottie.md) — Embed Lottie/After Effects animations
- [TailwindCSS](rules/tailwind.md) — Style compositions with Tailwind
- [DOM Measurement](rules/measuring-dom-nodes.md) — Measure element dimensions at render time

### Media Utilities
- [Video Duration](rules/get-video-duration.md) — Get length in seconds
- [Video Dimensions](rules/get-video-dimensions.md) — Get width/height
- [Audio Duration](rules/get-audio-duration.md) — Get audio length
- [Extract Frames](rules/extract-frames.md) — Pull frames at specific timestamps

## ⚡ Quick Start

```bash
# Create a new Remotion project
npx create-video@latest my-video

# Preview in browser
cd my-video && npm start

# Render to MP4
npx remotion render src/index.ts MyComposition out/video.mp4

# Pass dynamic data
npx remotion render src/index.ts MyComposition out.mp4 --props '{"title": "Hello"}'
```

## 🤝 Contribute

**GitHub:** [github.com/shreefentsar/remotion-video-toolkit](https://github.com/shreefentsar/remotion-video-toolkit)

Missing a feature? Found a better pattern? PRs are welcome — submit new rules, improve existing ones, or add code examples.

Built by [Zone 99](https://zone99.dev) ⚡
