# Architecture — video-tiktok

| Component | Path / Setting | Purpose |
| :--- | :--- | :--- |
| Root Composition | `index.html` | `45.3s` TikTok 9:16 (`1080x1920`, `30fps`) synced to Vietnamese voiceover + 25 SFX cues |
| Hook Scene | `compositions/s1-hook.html` | `0.0–6.5s`: Frame-0 hook (`Dùng Neon chỉ 60K?!`) + subtitle synced at `3.3s` |
| Price Slash Scene | `compositions/s2-price-slash.html` | `6.5–12.6s`: `$20/THÁNG` crimson double-slash & `80K/NĂM` slam synced to spoken price |
| Verdict Beat | `compositions/s3-verdict.html` | `12.6–17.2s`: Paper-Cream (`#F5F3EE`) pattern interrupt (`Có thật sự là món hời?`) |
| Core Perks Scene | `compositions/s4-perks-core.html` | `17.2–25.6s`: 5TB Cloud, Gemini Pro, Antigravity · Argon · Neon (`Chưa gồm Carbon`) |
| Creative Perks Scene | `compositions/s5-perks-create.html` | `25.6–32.3s`: Flow (`1.000 CREDITS`), NotebookLM, hàng ngàn ưu đãi khác |
| Warnings Scene | `compositions/s6-warnings.html` | `32.3–39.3s`: 3 nhược điểm minh bạch (acc phụ, bảo hành 2h đầu, chờ lâu) |
| CTA Scene | `compositions/s7-cta.html` | `39.3–45.3s`: Chốt deal (`Cần deal ngon? IB mình ngay!`) & recap giá |
| Progress Overlay | `compositions/progress-bar.html` | `0.0–45.3s`: Thanh tiến trình liên tục trong vùng an toàn TikTok |
| Voiceover Audio | `assets/voice/v1..v7.mp3` | 7 file giọng nam `vi-VN-NamMinhNeural` (`edge-tts` +12%, normalized `-16 LUFS`) trên Lane 4 |
| Free SFX Assets | `assets/sfx/*.mp3` | 25 cue SFX ducked dưới giọng đọc trên Lane 2 & 3 |
| Video #2 Project | `videos/hydrogen-pro/index.html` | `39.7s` TikTok 9:16 (`1080x1920`, `30fps`): Google model mới, Pro `30K/3T` & `80K/năm` (`Neon • Argon • Hydrogen`), `Add Family 20K/người/năm` (chia 5 người) + 6 VO (`vi-VN-NamMinhNeural`) + 25 SFX |
| Cloud Render CI | `.github/workflows/render.yml` | GitHub Actions (`ubuntu-latest`): auto-detect root (`.`) hoặc `videos/<slug>`, `lint`/`check`, `render`, upload chung lên Release `latest-render` |
