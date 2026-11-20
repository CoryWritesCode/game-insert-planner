# Game Insert Planner

A single-page tool for building board game box inserts out of foam board, plywood or MDF.

Enter the inside of the box, the components you want to store and the sheet material you cut, or start from one of ten popular games (7 Wonders, Azul, Carcassonne, Catan, Everdell, Pandemic, Splendor, Terraforming Mars, Ticket to Ride, Wingspan). The example sizes come from insert makers' published fit specs and real card sizes; token and tile trays are estimates, so measure your own copy before cutting. The page:

- lays out one open-top tray per component, stacking shallow trays only when needed and closing gaps so nothing slides around
- lists every tray with its inside and outside size
- leaves an open space with no tray for anything that keeps its own shape, like a dice tower, and packs the trays around it
- builds a grouped cut list you can copy into a spreadsheet
- nests the pieces onto your sheets with as little material as it can, allowing for the blade kerf. Each sheet is cut into full-length strips first, then each strip is cut across into pieces, so every cut runs edge to edge and matching pieces sit side by side. Whatever is left comes off as one full-length offcut.
- lists the cutting order for each sheet: strip widths, then the lengths to cut from each strip
- downloads a full-size PDF cutting template: a cutting plan per sheet plus template cards on Letter, A4, Tabloid or A3 paper, or one full-size page per sheet for a print shop. Cards break only where you cut, so a piece prints whole on one page unless it is bigger than the page.

Inputs are saved in the browser's local storage. There is no backend.

## Run locally

It is one static file with no build step. Open `index.html` in a browser, or serve the folder:

```sh
npx serve .
```

## Deploy

Any static host works. On Vercel, import the repo with the "Other" framework preset and no build command; `index.html` is served at the root.

## Dependencies

Loaded from CDNs at runtime:

- [jsPDF 2.5.1](https://github.com/parallax/jsPDF) for the PDF template
- Google Fonts: Archivo, IBM Plex Sans, IBM Plex Mono
