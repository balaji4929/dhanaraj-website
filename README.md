# Rainbow Puppetry — Dr. N. Dhanaraj

## Structure
```
index.html      Main site (3D interludes, gallery, story)
archive.html    Full photo archive (filterable)
images/         All photographs
videos/         show.mp4, show2.mp4
js/             three.module.min.js (3D engine — do not delete)
```

## Adding photographs to the ARCHIVE

1. Drop the file into `images/`
2. Open `archive.html`, find the `const ARCHIVE = [` list
3. Add one line:

```js
{ src:"images/g23.jpg", cat:"performances", caption:"Your caption here" },
```

Categories: `performances`, `classrooms`, `honours`, `archival`, `people`
(Invent your own — filter buttons build themselves automatically.)
Leave `caption:""` if you don't have one yet.

## Adding photographs to the HOME gallery
Open `index.html`, find `<div class="pgrid" id="pgrid">`, copy an existing
`<figure class="ph tilt">` line and change the filename.
Then update the count in the tab: `Photographs <sup>21</sup>`

## Notes
- Must be served over http(s) — Netlify is fine. Opening index.html
  directly from the file manager may not show the 3D scenes.
- Keep the `js/` folder — the 3D interludes need it.
