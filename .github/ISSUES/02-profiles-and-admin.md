Title: Add `Profiles`, `Groups`, and simple admin endpoints

Description:
Introduce persistent member `Profiles` (name, email, grade, role, bio) and management endpoints or a minimal admin UI to create/update member profiles, groups, teams, and responsibilities.

Acceptance criteria:
- Add a `Profile` model persisted in the DB with fields: `id`, `email` (unique), `name`, `grade`, `role`, `bio`, `joined_at`.
- Add models for `Group`, `Team`, and `Responsibility` with clear relations to `Profile`.
- Provide protected admin endpoints (or a minimal HTML admin page) to manage profiles and groups. Admin can create/update/delete.
- Provide API docs examples and at least one integration test for profile creation.

Notes:
- Authentication/authorization will be a separate issue; for now protect admin endpoints with a simple dev-mode token or a placeholder.

Estimate: Medium (1-2 days)

Labels: enhancement, backend, api
