# Keeling Curve Foundation, hero mockup

This repo holds a single HTML mockup of a redesigned hero section for the Keeling Curve Foundation. It reimagines the top of [keelingcurve.org](https://www.keelingcurve.org/) with a fresh palette and a live "observation feed" carousel, so visitors see the planet's signals as the page loads.

## What it is

`kcf-hero-mockup.html` runs on its own, with no build step or framework. Fonts load from Google Fonts. The design treats color as data: a thermal ramp from cool cyan through dawn gold to warm coral, on a deep Mauna Loa night palette, so the accents carry meaning. Type pairs Instrument Serif for display, IBM Plex Sans for body, and IBM Plex Mono for the readouts.

## The carousel

Nine slides cycle through current climate signals:

1. NASA CO2 visualization, Mauna Loa to Antarctic ice cores
2. Live ocean currents and sea surface temperature, Gulf Stream (nullschool)
3. Sea surface temperature anomaly, NE Pacific
4. NOAA NOWData temperature departure map
5. Harmful algal bloom, Monterey Bay
6. Live coral bleaching alert area (nullschool)
7. Arctic September sea-ice minimum
8. Greenland and the warming Arctic (Climate Central)
9. Scripps CO2 Program animation, past week to full Mauna Loa record

Slides 2 and 6 are live nullschool embeds. Slides 1, 4, 8, and 9 are real published sources, and the Scripps animation is embedded in the file. Slides 3, 5, and 7 are hand-built SVG scenes with invented figures, each flagged "illustrative, mock data."

The opening NASA video plays all the way through before the carousel moves on, with a timer fallback so it never stalls. Other slides advance on their own, pause on hover, and answer arrow keys and the on-screen controls. The Scripps plot holds for about seven seconds and restarts each time it appears.

## Loading and offline use

The Scripps animation is embedded, so it always shows. The NASA video, the two live globes, and the NOAA and Climate Central frames load from their web sources, so they need a connection. A sandboxed preview pane may block them, so open the file in a normal browser to see everything.

## Accessibility

Responsive to mobile, with visible keyboard focus, ARIA labels on the carousel, and reduced-motion support that stops the autoplay and ambient animation.

## Links

- This repo: [github.com/sdiggs/kcf](https://github.com/sdiggs/kcf)
- The foundation site: [keelingcurve.org](https://www.keelingcurve.org/)
- NASA source: [SVS 5447, atmospheric CO2](https://svs.gsfc.nasa.gov/5447/)

*Last updated July 19, 2026.*
