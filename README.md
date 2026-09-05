# Yukai — Where stillness reveals the unseen

A five-chapter night walk up a Kyoto mountain temple, rendered live in WebGL.

Single `index.html`. No build step, no framework. Three.js r150 is vendored
alongside it, so the page runs offline straight from the filesystem.

The temple, sanmon, staircase, stone lanterns and the five-storey pagoda are all
procedural geometry — no models. Every texture is painted into a 2D canvas at
runtime. The three gallery frames and the hero window are not images: each is a
second camera on the same scene, scissored into whatever rectangle its DOM
element occupies that frame.

Sections are marked with `##` comments — `grep -n "## " index.html` for the map.
