# Contributing to Minima Hub

Minima Hub is community-maintained. Anyone can add or update a dApp, library, or resource by submitting a Pull Request.

## How to Add Your dApp

1. **Fork** this repository on GitHub
2. **Edit** `data/dapps.json`
3. **Add** your dApp entry at the end of the array
4. **Submit** a Pull Request with title: `[feat] Add [Your dApp Name]`

Your PR will be reviewed and merged once the dApp is verified as live and the entry is accurate.

---

## dApp Entry Format

Add a new object to `data/dapps.json`:

```json
{
  "name": "Your dApp Name",
  "description": "One sentence. What it does, for who. Max 140 characters. No hype.",
  "category": "Finance",
  "url": "https://your-dapp-url.com",
  "github": "https://github.com/your-org/your-repo",
  "status": "active",
  "official": false,
  "added": "2026-05-26",
  "tags": ["relevant", "lowercase", "tags"]
}
```

### Field Reference

| Field | Required | Description |
|-------|----------|-------------|
| `name` | Yes | Official display name |
| `description` | Yes | One sentence, max 140 chars, factual and neutral |
| `category` | Yes | See categories below |
| `url` | Yes | Primary URL - must be live |
| `github` | No | GitHub repo URL, or `null` |
| `status` | Yes | `active`, `beta`, `experimental`, or `archived` |
| `official` | Yes | `true` only for minima-global GitHub org projects |
| `added` | Yes | Date you are submitting: `YYYY-MM-DD` |
| `tags` | Yes | Array of lowercase strings |

### Categories

| Category | Use for |
|----------|---------|
| `Finance` | Wallets, DEX, token tools, DeFi |
| `Tools` | Productivity, file management, utilities |
| `Communication` | Messaging, Maxima-based apps, social |
| `NFT` | NFT minting, marketplaces, collectibles |
| `Gaming` | Games and game-related dApps |
| `Infrastructure` | Block explorers, node monitors, network tools |
| `Developer` | SDKs, dev tools, templates, testing tools |

---

## How to Add a Resource or Library

Edit `data/resources.json`:

- **Node resources**: add to the `node` array
- **Documentation links**: add to the `docs` array
- **Community links**: add to the `community` array
- **Libraries**: add to the `libraries` array

Library format:

```json
{
  "name": "Library Name",
  "description": "What it does and who it is for.",
  "language": "JavaScript",
  "url": "https://docs-or-website.com",
  "github": "https://github.com/org/repo",
  "npm": "package-name or null",
  "status": "active",
  "official": false
}
```

---

## PR Standards

- One dApp or resource per PR (keeps reviews clean)
- PR title format: `[feat] Add [Name]` or `[update] Fix [Name] URL`
- All URLs must be live and reachable at the time of submission
- Descriptions must be factual - no marketing claims or vague language
- No em-dash character (—) in any content - use a hyphen with spaces instead

---

## Updating an Existing Entry

If a dApp has moved, changed status, or has an updated GitHub URL:

1. Fork and edit `data/dapps.json`
2. Update the relevant fields
3. Submit a PR with title: `[update] Fix [dApp Name] - brief reason`

---

## Reporting Issues

Use GitHub Issues to:
- Report a dead link
- Flag a dApp that is no longer maintained
- Suggest a new category
- Report a factual error

---

## Code of Conduct

- Be factual and respectful in PR descriptions and issue comments
- No self-promotional language in dApp descriptions
- All content must relate to the Minima ecosystem

---

**Questions?** Open a GitHub Issue or reach out to charles@0xhorizon.xyz
