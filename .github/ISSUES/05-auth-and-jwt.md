Title: Add authentication (JWT) with roles (admin/member)

Description:
Add user authentication to protect admin endpoints and allow members to manage their profiles and signups.

Acceptance criteria:
- Implement authentication using JWT (suggested libs: `fastapi-users`, `pyjwt`, or `fastapi-jwt-auth`).
- Add `role` field on `Profile` (e.g., `member`, `admin`) and enforce role-based access control for admin endpoints.
- Protect signup/unregister endpoints as appropriate (allow public read, but require auth for signup if desired).
- Provide login/register endpoints for members.

Estimate: Medium (1-2 days)

Labels: enhancement, auth
