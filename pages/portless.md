[portless](https://github.com/vercel-labs/portless) — stable named local URLs instead of port numbers, for humans and agents

- replaces `localhost:3000` with named URLs like `myapp.local`, https + auto-trusted certs
- vercel-labs, 7.7k⭐, active (v0.11.0 shipped Apr 28 2026)
- killer use case: char desktop dev when juggling tauri shell + backend + preview servers on whatever ports vite grabs
- fixes localhost OAuth callback pain (google-oauth example in repo)
- subdomain routing → cookies/auth scoped per app, no cross-port session collisions
- not needed for charpedia (always-on :8000 daemon) — this is a coding-time tool
