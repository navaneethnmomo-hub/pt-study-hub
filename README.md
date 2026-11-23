# Polytechnic Study Hub: app files

This folder is the whole app. Upload all of these files to a GitHub repository, then turn on GitHub Pages.

Files:
- index.html: the app itself (one file, works on its own)
- manifest.webmanifest: the app name, icons and colours used when it is installed
- sw.js: lets the app open and work without internet after the first visit
- icon-192.png, icon-512.png, maskable-512.png, apple-touch-icon.png: the app icons

## 1. Put it online
1. Create a new repository on GitHub. It must be public for free GitHub Pages.
2. Upload every file in this folder to the repository's main page (drag them in, or use Add file, then Upload files).
3. Go to Settings, then Pages. Choose Deploy from a branch, select main and / (root), and save.
4. After a minute, open the address GitHub shows, for example https://your-name.github.io/your-repo/

## 2. Install on your phone
- Android: open the address in Chrome, then tap the menu (three dots) and choose Install app. The header also shows an Install app button when Chrome allows it.
- iPhone: open the address in Safari, tap Share, then Add to Home Screen.

## 3. Updating the app
Upload the changed file again. If you change sw.js, also change the CACHE name at the top of it (for example study-hub-v1 to study-hub-v2), so phones pick up the new files.

## 4. Google Play (optional)
1. Create a Google Play Console developer account. There is a one-time US$25 fee.
2. Go to pwabuilder.com, enter your app's address, choose Package for stores, then Android, and download the package. Keep the signing key and its passwords somewhere safe. You need them for every future update.
3. Put the assetlinks.json file that PWABuilder gives you at .well-known/assetlinks.json in your repository. This removes the browser address bar from the app.
4. Upload the .aab file to Play Console. A new personal account must run a closed test with at least 12 testers for 14 days before it can apply for production.
5. Play asks for a privacy policy link. The app keeps your files on the phone. Your questions go to Anthropic only when you use the AI assistant with your own API key.

## Good to know
- Saved files stay in this phone's browser storage. Clearing the browser's site data can delete them, so download copies of anything important. Each file has a Download button.
- The AI assistant needs internet and your own Anthropic API key.
