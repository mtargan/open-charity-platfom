# Jurisdiction packs

Each folder (ISO 3166 code, lower case) contains `checklist.yaml`.

Item schema:
```yaml
- id: unique-slug
  category: registration | governance | data-protection | safeguarding | fundraising | finance | other
  title: Short name
  description: What is required and who it applies to
  applies_when: Condition (optional)
  source: Official URL
  last_verified: YYYY-MM-DD
  status: draft | verified
```
Rules: official sources only; mark `draft` until a practitioner has verified it.
