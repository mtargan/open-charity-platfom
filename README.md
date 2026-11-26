# Open Charity Platform

An open-source platform that helps charity volunteers and staff give people in need a consistent, joined-up experience, and helps new charities start on the right regulatory footing.

> **Status:** early stage / pre-alpha. Design docs and compliance data come first; code follows the [roadmap](ROADMAP.md).

## The problem

Small charities run on rotating volunteers. Case notes end up in WhatsApp threads, spreadsheets and people's heads, so the person asking for help has to repeat their story every visit, and nothing is reliably tracked.

## What it does (planned)

- **Appointments and walk-ins**: book meetings, manage office walk-in rota.
- **Shared case record**: applications, actions taken and outcomes per meeting, so any member can pick up where the last left off.
- **Member network**: one place to notify all members and for members to contact each other.
- **Fundraising and membership**: campaigns, donations tracking, member distribution.
- **Charity setup standard**: a machine-readable, per-jurisdiction checklist of regulatory requirements (registration, data protection, safeguarding, fundraising rules) for anyone opening a charity. See [`jurisdictions/`](jurisdictions/).

## Principles

1. **Privacy by design.** Case data is highly sensitive. See [docs/privacy-by-design.md](docs/privacy-by-design.md).
2. **Least-privilege access.** Volunteers see only what their role needs.
3. **Jurisdiction-aware.** UK first; other countries added as community-maintained packs.
4. **Usable by non-technical volunteers.** Simple, accessible, mobile-friendly.

## Repository layout

| Path | Purpose |
|---|---|
| `docs/` | Architecture, data model, privacy design |
| `jurisdictions/` | Per-country regulatory checklists (YAML) |
| `ROADMAP.md` | Milestones |
| `CONTRIBUTING.md` | How to help |

## Get involved

Contributions are welcome from developers, charity workers, lawyers and data-protection practitioners. Compliance data in particular needs domain experts. Start with [CONTRIBUTING.md](CONTRIBUTING.md) and the issues labelled `good first issue`.

## Licence

MIT, see [LICENSE](LICENSE).

> Nothing in this repository is legal advice. Compliance checklists are community-maintained guides and must be verified against current official sources.
