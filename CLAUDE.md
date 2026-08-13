# Chula Embarques — SHIPPING

## Git identity

At the start of any session working in this repo, set the git commit identity
before making any commits:

```
git config user.name "Chula Brand"
git config user.email "shipping@chulabrand.com"
```

This keeps commit history showing "Chula Brand" as the author instead of the
default assistant identity.

## Notes for future sessions

- `Code.gs` (the Google Apps Script backend) is **not** part of this git
  repo — it lives only in the Google Sheet's bound Apps Script project. Any
  backend changes are delivered to the user as a file to paste into the
  Apps Script editor themselves (`Manage deployments → Edit → New version`).
- `index.html` is the frontend and is tracked here, pushed directly to
  `origin main`.
- Before pushing `index.html`, verify JS syntax by extracting the inline
  `<script>` blocks and running `node --check` on them.
- Before delivering `Code.gs` changes, verify syntax with
  `cp Code.gs Code_check.js && node --check Code_check.js && rm Code_check.js`.
