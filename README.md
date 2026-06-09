# Cookie Chain Apps Registry

A public and community-maintained registry of applications, infrastructure, wallets, NFT projects, and ecosystem tools built on Cookie Chain.

## Purpose

This repository serves as the official source of ecosystem data used across Cookie Chain websites and applications.

Projects listed here can be automatically displayed on ecosystem pages, directories, explorers, dashboards, and other community-built services.

## Structure

```txt
.
├── apps.json
└── logos/
```

### apps.json

Contains the ecosystem registry.

Example:

```json
{
  "title": "CookieSwap",
  "description": "Native DeFi powerhouse for swaps, liquidity, and yield in the COOK ecosystem.",
  "tag": "DeFi",
  "href": "https://cookieswap.fun",
  "logo": "https://raw.githubusercontent.com/cookiechain/apps/main/logos/cookieswap.png"
}
```

### logos/

Contains logo assets referenced by entries inside `apps.json`.

Supported formats:

* PNG
* JPG
* JPEG
* SVG
* WEBP

## Categories

Current ecosystem categories include:

* DeFi
* Wallet
* Infra
* NFT
* Meme

Additional categories may be added as the ecosystem grows.

## Adding Your Project

1. Fork this repository.
2. Add your logo to the `logos/` directory.
3. Add a new entry to `apps.json`.
4. Open a Pull Request.

Example:

```json
{
  "title": "My App",
  "description": "Short description of the project.",
  "tag": "DeFi",
  "href": "https://myapp.xyz",
  "logo": "https://raw.githubusercontent.com/cookiechain/apps/main/logos/myapp.png"
}
```

## Listing Requirements

Projects should:

* Be related to Cookie Chain.
* Have a working public website.
* Provide a clear description.
* Use an appropriate category.
* Include a logo asset.

The community may reject spam, malicious, or misleading submissions.

## Data Source

Public JSON endpoint:

```txt
https://raw.githubusercontent.com/cookiechain/apps/main/apps.json
```

Applications can fetch ecosystem data directly:

```javascript
const apps = await fetch(
  "https://raw.githubusercontent.com/cookiechain/apps/main/apps.json"
).then((res) => res.json());
```

## Community Maintained

This repository is maintained by the Cookie Chain community.

Built by builders.
Maintained by degens.
Powered by cookies. 🍪
