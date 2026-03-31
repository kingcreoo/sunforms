# Sunforms

> **Bookmarked** — This project is paused and will be completed at a later date.

A simple browser-based sun/shade simulator. Place objects on a 2D canvas (houses, trees, fences) and see how shadows fall at any time of day, any date of the year, for any location on Earth.

## How It Works

- Uses the [suncalc](https://github.com/mourner/suncalc) library to calculate real sun position (altitude + azimuth) from lat/long, date, and time
- Shadows are projected using basic trigonometry — shadow length = object height / tan(sun altitude)
- Everything runs client-side in a single `index.html` file — no build tools, no backend

## Current Features

- **Objects**: Houses (rectangles), fences (lines with posts), and trees
- **Tree system**: Draw your own tree silhouette or pick from 8 templates (Oak, Pine, Palm, Willow, Cypress, Maple, Spruce, Magnolia). The silhouette is sliced into horizontal layers that each cast their own shadow at their respective height
- **Controls**: Date picker, time-of-day slider, lat/long input + browser geolocation
- **Canvas**: Pan (drag), zoom (scroll wheel), grid overlay, compass (N/E/S/W)
- **Interaction**: Click to select, drag to move, rotation handles on houses/fences, scale handles on fence endpoints, Ctrl+C/V to copy/paste, Delete to remove
- **Units**: Feet

## Usage

Open `index.html` in a browser.
