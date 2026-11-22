# Tasks — video-tiktok

| ID | Task | Status | Notes |
| :--- | :--- | :--- | :--- |
| T1–T6 | HyperFrames CLI, Chromium, 9 skills, project scaffold, verification | Done | `hyperframes@0.9.80`, `sharp@^0.35.5`, 9/9 skills synced |
| T7 | Configure `.gitignore` & `.github/workflows/render.yml` | Done | `push` on `main` & `workflow_dispatch` with quality/fps/format/variables |
| T8 | Build & verify 8s TikTok 9:16 demo (`index.html`) | Done | `lint` (0 errors), `check --safe-zone tiktok` (`ok: true`, contrast `16/16`), `draft.mp4` (`1080x1920`, `h264`, `8.0s`) |
| T9 | Initialize Git repo (`main`) & initial commit | Done | Committed on local `main`; add `origin` remote & push to trigger GitHub Actions |
