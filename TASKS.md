# Tasks — video-tiktok

| ID | Task | Status | Notes |
| :--- | :--- | :--- | :--- |
| T1–T9 | HyperFrames CLI, 9 skills, GitHub CI workflow, local Git `main` | Done | Repo `https://github.com/knguyenminh856-bit/video-tiktok` |
| T10 | Build 30s Neon/Gemini Pro deal video (`compositions/*.html` + `index.html`) | Done | 7 scenes + progress bar, custom SVG icons, price-slash & slam |
| T11 | QA (`lint`, `check --safe-zone tiktok`, `snapshot`) | Done | `lint` 0/0, `layout` 0/0, `contrast` 20/20, `craft` only `film_silent` |
| T12 | Live Studio preview | Done | Running at `http://localhost:3002/#project/video%20tiktok` (daemon PID 9300, HTTP 200) |
| T13 | Push to GitHub & Cloud Render MP4 + Release download | Done | Run `44999606156` `success`; `neon-deal-tiktok.mp4` (`2,783,545 B`, 1080x1920 H.264 30fps 30s) |
| T14 | Add 25 synchronized free SFX cues & re-render on CI | Done | Run `45000435958` `success`; `neon-deal-tiktok.mp4` (`3,138,158 B`, H.264 + AAC 48kHz, `-15.9 LUFS`, `-1 dBTP`, 0 clip) |
| T15 | Add Vietnamese Neural voiceover (`vi-VN-NamMinhNeural`) & sync `45.3s` | Done | 7 VO MP3s + 25 SFX cues (`check` 0 errors / 0 warnings across all gates), pushed to `origin/main` |
