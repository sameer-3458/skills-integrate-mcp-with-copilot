Title: Add persistence (SQLite + ORM) to activities and users

Description:
Add a persistent datastore so activities, students, and signups survive server restarts. Replace the current in-memory `activities` dictionary with database-backed models and migrations.

Acceptance criteria:
- Use SQLite as the default dev DB (file-based) and an ORM compatible with FastAPI (suggested: SQLModel or SQLAlchemy + Pydantic models).
- Create models for `Activity`, `Student` (profile stub), and `Signup` (relationship).
- Provide schema migration scripts or instructions (alembic or equivalent).
- Update existing endpoints (`GET /activities`, `POST /activities/{name}/signup`, `DELETE /activities/{name}/unregister`) to work with the DB.
- Add basic unit tests verifying persistence across app restart (or a simple DB smoke test).

Notes:
- Keep API contract stable where reasonable (the same JSON shape as today) or document breaking changes.
- Use `sqlite:///./dev.db` for local development.

Estimate: Medium (2-3 days)

Labels: enhancement, backend, database
