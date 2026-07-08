# HyperFrames Short — What is AI?

**YouTube Short:** 1080×1920 · 27 seconds · 5 scenes

## Render on Desktop (not Termux)

HyperFrames needs `onnxruntime-node` which only supports **Linux/macOS/Windows**. Render this on any desktop:

```bash
# 1. Install HyperFrames CLI
npm install -g hyperframes

# 2. Render the Short
npx hyperframes render ./what-is-ai --quality high --output what-is-ai-short.mp4

# Or use the skills system
npx skills add heygen-com/hyperframes
npx hyperframes render ./what-is-ai -o short.mp4
```

## Preview on Any Device (incl. Phone)

Open `index.html` in Chrome/Kiwi browser — GSAP animations play automatically with the timeline.

## Render on GitHub Codespaces (Free)

1. Push this folder to GitHub
2. Open in Codespaces
3. Run: `npx hyperframes render . --output short.mp4`
4. Download the MP4

## Cloud Render (AWS Lambda)

```bash
npx hyperframes lambda deploy
npx hyperframes lambda render ./what-is-ai --width 1080 --height 1920 --wait
```

## Structure
```
what-is-ai/
├── index.html          # HyperFrames composition
├── hyperframes.json    # Project metadata
└── README.md           # This file
```

## Scenes
| Time | Scene | Animation |
|------|-------|-----------|
| 0-5s | 🤖 Hook: What is AI? | Emoji explode → title fade |
| 5-12s | 01 — AI Since 1956 | Number slide → text fade |
| 12-19s | 02 — 97M Jobs | Number slide → text fade |
| 19-24s | 03 — Cancer Diagnosis | Number slide → text fade |
| 24-27s | 🌍 Outro: Subscribe | Scale in → CTA |
