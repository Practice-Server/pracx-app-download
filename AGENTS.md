# AGENTS.md

Working instructions for this repository — for human contributors and AI
coding agents alike.

**This repo is a release feed, not a codebase.** It exists so that
`pracx-app`'s Electron Forge publisher has somewhere to push Windows
installers, and so every installed PracX desktop client has somewhere to check
for updates (`electron-updater` reads this repo's GitHub Releases).

Rules, all of them:

- **No application code lives here, ever.** Client code belongs in
  `pracx-app`.
- **Releases and tags are load-bearing.** Deleting or re-tagging a release can
  break auto-update for every installed client. Do not touch releases by hand
  — they are produced by `pracx-app`'s publish flow, and a human decides when
  one goes out.
- Never commit secrets — here or anywhere in this org.
