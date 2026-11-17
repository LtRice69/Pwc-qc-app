# PWC QC - Android app (APK)

The same QC screens as the web link, packed as an Android app with Capacitor.
Works on Samsung Galaxy and Amazon Fire tablets (no Google Play needed - you install the APK yourself).

## Make the APK (GitHub builds it for you)
1. github.com > **New repository** > name `pwc-qc-app` > **Public** > Create.
   (Public is needed so the tablets can download updates. Nothing private is in here: no QC link, no key word.)
2. **Add file > Upload files** > drag in everything from this folder (including the hidden `.github` folder) > Commit.
3. **Actions** tab > "Build PWC QC APK" runs by itself (~6 minutes). Green tick = done.
4. **Releases** (right side of the repo page) > newest > `PWC_QC.apk`.

## Install on a tablet
1. On the tablet open `github.com/<you>/pwc-qc-app/releases` > tap **PWC_QC.apk**.
2. Open the download > **Install**. First time: allow **Install unknown apps** for Chrome (Galaxy) or Silk (Amazon).
3. Open **PWC QC** > paste the QC link + key word once > **Start**. Allow the camera.

## Updates
I send new files > upload them to the repo (replace) > GitHub builds a new Release.
Tablets show **Update available** next time the app opens > Download update > Install. Reports waiting to send are kept.

Keystore: `keystore/pwc-qc.jks` signs every build the same way so updates install over the old app. Keep it - if it's lost, tablets must uninstall and reinstall.
