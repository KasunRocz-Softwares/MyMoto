# My moto — website

The project site for **My moto** (the *Rider Extras* build of OpenCfMoto): wireless Android Auto on
CFMoto MotoPlay and other Carbit / EasyConnect dashes, plus tyre pressure, fuel range, rain alerts,
ride reports and bike care.

**Live:** https://kasunrocz-softwares.github.io/MyMoto/

The app itself, its source and its releases live at
[KasunRoczDev/open-cfmoto](https://github.com/KasunRoczDev/open-cfmoto). The download buttons always
point at that repo's latest release, and the page fills in the version number from the GitHub API.

## Editing

Plain static files, no build step:

- `index.html` — the page
- `style.css` — styles (the app's dark colour tokens)
- `img/screens/` — app screenshots (from `docs/screenshots` in the app repo)
- `img/dashes/` — community dash photos, resized to 800×600
- `media/hud-demo.mp4` — the hero video

Preview locally with `python -m http.server` in this folder. GitHub Pages publishes `main` on every push.
After changing `style.css`, bump the `?v=` number on its `<link>` so browsers fetch the new file.
