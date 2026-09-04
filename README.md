# Cashew price survey

A single-page form for logging cashew price observations in the field, matching
the "Price Survey" tab of the Cashew Market Survey template.

## Run it

No build step, no dependencies. Two options:

**Option 1 — just open it**
Double-click `index.html`, or right-click it in VS Code and choose
"Open with Live Browser" / "Reveal in File Explorer" and open in your browser.

**Option 2 — Live Server (recommended)**
1. Install the "Live Server" extension in VS Code (by Ritwick Dey).
2. Right-click `index.html` → "Open with Live Server".
3. It opens at something like `http://127.0.0.1:5500` and auto-reloads on save.

## Data storage

Entries save to the browser's `localStorage`, scoped to whichever origin you're
viewing it from:

- Opening the file directly (`file://...`) and opening it via Live Server
  (`http://127.0.0.1:...`) are **different origins** to the browser, so they
  keep separate data. Pick one method and stick with it.
- Data lives in that browser only — it won't show up if you open the same file
  in a different browser or a different computer.
- Clearing your browser's site data/history for that origin will erase it.

Use the **Export CSV** button regularly to back up your entries outside the
browser — it writes a CSV in the same column order as the original survey
template, ready to paste back into the workbook.

## Files

- `index.html` — everything: markup, styles, and logic in one file.
