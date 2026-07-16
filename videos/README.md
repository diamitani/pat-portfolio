# 🎬 Master Videos Repository

HyperFrames video projects — each video is a self-contained project folder.

## Create a new video

```bash
cd videos
npx hyperframes init my-video-name
```

This scaffolds a standard HyperFrames project with:
- `index.html` — composition entry point
- `STORYBOARD.md` — scene plan
- `assets/` — media, voiceovers, BGM

## Render

```bash
cd videos/my-video-name
npx hyperframes lint
npx hyperframes validate
npx hyperframes preview   # review in Studio
npx hyperframes render --quality high --output out.mp4
```

## Project structure

```
videos/
├── README.md              ← this file
├── my-first-video/        ← each video is a folder
│   ├── index.html
│   ├── STORYBOARD.md
│   ├── SCRIPT.md
│   ├── assets/
│   └── out.mp4
├── explainer-v2/          ← another video
├── product-demo/          ← etc.
└── ...
```

## Narration

Use the `media-use` skill for TTS voiceover. Add character box narration by placing a `<div>` with the narrator text and styling it as a talking-head box with the speaker's name.

## Publishing

Rendered MP4s are ignored by git (`.gitignore`). Upload finished videos to YouTube, social media, or embed on the portfolio site.
