# 🧊 Glass Notes

> **Your personal notes. Reimagined.**

Glass Notes is a customizable notes and personal-assistant PWA focused on a clean **UX/UI**, Liquid Glass aesthetics, personal organization, reminders, checklists and the JARVIS assistant concept.

## ✨ Current features

- 📝 Notes
- ✅ Checklists with visual completion and strike-through
- 💳 Payment tracking and due dates
- 🔔 JARVIS browser notifications
- 🤖 JARVIS assistant and contextual queries
- 🎙️ Voice interaction
- 🧠 JARVIS Memory for notes, tasks and payments
- 🎨 Customizable Liquid Glass experience
- 🖼️ Custom main background
- 📱 Installable PWA experience
- 🔤 Custom typography architecture

## 📁 Project structure

```text
glass-notes/
├── index.html
├── sw.js
└── README.md
```

## 🚀 Run / publish

The project is a client-side PWA. Upload the files to a GitHub repository and publish the repository with GitHub Pages.

After replacing files, reload the PWA. If an older version remains visible, clear the site's cached data or unregister the old service worker and reload.

## 🤖 JARVIS

JARVIS is designed as the assistant layer of Glass Notes.

The current architecture separates:

1. **Commands** — create or manage information.
2. **Memory queries** — ask about notes, tasks and payments.
3. **Alerts** — surface approaching due dates.
4. **Voice** — interact naturally through speech recognition and speech synthesis.

## 🧊 Design principles

Glass Notes prioritizes:

- UX/UI before feature overload
- Liquid Glass / iOS-inspired visual language
- Cyberpunk accents without sacrificing readability
- Per-note personalization
- Fast interaction on mobile
- Local-first behavior where practical

## 🗺️ Roadmap

- [x] Notes
- [x] Checklists
- [x] Payments
- [x] Reminders
- [x] JARVIS
- [x] Voice interaction
- [x] Browser notification layer
- [x] Custom main background
- [ ] Reliable Push Notifications when the PWA is closed
- [ ] Full generative AI conversation
- [ ] Smarter contextual prioritization
- [ ] Optional cloud synchronization
- [ ] Backup / restore
- [ ] Advanced JARVIS Command Center

## ⚠️ Current notification limitation

Browser notifications are available when permission is granted. Reliable notifications while the PWA is completely closed require a Push Notifications service and backend infrastructure.

## 📌 Version

**V1.3 Stable — Smart Checklist + project documentation**

