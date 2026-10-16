# Pollen Art Lab

[![Made with pollinations.ai](https://raw.githubusercontent.com/pollinations/pollinations/main/packages/ui/src/brand/badge-made-with.svg)](https://pollinations.ai/?ref=badge)

Turn a text idea into artwork using the [Pollinations](https://pollinations.ai) image API.

**Live app:** https://ovalprint1-sketch.github.io/pollen-app/

## What it does

- Describe an idea, pick a **style** (painting, neon, watercolor, pixel, oil, 3D…) and an **aspect ratio** (1:1, 16:9, 9:16, 4:3).
- **Sign in with Pollinations** (Bring Your Own Pollen): each visitor authorizes the app and spends their own Pollen on generations.
- Download the resulting image in one click.

## How it uses Pollinations

- Image generation: `https://gen.pollinations.ai/image/<prompt>` with the user's authorized key sent as `Authorization: Bearer sk_...`.
- Sign-in: OAuth authorization at `https://enter.pollinations.ai/authorize` (returns a scoped user key in the URL fragment).
- The app is a single static `index.html` — no backend, no stored keys.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8080
```

## Built with

- Vanilla HTML/CSS/JS, no build step.
- Powered by [Pollinations](https://pollinations.ai).
