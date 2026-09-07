# Botric Documentation

The product manual for [Botric](https://botric.ai), published with [Mintlify](https://mintlify.com) at [manual.botric.ai](https://manual.botric.ai).

## Structure

Navigation mirrors the app's own information architecture, so a page in the docs maps to a page in the product.

| Group | Covers |
| --- | --- |
| `getting-started/` | Sign-up, onboarding, navigation, core concepts |
| `workspace/` | Dashboard, Brand Profile, Knowledge Source, Reports, Analytics, Integrations |
| `search/` | Site Audit, GEO Audit |
| `discoverability/` | AI Visibility (GEO), Prompt Research, Citations, Competitors |
| `content/` | Content Brain, Blog Agent, Page Agent |
| `support/` | Chat Agent, Conversations |
| `account/` | Profile, Workspaces, Admins, Plans, Subscription, Credits, Invoices, Support |
| `reference/` | Credits, glossary, troubleshooting |

Navigation is defined in `docs.json`. Adding a page means creating the `.mdx` file **and** registering its path there.

## Local development

```bash
npm i -g mintlify
mintlify dev
```

Run from the repository root, where `docs.json` lives.

## Publishing

The Mintlify GitHub app deploys automatically on push to the default branch.

## Conventions

- One page per product screen or per coherent group of tabs.
- `{/* IMAGE: ... */}` marks a spot where a screenshot belongs.
- Link between pages with absolute paths (`/workspace/dashboard`).
- Keep feature descriptions grounded in what the app actually does today; mark unreleased work as coming soon rather than documenting it as available.

## Troubleshooting

- `mintlify dev` not running — run `mintlify install` to reinstall dependencies.
- A page 404s — check it's registered in `docs.json`.
