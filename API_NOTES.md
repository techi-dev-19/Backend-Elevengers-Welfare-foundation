Authenticated routes require `Authorization: Bearer <JWT>`.
CRUD collection routes: `/api/donations`, `/donors`, `/campaigns`, `/projects`, `/allocations`, `/expenses`, `/volunteers`, `/assignments`, `/receipts`, `/messages`; GET supports `page` and `limit`; POST and PATCH are permission-gated. `/api/dashboard/summary` returns key counts and totals.
Payment gateway webhooks must verify signatures and idempotency before marking donations Paid. Add organization scoping, audit logs, PDF receipt templates, tests, and stricter per-field validation before production.
