# Hi Bored, I'm Dad 🫙

A "what should we do" jar for the kids. Installable web app (PWA): works offline, home-screen icon, full screen.

## Files
- index.html: the app screens and logic
- ideas.js: ALL the ideas, steps and links. Edit this to add or change ideas.
- manifest.json: app name, icon and colors for installing
- sw.js: offline support. Bump CACHE version after any change.
- icons/: app icons

## Host it free
### Option A: Netlify Drop (fastest, needs a computer)
1. Unzip this folder.
2. Go to https://app.netlify.com/drop and drag the folder onto the page.
3. You get an https link right away. Make a free account to keep it and rename it (e.g. bored-jar-jerez.netlify.app).
4. To update: drag the new folder onto the site's Deploys page.

### Option B: GitHub Pages
1. Create a new public repo (e.g. bored-jar).
2. Upload all files (keep the icons folder) via "Add file > Upload files" and commit.
3. Settings > Pages > Source: Deploy from a branch > main / (root) > Save.
4. After about 1 minute it's live at https://YOUR-USERNAME.github.io/bored-jar/

## Install on devices
- iPhone/iPad: open the link in Safari > Share > Add to Home Screen.
- Android: open in Chrome > Install app (or menu > Add to Home screen).

Done list and added ideas save on each device separately.

## Later: home lab
Any static web server works, e.g.
  docker run -d -p 8080:80 -v /path/to/bored-jar-app:/usr/share/nginx/html:ro nginx
Note: install and offline mode need https (or localhost).
