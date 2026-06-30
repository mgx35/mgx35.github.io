# AI Product Portfolio — Mykola Golovko

A zero-dependency static portfolio. No frameworks, no build step. Open
`index.html` in a browser and it works.

## Edit your content

| What | Where |
|------|-------|
| Name, role, tagline, email, links | `js/projects.js` → `PROFILE` |
| Projects (add / edit / reorder) | `js/projects.js` → `PROJECTS` |
| About paragraphs | `index.html` → `<div id="aboutProse">` |
| Colors / styling | `css/styles.css` → top `:root` and theme blocks |

### Add a project
Copy one object inside the `PROJECTS` array in `js/projects.js` and change the
fields. `featured: true` pins it to the top. `link` (optional) adds an "Open ↗"
button. `tags` render as pills. Save, refresh — done.

## Preview locally
Just double-click `index.html`. For a local server (optional, nicer):
```
# Python (no install needed on most systems)
python -m http.server 8000
# then open http://localhost:8000
```

## Deploy (free)

**Netlify (drag-and-drop, easiest)**
1. Go to app.netlify.com → "Add new site" → "Deploy manually".
2. Drag the `portfolio` folder in. Live in ~10 seconds.

**GitHub Pages**
1. Create a repo, push this folder's contents.
2. Settings → Pages → Source: `main` branch, root.
3. Site goes live at `https://<user>.github.io/<repo>/`.

**Vercel**
1. Import the repo at vercel.com.
2. Framework preset: "Other". Output dir: root. Deploy.

## To do before going live
- [ ] Fill in your real LinkedIn URL in `PROFILE.links.linkedin`
- [ ] Confirm the four project write-ups read the way you want
- [ ] Replace `About` copy with your own voice
- [ ] (Optional) Add a real demo/repo `link` to any project
- [ ] (Optional) Add a custom domain at your host
