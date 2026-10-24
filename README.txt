POCKET READER — UPDATED BUILD

Features
- Night / dark, light and sepia themes
- Higher-resolution PDF canvas rendering using device pixel ratio
- Continuous vertical scrolling and single-page layout
- Text Reader mode for selectable-text PDFs, with adjustable font size, line spacing and margins
- Zoom controls for original PDF pages
- Bookmarks, saved last-page progress and a local bookshelf
- Search inside text-based PDFs
- Table of contents / PDF outline when the document contains one
- Reader engine cached in browser storage after first successful online load; app shell cached by the service worker

Install/update using GitHub Pages on Android
1. Extract this ZIP on your phone.
2. Upload/replace index.html, manifest.json, sw.js, icon.svg in the root of your existing GitHub Pages repository.
3. Commit the changes and wait for GitHub Pages to publish.
4. Open your existing Pocket Reader URL in Chrome. Refresh the page. If the old version still appears, Chrome > site info > Site settings > Clear data for that site, then reopen it. Clearing site data also removes books saved at that site, so export/back up important PDFs first.
5. Use Chrome's menu > Install app / Add to Home screen if needed.

Important notes
- This is a Progressive Web App (PWA), not a signed Android APK.
- Keep the PDF rendering engine online for the first use. The app tries to cache the engine files in browser Cache Storage after downloading them so later use can work offline; browser or site-data clearing may remove these caches.
- Adjustable fonts work in Text Reader mode and only when the PDF contains extractable text. Scanned pages and image-only PDFs keep their original page layout; OCR is not included.
- Dark mode inverts PDF page colors to reduce glare; that can alter the look of photos and colored diagrams. Use light or sepia when color fidelity matters.
- Books are stored locally in this browser's IndexedDB. Clearing site data can delete the library and reading progress.
