# Architecture — video-tiktok

| Component | Path / Setting | Purpose |
| :--- | :--- | :--- |
| Root Composition | `index.html` | 8s TikTok 9:16 (`1080x1920`, `30fps`) demo with GSAP 3.15, Tailwind v4, and `data-composition-variables` (`badge`, `headline`, `subheadline`, `step1`, `step2`, `step3`, `cta`) |
| Cloud Render CI | `.github/workflows/render.yml` | GitHub Actions (`ubuntu-latest`): Node 22, FFmpeg, cached Chromium, `lint`/`check`, `render`, `ffprobe` summary, artifact upload |
| HyperFrames Config | `hyperframes.json` | Registry URL, `compositions/`, `compositions/components/`, `assets/` paths, `autoProxy: true` |
| Project Metadata | `meta.json` | Studio project identity (`video tiktok`) |
| Package & Scripts | `package.json`, `package-lock.json` | Local `hyperframes` (`^0.9.80`) & `sharp` (`^0.35.5`), npm scripts for Studio, lint, check, snapshot, render |
| Git Ignore | `.gitignore` | Ignores `node_modules/`, `renders/`, `*.mp4`, `*.webm`, `.hyperframes/`, `.env` |
| Agent Instructions | `AGENTS.md`, `CLAUDE.md` | HyperFrames composition contract and CLI rules |
| Output Artifacts | `renders/`, `.hyperframes/artifacts/` | Local draft/final MP4s and PNG snapshots (gitignored) |
| Env Template | `.env.example` | Optional cloud API keys (`HEYGEN_API_KEY`, `ELEVENLABS_API_KEY`, `GEMINI_API_KEY`) |
