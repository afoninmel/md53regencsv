# md53regencsv

This repository contains a static browser-based CSV comparison page that can be hosted on GitHub Pages.

## Usage

1. Open `index.html` in a browser.
2. Upload the Beekai CSV and the Power Automate CSV.
3. Click **Compare files**.
4. The page shows rows from the Beekai CSV that do not appear in the Power Automate CSV by comparing shared columns.

> All processing happens in the browser. No files are uploaded to a server, and reloading the page clears all data.

## GitHub Pages

To host this page for free on GitHub Pages, enable Pages for this repository and use the root branch. The entry point is `index.html`.

The URL will be:

`https://afoninmel.github.io/md53regencsv/`

## POST Request Support

After you compare files and missing rows appear, select one row in the results table. Enter a destination URL and click **Send selected row**. The page sends the selected row as JSON via HTTP POST from the browser.

> The destination endpoint must accept CORS requests from the static page for the POST to succeed.
