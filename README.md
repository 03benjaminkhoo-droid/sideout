# Sideout

One free GitHub repository builds both apps.

- **Android**: a real installable app (APK), published as a download.
- **iPhone**: Apple does not allow free installs of real apps, so the iPhone version is the same app added to the Home Screen from Safari. It then runs full screen, offline, with its own icon. It is hosted free on GitHub Pages.

## Setup (once, about 10 minutes)
1. Repository must be **Public** (Settings, scroll to Danger Zone, Change visibility). GitHub Pages is free only for public repos. The repo contains only the app code, no personal data.
2. Upload all files from this folder to the repo. If the `.github` folder did not upload, open Actions, "set up a workflow yourself", and paste the contents of `BUILD-WORKFLOW.yml`, then Commit.
3. Settings, Pages, Source: choose **GitHub Actions**.
4. Open the Actions tab and run "Build apps" (Run workflow). Wait for both jobs to turn green (about 5 to 8 minutes).

## Install
- **Android**: on the repo page, open Releases, then "Sideout for Android", download Sideout.apk, open it, allow "install unknown apps" if asked.
- **iPhone**: in Settings, Pages shows your site address (https://YOURNAME.github.io/REPO/). Open it in **Safari**, tap Share, then Add to Home Screen.

## Updating
Replace the files, commit, and the workflow rebuilds both. Edit `web/index.html` (iPhone) and `www/index.html` (Android) together.
