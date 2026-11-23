# GoHotel releases

- `staff/`: GoHotel Staff, the staff phone app (Android). Its home screen shows one tile per module the person's job allows: Housekeeping, Maintenance, Security, Waiter POS, and Kitchen/Bar display.

`latest.json` names the newest APK (version, size, SHA-256); the newest two are kept. Published by `npm run apk -- --release` in `apps/mobile-staff` of the GoHotel repository (scripts/apk.js).

Installed apps update themselves from this folder: each reads `latest.json` when it opens and offers the newer version. The download is checked against the size and SHA-256, and Android installs it only if it is signed with GoHotel's release key.

First install on a phone: download the newest APK from `staff/`, open it, and allow installing from that source when Android asks. Then open GoHotel Staff and enter the server address and business code the hotel gives you.
