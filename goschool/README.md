# GoSchool releases

- `tablet/`: the GoSchool tablet app (Android), the desktop hub's twin for schools that run on tablets.
- `owner/`: GoSchool Owner, the school owner's phone app.

Each folder's `latest.json` names the newest APK (version, size, SHA-256); the newest two are kept. Published by `node scripts/apk.js --release` in `apps/mobile` and `apps/owner` of the GoSchool repository (tools/publish-apk.js).

Windows installers aren't here: at about 114 MB each they're over GitHub's 100 MB file limit.
