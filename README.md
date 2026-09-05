# 🧊 Glass Notes

> Your personal notes. Reimagined.

Glass Notes is a mobile-first PWA for notes, checklists, payments, reminders and the JARVIS assistant concept.

## ✨ Features
- 📝 Notes with per-note personalization
- ✅ Checklists with Liquid Glass checkboxes and strike-through
- 💳 Payment agenda with due dates and reminders
- 🤖 JARVIS assistant, memory and contextual summaries
- 🎙️ Voice interaction
- 🔔 Browser notifications
- 🎨 Custom background and typography architecture
- 📱 PWA / GitHub Pages friendly

## 🛠️ V1.3.1 Stability Fix
This release hardens the local data migration so older notes without a checklist cannot crash the main screen. Existing checklist items are normalized with stable IDs.

## 📁 Structure
```text
glass-notes/
├── index.html
├── sw.js
└── README.md
```

## 🚀 GitHub Pages
Upload/replace `index.html`, `sw.js` and `README.md` in the repository. If the old PWA shell remains cached, refresh the page and, if necessary, clear the site's cached data once.

## 🗺️ Roadmap
- [x] Notes
- [x] Checklists
- [x] Payments
- [x] Reminders
- [x] JARVIS
- [x] Voice
- [x] Custom backgrounds
- [ ] Reliable push notifications when fully closed
- [ ] Cloud sync
- [ ] Backup / restore
- [ ] Advanced JARVIS Command Center

**Version: V1.3.1 Stable**
