Title: Integrations: Attendance import, Telegram notifications, GitHub contributions

Description:
Add integration points so the app can import attendance data, send Telegram notifications, and optionally track GitHub contributions for members.

Acceptance criteria:
- Attendance: add an endpoint or import job that accepts attendance records (CSV or API payload) and links them to `Profile` attendance logs.
- Telegram: add a background task or webhook to send notifications to a Telegram chat when events occur (new event created, signup threshold reached). Provide setup docs for bot token and chat id.
- GitHub: add a periodic job or endpoint to fetch contribution statistics for members by GitHub username and store summary stats on `Profile`.

Notes:
- Keep integrations optional and configurable via environment variables.
- Document setup steps in README.

Estimate: Medium (2-3 days)

Labels: enhancement, integrations
