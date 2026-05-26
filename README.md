# Minima Hub

Community-curated hub for the Minima blockchain ecosystem - nodes, libraries, and dApps.

**Live site**: [minima-hub.github.io](https://minima-hub.github.io)

---

## What is this?

Minima Hub is a one-page open-source directory of everything in the Minima ecosystem:

- **Nodes**: setup guides for desktop, Docker, Raspberry Pi, and VPS
- **dApps**: community-curated list of MiniDApps with filtering and search
- **Libraries**: official and community SDKs for building on Minima
- **Resources**: documentation, community links, developer tools

The goal: be the go-to reference for anyone looking for Minima resources.

---

## How to add your dApp

Edit `data/dapps.json` and submit a Pull Request. No HTML knowledge required.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full guide.

Quick version:

```json
{
  "name": "Your dApp Name",
  "description": "One sentence about what it does. Max 140 characters.",
  "category": "Finance",
  "url": "https://your-dapp-url.com",
  "github": "https://github.com/your-org/your-repo",
  "status": "active",
  "official": false,
  "added": "2026-05-26",
  "tags": ["relevant", "tags"]
}
```

Categories: `Finance`, `Tools`, `Communication`, `NFT`, `Gaming`, `Infrastructure`, `Developer`

---

## Run locally

```bash
# Using any static server
npx http-server . -p 8000
# Visit http://localhost:8000
```

Or open via the 0xHorizon build system:

```bash
cd ../1_working_files
npm install
npm run dev
```

---

## Project structure (public files)

```
2_development/
├── index.html         One-page website (pure HTML/CSS/JS)
├── data/
│   ├── dapps.json     dApp registry - edit this to add dApps
│   └── resources.json Node, docs, community, library links
├── assets/            Images and icons
└── CONTRIBUTING.md    How to contribute
```

---

## Stack

- Pure HTML, CSS, JavaScript - no frameworks, no build step required
- Data loaded at runtime via `fetch()` from JSON files
- Hosted on GitHub Pages
- Maintained by [0xHorizon](https://0xhorizon.xyz)

---

## Not affiliated with Minima Global

This is an independent community resource. For official Minima resources, visit [minima.global](https://minima.global).

---

## License

MIT - open source, fork and adapt freely.
