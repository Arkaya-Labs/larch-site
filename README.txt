Larch site (larch-engine.com)

Plain static HTML with no build step. Serve this folder, e.g. `python3 -m http.server 8000`, then open
http://localhost:8000. Opening index.html straight from disk also works, but browsers block WebGL from
reading files there, so the stars and the lit tower window will not move.

- vercel.json: no build step. The install commands download the installers straight from the latest
  GitHub release of Arkaya-Labs/Larch, so no redirects are needed. When Windows and Linux builds ship,
  update the install note, the hardware question and operatingSystem in the JSON-LD.
- Search and AI crawlers: the <head> has a canonical URL, Open Graph and Twitter card tags (card image
  assets/og/larch.jpg) and JSON-LD (SoftwareApplication, FAQPage, VideoObject). Keep the FAQ JSON-LD in step
  with the Questions section. robots.txt, sitemap.xml and llms.txt sit next to index.html.
- Larch is one product: an AI engine with a built-in agent. Don't present "Larch engine" and "Larch" as two
  products.
- demos.js: the demo carousel. To add a recording, set a demo's videoSrc and posterSrc and add its tab
  button in index.html. A demo without a recording shows an animated concept (assets/demos/<key>.gif).
- styles.css: the Arkaya Labs site's stylesheet plus the Larch section at the end.

Footer: "Copyright 2026 the Arkaya Labs authors".
