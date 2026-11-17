# Game Insert Planner

A single-page tool for building board game box inserts out of foam board, plywood or MDF.

Enter the inside of the box, the components you want to store and the sheet material you cut. The page:

- lays out one open-top tray per component, stacking shallow trays only when needed and closing gaps so nothing slides around
- lists every tray with its inside and outside size
- builds a grouped cut list you can copy into a spreadsheet
- nests the pieces onto your sheets, allowing for the blade kerf
- downloads a full-size PDF cutting template: tiled onto Letter, A4, Tabloid or A3 pages with a scale check and page-join labels, or one full-size page per sheet for a print shop

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
