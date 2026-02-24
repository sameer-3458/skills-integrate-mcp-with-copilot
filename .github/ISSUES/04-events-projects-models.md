Title: Add `Events`, `Projects`, `Honours`, `Talks`, `Publications` models and endpoints

Description:
Expand the data model to track events, projects, honours, talks, and publications with rich metadata and endpoints to create/list/update them.

Acceptance criteria:
- Create DB models for `Event` (type, date, location, description, attendees), `Project` (title, repo link, members, status), `Honour`, `Talk`, and `Publication`.
- Provide API endpoints to CRUD these resources and list by member or date range.
- Link `Event` and `Project` records to `Profile` (members) and optionally to `Activity`.
- Add at least basic pagination for listing endpoints.

Estimate: Medium (2 days)

Labels: enhancement, data-model, api
