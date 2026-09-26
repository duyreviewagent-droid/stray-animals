# Stray Animals

A survival story in four lives, in one self-contained page.

Three animals with nobody coming to feed them — a cat washed into the
storm drains, a dog waiting at the end of a logging road, a rat in the
neon — and a fourth route, the council sweeper with a stick and a quota,
which only opens once all three animals have reached an ending.

58 chapters, 12 endings, 47 trophies, a leaderboard, and a tutorial you
can take as any animal in any map.

Everything is generated in the browser at load. There are no image files
and no audio files: the textures are painted onto canvases and their
relief is read back out of them, the voices are formant-synthesised, the
purr is built pulse by pulse across both halves of the breath, and the
score is written as you play.

## Play

- **On the web:** https://stray-animals.onrender.com
- **On a Mac:** run `mac/build.sh`, then open `Stray Animals.app`. It
  plays offline — the whole game is inside the bundle.

## Layout

    web/public/       the entire game (index.html + vendor/three.min.js)
    render.yaml       Render Blueprint: a free static site
    mac/build.sh      builds Stray Animals.app around web/public
    mac/main.swift    a WKWebView that serves the game over stray://

`mac/icon-1024.png` is drawn by the game itself — open the page with
`?icon=1&data=1` and it hands back the PNG.

## Controls

WASD moves relative to the camera, the arrow keys move on the world's own
axes. Space jumps, C crouches, E uses, Q calls, F is your species' sense,
O and L climb a ladder, V switches between third person and the animal's
own eyes, Tab advances dialogue. Click any ground to walk there.
