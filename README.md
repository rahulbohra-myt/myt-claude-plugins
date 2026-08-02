# MyYogaTeacher Claude Plugins

Internal marketplace of Claude plugins for MyYogaTeacher content, copy, and growth workflows.
GitHub-synced so updates roll out to the team automatically once connected.

## Plugins

| Plugin | Status | Description |
|---|---|---|
| `myt-lp-product-copy` | ✅ Live | Landing page and product/feature copy generation |
| Articles/taxonomy plugin | 🔜 Planned | Content briefs and article generation |
| LP → Astro code plugin | 🔜 Planned | Converts finished LP copy into shippable `.astro` files |
| Google Ads audit plugin | 🔜 Under consideration | Campaign diagnostics — separate from copy generation by design |

## Setup (one-time)

1. Push this repository to GitHub (private repo recommended)
2. In Claude: **Organization Settings → Plugins → Add plugins → Add marketplace → GitHub repository**
3. Point it at this repo — Cowork will sync automatically on future pushes

## Adding a new plugin later

1. Create the new plugin folder under `plugins/`, with its own `.claude-plugin/plugin.json`
2. Add an entry to `.claude-plugin/marketplace.json` under `"plugins"`
3. Push — the sync picks it up, no re-upload needed

## Maintenance

Each plugin should carry its own brand/reference source of truth (e.g. `myt-lp-product-copy`
bundles `MYT_Brand_Core.md`) rather than duplicating rules across plugins, to avoid the kind of
brand-language drift this setup was built to prevent.
