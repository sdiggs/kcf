# Keeling Curve Foundation, hero mockup

This repo holds a single self-contained HTML mockup of a redesigned hero section for the Keeling Curve Foundation. It reimagines the top of [keelingcurve.org](https://www.keelingcurve.org/) with a fresh color palette and a live "observation feed" carousel, so a visitor sees the planet's current signals the moment the page loads.

## What it is

`kcf-hero-mockup.html` is one file. No build step, no dependencies, no framework. Open it in a browser and it runs. Fonts load from Google Fonts, and everything else (layout, illustrations, and interaction) lives in the file.

The design treats color as data. A thermal ramp moves from cool cyan through dawn gold to warm coral, sitting on a deep Mauna Loa night palette, so the accent colors carry meaning instead of decoration. Type pairs Instrument Serif for display, IBM Plex Sans for body, and IBM Plex Mono for the instrument-style readouts.

## The carousel

Six slides cycle through current climate signals:

1. **Live ocean conditions** from earth.nullschool.net, showing surface currents and sea surface temperature over the Gulf Stream
2. Sea surface temperature anomaly
3. Harmful algal bloom
4. Coral bleaching
5. Arctic sea-ice minimum
6. The real Scripps CO₂ Program animation, stepping through timescales from the past week to the full Mauna Loa record

Slides one and six carry real data: the nullschool globe and the Scripps CO₂ animation. The other four are hand-built SVG scenes with invented figures, each flagged "illustrative, mock data." The carousel advances on its own, pauses on hover, and answers arrow keys as well as its own dot and arrow controls. It lingers about four to five seconds on the Scripps plot and restarts that animation each time the slide comes around.

## Accessibility

The mockup ships responsive down to mobile, with visible keyboard focus, ARIA labels on the carousel, and reduced-motion support that stops the autoplay and ambient animation.

## Links

- This repo: [github.com/sdiggs/kcf](https://github.com/sdiggs/kcf)
- The real foundation site: [keelingcurve.org](https://www.keelingcurve.org/)
- Live nullschool view: [ocean currents and SST over the Gulf Stream](https://earth.nullschool.net/#current/ocean/surface/currents/overlay=sea_surface_temp/grid=on/orthographic=-67.47,38.26,2400/loc=-67.801,39.446)

## A note on the embed

The live globe loads fine in a normal browser. Some sandboxed preview panes block nested iframes, so if the globe ever looks blank, the "Live, nullschool" badge in the viewport opens the same view on the real site.

*Last updated July 10, 2026.*
