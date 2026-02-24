Title: Support file uploads for certificates and attachments

Description:
Allow members to upload certificates and attachments and associate them with `Profile` and `Activity` records.

Acceptance criteria:
- Implement an uploads endpoint that accepts file multipart upload and returns a persistent URL/reference.
- Store file metadata (filename, uploader profile, upload date, link to activity or project) in DB.
- Serve uploaded files from a secure static path (local `uploads/` folder for dev) and ensure filename collisions are handled.
- Add validation for allowed file types and a size limit.

Notes:
- Consider using `python-multipart` and `aiofiles` for FastAPI handling.
- For production, document S3-compatible storage as an option.

Estimate: Small (1 day)

Labels: enhancement, uploads
