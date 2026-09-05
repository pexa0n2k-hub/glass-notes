# 🧊 Glass Notes

> Your personal notes. Reimagined.

**V1.3.2 — Stable Checklist**

## Features
- 📝 Notes
- ✅ Checklists with visual checkbox, completion and strike-through
- 💳 Payment reminders
- 🤖 JARVIS assistant and memory
- 🎙️ Voice interaction
- 🔔 Browser notifications
- 🎨 Liquid Glass UI
- 🖼️ Custom global and per-note backgrounds
- 🔤 Custom fonts
- 📱 PWA / GitHub Pages

## V1.3.2 stability fixes
- Safe recovery for malformed or legacy localStorage data
- Stable IDs for checklist items
- Removed a null-element startup crash in the home screen
- Protected rendering from incompatible persisted data
- Service-worker version bumped to avoid stale assets

## Project structure
```text
glass-notes/
├── index.html
├── sw.js
└── README.md
```

## Roadmap
- [x] Notes
- [x] Checklists
- [x] Payments
- [x] Reminders
- [x] JARVIS
- [x] Voice interaction
- [x] Custom backgrounds
- [x] Custom fonts
- [ ] Reliable push notifications while the PWA is closed
- [ ] Cloud sync
- [ ] Backup / restore
- [ ] Advanced JARVIS AI
