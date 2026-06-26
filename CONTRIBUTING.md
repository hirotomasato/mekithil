# Contributing to MiMo Chain Bot

Thanks for your interest in contributing! 🚀

## Getting Started

```bash
git clone https://github.com/hirotomasato/mekithil.git
cd mekithil
npm install
cp config/default.example.json config/default.json
# Edit config with your test credentials
```

## Project Structure

```
src/
├── clients/      # External API wrappers (tempmail, 2Captcha)
├── core/         # Main registration logic
├── browser/      # Playwright helpers (fingerprint, human, proxy)
├── runner/       # Chain orchestrator
├── bot/          # Telegram bot (commands, UI, middleware)
├── config.js     # Config loader
└── index.js      # Barrel export

scripts/          # CLI entry points
config/           # Configuration templates
```

## Development

### Running Tests
```bash
# Single account test (CLI)
npm test

# Telegram bot (dev mode — headless)
npm run bot
```

### Code Style
- ESM modules only (`import`/`export`)
- Async/await everywhere
- Console logs in English, Telegram messages in Indonesian
- New features → add to `src/`, update barrel export in `src/index.js`

## Pull Requests

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "feat: description"`
4. Push: `git push origin feature/your-feature`
5. Open a PR against `main`

### Commit Convention
- `feat:` — new feature
- `fix:` — bug fix
- `docs:` — documentation
- `refactor:` — code restructuring
- `chore:` — maintenance

## Reporting Bugs

Open an issue with:
- Bot version (`/start` shows version)
- Error message / screenshot
- Steps to reproduce
- Config used (hide sensitive values!)

## Feature Requests

Open an issue with:
- What problem it solves
- Suggested implementation
- Use case example

---

🔷 MiMo Chain Bot — built with ❤️ by [masantoid](https://github.com/hirotomasato)
