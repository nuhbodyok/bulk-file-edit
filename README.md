# File Batch Editor

A lightweight, client-side bulk file editor that runs entirely in the browser — no server, no installs, no data ever leaves your machine.

![HTML](https://img.shields.io/badge/HTML-single%20file-orange) ![No Dependencies](https://img.shields.io/badge/runtime%20deps-none-brightgreen) ![GitHub Pages](https://img.shields.io/badge/hosted%20on-GitHub%20Pages-blue)

---

## Features

- **Find & Replace** — plain text or regex, with optional case sensitivity
- **Remove Lines** — filter out lines matching a string or pattern
- **Remove Empty Lines** — strip all blank lines in one click
- **Trim Whitespace** — remove leading/trailing spaces from every line
- **Add Prefix/Suffix** — prepend or append text to each line (skips empty lines optionally)
- **Sort Lines** — ascending or descending, case-insensitive or numeric
- **Convert Case** — lowercase, UPPERCASE, Title Case, Sentence case
- **Convert Format** — CSV ↔ JSON, MD → TXT (with optional markdown stripping)
- **Batch Rename** — rename files using `[index]`, `[name]`, and `[ext]` placeholders
- **Diff View** — side-by-side comparison of original vs. modified content
- **Download** — save files individually or all at once as a ZIP
- **Copy** — copy a single file or all files to clipboard
- **Search** — filter and highlight results across all processed files
- **Dark mode** — follows your OS preference automatically

---

## Supported File Types

`.txt` `.md` `.csv` `.json` `.html` `.css` `.js`

---

## Usage

### Hosted on GitHub Pages

Just open the page — no setup needed.

### Run Locally

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
# Open index.html in any modern browser
open Bulk_File_Editor.html
```

No build step, no `npm install`, no dependencies to manage.

---

## How It Works

1. **Import** — select one or more files using the file picker
2. **Select operation** — choose what to do and configure the parameters
3. **Apply** — click *Apply Changes* to process all files at once
4. **Review** — inspect previews, open the diff view, search across results
5. **Export** — download individually or as a ZIP

All processing happens in your browser using the [File API](https://developer.mozilla.org/en-US/docs/Web/API/File_API). Nothing is uploaded anywhere.

---

## External Libraries

Loaded from CDN at runtime — no local copies needed:

| Library | Purpose |
|---|---|
| [Tailwind CSS](https://tailwindcss.com/) | Styling |
| [JSZip](https://stuk.github.io/jszip/) | ZIP file creation |
| [FileSaver.js](https://github.com/eligrey/FileSaver.js) | Browser download trigger |
| [diff](https://github.com/kpdecker/jsdiff) | Line-by-line diff engine |

---

## Browser Compatibility

Works in any modern browser (Chrome, Firefox, Edge, Safari). Requires JavaScript enabled. No polyfills needed.

---

## License

MIT — do whatever you like with it.
