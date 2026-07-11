# Keeling Curve Foundation, hero mockup

This repo holds a single HTML mockup of a redesigned hero section for the Keeling Curve Foundation. It reimagines the top of [keelingcurve.org](https://www.keelingcurve.org/) with a fresh palette and a live "observation feed" carousel, so visitors see the planet's current signals as the page loads.

## What it is

`kcf-hero-mockup.html` runs on its own, with no build step or framework. Fonts load from Google Fonts. The design treats color as data: a thermal ramp from cool cyan through dawn gold to warm coral, set on a deep Mauna Loa night palette, so the accent colors carry meaning. Type pairs Instrument Serif for display, IBM Plex Sans for body, and IBM Plex Mono for the readouts.

## The carousel

Eight slides cycle through current climate signals:

1. Live ocean currents and sea surface temperature over the Gulf Stream (nullschool)
2. Sea surface temperature anomaly, NE Pacific
3. NOAA NOWData temperature departure map
4. Harmful algal bloom, Monterey Bay
5. Live coral bleaching alert area, eastern tropical Pacific (nullschool)
6. Arctic September sea-ice minimum
7. Greenland and the warming Arctic (Climate Central)
8. The Scripps CO2 Program animation, from the past week to the full Mauna Loa record

Slides 1 and 5 are live nullschool embeds. Slides 3, 7, and 8 are real published sources, and the Scripps animation is embedded in the file. Slides 2, 4, and 6 are hand-built SVG scenes with invented figures, each flagged "illustrative, mock data." The carousel advances on its own, pauses on hover, and answers arrow keys as well as its dot and arrow controls. It lingers about four to five seconds on the Scripps plot and restarts that animation each time it appears.

## Loading and offline use

The Scripps animation is embedded, so it always shows. The two live globes are iframes, and the NOAA and Climate Central frames load from their web sources, so those four need a connection. A sandboxed preview pane may block them, so open the file in a normal browser to see everything.

## Accessibility

Responsive to mobile, with visible keyboard focus, ARIA labels on the carousel, and reduced-motion support that stops the autoplay and ambient animation.

## Links

- This repo: [github.com/sdiggs/kcf](https://github.com/sdiggs/kcf)
- The foundation site: [keelingcurve.org](https://www.keelingcurve.org/)
- Live ocean view: [nullschool, Gulf Stream SST and currents](https://earth.nullschool.net/#current/ocean/surface/currents/overlay=sea_surface_temp/grid=on/orthographic=-67.47,38.26,2400/loc=-67.801,39.446)
- Live bleaching view: [nullschool, coral bleaching alert area](https://earth.nullschool.net/#current/bio/surface/currents/overlay=bleaching_alert_area/orthographic=-104.16,22.66,669/loc=-112.770,8.476)

*Last updated July 11, 2026.*
