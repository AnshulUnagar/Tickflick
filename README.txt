TICKFLICK - installable iPhone web app
=======================================

What's in this folder (all files sit side by side, no sub-folders):
  index.html            the whole app (fonts are built in)
  manifest.webmanifest  tells iOS the app's name and icons
  sw.js                 lets the app open with no internet
  apple-touch-icon.png, icon-192.png, icon-512.png   the app icon

1. Put the files online (free). The app has to be served from an https address.

   Option A - GitHub Pages (works from an iPhone)
     a. On github.com, create a new public repository, e.g. "tickflick".
     b. Add file > Upload files. Select every file from this folder, commit.
     c. Settings > Pages > Source: "Deploy from a branch", branch "main", folder "/ (root)", Save.
     d. After a minute your app is at  https://YOUR-NAME.github.io/tickflick/

   Option B - Netlify Drop (easiest on a computer)
     Open app.netlify.com/drop, drag this whole folder onto the page.

2. Install on your iPhone.
     Open the address in Safari > Share button > Add to Home Screen > Add.
     Open it from the new Tickflick icon. It runs full screen, with no Safari bars.

3. Good to know
     - Tasks, notes and photos are stored on that iPhone only. They do not sync with the
       Claude page version and do not move to other devices.
     - Deleting the Home Screen app or clearing Safari website data erases them.
     - The first launch needs internet. After that it works offline.
     - Sound effects are muted by the iPhone silent switch.
     - To publish an update later, re-upload the files and change the CACHE name
       in sw.js (currently 'tickflick-v8') to a new one, e.g. 'tickflick-v9', so phones pick up the new version.
