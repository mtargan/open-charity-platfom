# Data model (draft)

| Entity | Notes |
|---|---|
| organisation | A charity (tenant) |
| user | Staff or volunteer account, belongs to organisation(s) |
| role / permission | admin, staff, volunteer; least privilege |
| person | Someone receiving support; minimal fields, special-category data flagged |
| case | Ongoing matter for a person (e.g. application) |
| case_note | Timestamped entry per meeting, author, visibility level |
| appointment | Meeting or walk-in slot, attendees, status |
| task | Follow-up action assigned to a user |
| message / notification | Member-to-member and broadcast |
| campaign / donation | Fundraising records |
| audit_log | Who viewed or changed what, and when |
| checklist_run | An organisation's progress through a jurisdiction checklist |

Principles: collect the minimum, record a lawful basis per data category, support export and erasure, never delete audit logs.
