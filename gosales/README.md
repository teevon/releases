# GoSales releases

- `android/`: the Android app. `latest.json` names the newest APK (version, size, SHA-256); installed tablets read it to update themselves. Published by `npm run release --workspace @gosales/mobile` in the GoSales repository.

Windows installers aren't here: at about 114 MB each they're over GitHub's 100 MB file limit, so the GoSales server serves them itself.
