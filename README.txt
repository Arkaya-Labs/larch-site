Larch site (larch-engine.com)

Plain static HTML with no build step. Serve this folder, e.g. `python3 -m http.server 8000`, then open
http://localhost:8000. Opening index.html straight from disk also works, but browsers block WebGL from
reading files there, so the stars and the lit tower window will not move.

- vercel.json: no build step. Until launch day (26 Nov 2026) the page has no GitHub, docs or install
  links; the launch-day change adds them and the /install.sh and /install.ps1 redirects.
- demos.js: the demo carousel. To add a recording, set a demo's videoSrc and posterSrc and add its tab
  button in index.html. Until then each demo shows an animated concept (assets/demos/*.gif).
- styles.css: the Arkaya Labs site's stylesheet plus the Larch section at the end.

Footer: "Copyright 2026 the Arkaya Labs authors".
