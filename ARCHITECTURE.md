# Architecture — video-tiktok

| Component | Path / Setting | Purpose |
| :--- | :--- | :--- |
| Root Composition | `index.html` | 30s TikTok 9:16 (`1080x1920`, `30fps`) entry mounting 8 sub-compositions with brand color vars |
| Hook Scene | `compositions/s1-hook.html` | `0.0–3.4s`: Frame-0 visible hook (`Dùng Neon chỉ 60K?!`) with lightning icon & neon volt accent |
| Price Slash Scene | `compositions/s2-price-slash.html` | `3.4–7.8s`: `$20/THÁNG` crimson SVG double-slash + recoil & `80K/NĂM` neon slam |
| Verdict Beat | `compositions/s3-verdict.html` | `7.8–10.8s`: High-contrast Paper-Cream (`#F5F3EE`) pattern interrupt (`Có thật sự là món hời?`) |
| Core Perks Scene | `compositions/s4-perks-core.html` | `10.8–15.8s`: 5TB Cloud, Gemini Pro, Antigravity · Argon · Neon (`Chưa gồm Carbon`) |
| Creative Perks Scene | `compositions/s5-perks-create.html` | `15.8–20.8s`: Flow (`1.000 CREDITS`), NotebookLM, và hàng ngàn ưu đãi khác |
| Warnings Scene | `compositions/s6-warnings.html` | `20.8–26.0s`: 3 nhược điểm minh bạch (acc phụ, bảo hành 2h đầu, chờ lâu) |
| CTA Scene | `compositions/s7-cta.html` | `26.0–30.0s`: Chốt deal (`Cần deal ngon? IB mình ngay!`) & recap giá |
| Progress Overlay | `compositions/progress-bar.html` | `0.0–30.0s`: Thanh tiến trình liên tục trong vùng an toàn TikTok |
| Free SFX Assets | `assets/sfx/*.mp3` | 12 hiệu ứng âm thanh miễn phí từ thư viện HyperFrames, gắn 22 cue đồng bộ beat trên Lane 2 & 3 trong `index.html` |
| Cloud Render CI | `.github/workflows/render.yml` | GitHub Actions (`ubuntu-latest`): `lint`/`check`, `render` (`neon-deal-tiktok.mp4`), `ffprobe`, Release direct download (`latest-render`) & artifact upload |
