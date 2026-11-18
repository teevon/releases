# GoSchool releases

- `tablet/`: the GoSchool tablet app (Android), the desktop hub's twin for schools that run on tablets.
- `owner/`: GoSchool Owner, the school owner's phone app.

Each folder's `latest.json` names the newest APK (version, size, SHA-256); the newest two are kept. Published by `node scripts/apk.js --release` in `apps/mobile` and `apps/owner` of the GoSchool repository (tools/publish-apk.js).

Installed apps update themselves from these folders: each reads its `latest.json` when it opens and offers the newer version.

The Windows installer isn't in these folders: at about 114 MB it's over GitHub's 100 MB file limit for committed files. It's on this repository's Releases page instead, as a single release tagged `goschool-desktop`. That release holds only the newest version, and the owner decides when one goes there (`node tools/release-desktop.js` in the GoSchool repository). The download link stays the same:

https://github.com/teevon/releases/releases/download/goschool-desktop/GoSchool-Setup.exe
