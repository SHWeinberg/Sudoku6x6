6x6 VARIANT SUDOKU - installable app (PWA)
==========================================

FILES
  index.html            the whole app (puzzles, generator, editor, history)
  manifest.webmanifest  name, colors and icons for the Home Screen
  sw.js                 makes the app work offline
  icons/                app icons

STEP 1: PUT THE FOLDER ON THE WEB (any one of these; all free and HTTPS)
  A. Netlify Drop (quickest)
     Open app.netlify.com/drop and drag this whole folder onto the page.
     Copy the https address it gives you.
  B. GitHub Pages
     Create a repository, upload index.html, manifest.webmanifest, sw.js and
     the icons folder, then Settings > Pages > deploy from the main branch.
     Address: https://YOURNAME.github.io/REPOSITORY/
  C. Cloudflare Pages
     Workers & Pages > Create > Pages > Upload assets, then drop the folder.

  iPhone web apps need HTTPS. Opening index.html straight from Files will not
  install as an app.

STEP 2: INSTALL ON THE IPHONE
  1. Open the address in Safari.
  2. Tap Share, then Add to Home Screen, then Add.
  3. Open the app from its Home Screen icon. After the first launch it works
     with no connection.

GOOD TO KNOW
  - Saved puzzles, solve history and in-progress puzzles are stored on the
    device. The Home Screen app and Safari keep separate storage. Use
    Library > Export current to back up or move a puzzle.
  - The address is not password protected. The app holds no personal data and
    sends nothing anywhere. For a private address, put it behind an access
    control such as Cloudflare Access.
  - To update, upload the new files over the old ones. The installed app picks
    up the update the next time you open it (it may take a second launch).
