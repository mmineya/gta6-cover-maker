# AFTER HOURS — Cover Art Studio

An original, offline, multi-panel crime-poster studio. Your photos never leave your device. MIT licensed.

Open `app/index.html` directly in desktop Chrome, or run `node serve.ts` and visit `http://localhost:8080`. No installation, build step, dependencies, API, or network connection is needed.

Drop one or more images, edit your headline and tagline, choose Fracture, Classic, or Cinema composition and one of four color stories. Click a panel to select it, click a photo thumbnail to assign it, drag to reframe, and adjust zoom. Numbered panel buttons and the content selector make every panel accessible. Use “Use this photo in every panel” to build from a single photo; each crop stays independent. Horizontal and vertical sliders or arrow keys position the selected photo precisely. Original scenery can be restored per panel. Optional local comic-ink processing and deterministic print grain are included. Export a real PNG at 1080×1080, 1080×1350, or 1920×1080.

The city, convertible, helicopter, and palms are original Canvas artwork. The two sample photos are supplied by the competition starter and permitted for reuse. A compact embedded copy in `app/src/sample-data.js` keeps Canvas untainted when the editor is opened directly via `file://`; user photos use local object URLs. Anton and Barlow Condensed are open-license fonts with their SIL OFL licenses included in `app/fonts/`. No official game art, logos, or fonts are used.

`node main.ts` packages the app and screenshots into `/output`. For a local build use `MAKEFUN_OUTPUT_DIR=out node main.ts`. The vendored packaging helper is unchanged.

Verified in Chromium: offline direct-file startup, multiple-image upload, title/tagline editing, compositions and grades, zoom/recenter/shuffle/reset, mobile overflow, and PNG signatures and dimensions for all three export sizes. Screenshots show actual browser renders, not mockups.

Screenshot handoff: open `/?shot=editor` for the workspace, `/?shot=cover` for the square cover, `/?shot=cover&size=1080x1350&grade=neon&caption=NEON%20RUNAWAY` for a portrait, or `/?shot=cover&size=1920x1080&grade=gold&layout=blocks&caption=GOLDEN%20OUTLAWS` for a landscape. Set the viewport to the export dimensions for cover-only captures. `window.__shotReady === true` means fonts and samples are painted. Use the Download PNG button for the actual exported cover.
