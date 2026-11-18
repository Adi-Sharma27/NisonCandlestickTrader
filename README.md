# Nison Candlestick Trader (Standalone App Package)

This package is a **completely separate, isolated application** (`com.nison.candlesticktrader`) with its own local storage namespace (`nison_candlestick_trader_cfg_v1`), separate Android package ID, and dedicated GitHub Actions APK build pipeline so it never conflicts with any other trading app installed on your device.

## Package Contents
- `www/index.html` — Complete standalone Nison Candlestick Pattern & 4-Stage Dynamic Trailing BTC Auto-Trader (Delta India & Delta Global WebSocket/REST).
- `www/manifest.json` — Standalone Progressive Web App (PWA) manifest.
- `capacitor.config.json` — Capacitor Android config (`appId: com.nison.candlesticktrader`, `appName: Nison Candlestick Trader`).
- `package.json` — Capacitor 6 dependencies.
- `.github/workflows/build-apk.yml` — Automated GitHub Actions workflow that generates launcher icons, injects Android permissions, and compiles `app-debug.apk`.

## Quick Start
1. **Instant Desktop / Mobile Browser Mode:** Open `www/index.html` directly in Chrome/Edge or serve `www/` via any static server.
2. **Build Separate Android APK:** Push this folder to a new GitHub repository (`main` branch). GitHub Actions will automatically build and publish `nison-candlestick-trader-debug-apk` under the **Actions** tab.
