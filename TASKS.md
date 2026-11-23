# Tasks — video-tiktok

| ID | Task | Status | Notes |
| :--- | :--- | :--- | :--- |
| T1–T9 | HyperFrames CLI, 9 skills, GitHub CI workflow, local Git `main` | Done | Repo `https://github.com/knguyenminh856-bit/video-tiktok` |
| T10 | Build 30s Neon/Gemini Pro deal video (`compositions/*.html` + `index.html`) | Done | 7 scenes + progress bar, custom SVG icons, price-slash & slam |
| T11 | QA (`lint`, `check --safe-zone tiktok`, `snapshot`) | Done | `lint` 0/0, `layout` 0/0, `contrast` 20/20, `craft` only `film_silent` |
| T12 | Live Studio preview | Done | Running at `http://localhost:3002/#project/video%20tiktok` (daemon PID 9300, HTTP 200) |
| T13 | Push to GitHub & Cloud Render MP4 + Release download | Done | Run `44999606156` `success`; `neon-deal-tiktok.mp4` (`2,783,545 B`, 1080x1920 H.264 30fps 30s) |
| T14 | Add 25 synchronized free SFX cues & re-render on CI | Done | Run `45000435958` `success`; `neon-deal-tiktok.mp4` (`3,138,158 B`, H.264 + AAC 48kHz, `-15.9 LUFS`, `-1 dBTP`, 0 clip) |
| T15 | Add Vietnamese Neural voiceover (`vi-VN-NamMinhNeural`) & sync `45.3s` | Done | Run `45001639446`; `neon-deal-tiktok.mp4` (`4,006,772 B`, `45.3s` H.264 + AAC `-16 LUFS`, `-2.1 dBTP`, 0 clip) |
| T16 | Build Video #2 (`videos/hydrogen-pro/`, `39.7s`, 6 VO + 25 SFX) | Done | `lint` 0/0, `check --safe-zone tiktok` 0/0 across all gates, snapshots verified |
| T17 | Multi-video CI (`.github/workflows/render.yml`) & render `hydrogen-pro-tiktok.mp4` | Done | Run `45095615916`; `hydrogen-pro-tiktok.mp4` (`4,064,289 B`, `39.7s` `1080x1920` 30fps H.264 + AAC 48kHz `-16 LUFS`, `-1.7 dBTP`, 0 clip) |
