# PDF Studio

A browser app to merge PDFs, extract selected pages, split pages into a ZIP, and visually rearrange pages with drag and drop or accessible arrow buttons.

## Run

Serve this folder with any static HTTP server, for example `python -m http.server 8000`, then open `http://localhost:8000`. No build, API key, backend, or account is needed. Modern Chrome, Edge, Firefox, or Safari is required. Internet is required to load the pinned PDF and ZIP libraries from jsDelivr and optional Google Fonts. PDF files are processed in memory on your device, never uploaded by this app. Closing or refreshing the page clears the workspace.

## Use

1. Choose or drop one or several PDF files. Added PDFs append to the workspace.
2. Drag page cards or use their arrows to change the output order.
3. Check pages, or select positions using a range such as `1-3, 5`.
4. Download selected PDF to merge/extract in the displayed order, or split selected pages into a ZIP of one-page PDFs.

## Deploy to GitHub Pages

In the repository's **Settings → Pages**, select **Deploy from a branch**, choose **main**, **/(root)** and save. The static app works under a repository subpath.

## Limits

Password-protected/encrypted PDFs are rejected. The per-file limit is 100 MB; total capacity depends on browser memory. Bookmarks, signatures, document-level metadata, attachments and interactive form behavior are not guaranteed to survive copying pages. Originals are never changed. No analytics, file persistence or server upload endpoints are included.

Libraries: [pdf-lib](https://pdf-lib.js.org/), [PDF.js](https://mozilla.github.io/pdf.js/), [JSZip](https://stuk.github.io/jszip/).
