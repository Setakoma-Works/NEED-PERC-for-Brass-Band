# 🥁 NEED-PERC for Brass Band

> A single-page app to track, aggregate, and manage percussion requirements for brass band concerts.

No server. No install. Just open `index.html` in a browser.

---

## What It Does

When a concert program is finalized, figuring out which percussion instruments are needed — across all pieces, without duplicates — is surprisingly tedious. NEED-PERC lets you register each piece with its required instruments, mark which ones your ensemble already owns, and instantly see what needs to be rented.

Spec notes (size, octave range, material, etc.) can be attached to each instrument, so the summary doubles as a ready-to-send rental request.

---

## Features

### Tab 1 — PROGRAM
- Register pieces by name with their required percussion instruments
- Select instruments from a preset list (multi-select toggle buttons)
- **Add custom instruments permanently to the master list** via the "+ Add to Master" button
- Registered pieces are listed as cards and can be deleted individually

### Tab 2 — INVENTORY
- Mark which instruments your ensemble owns
- **Attach spec notes to any instrument** — octave range, head size, material, manufacturer, etc.
- Notes appear inline in the inventory list and carry through to the summary

### Tab 3 — SUMMARY
- All instruments across all pieces are deduplicated and sorted automatically
- Split into two lists:
  - 🟠 **Needs rental** — instruments used in the program but not owned
  - 🟢 **Already owned** — instruments your ensemble can provide
- Spec notes are displayed under each instrument in both lists
- **Print / Export PDF** button generates a clean printable report

---

## Usage

```
1. Download or clone this repository
2. Open index.html in any modern browser
3. No build step, no dependencies, no internet required
```

All data is saved automatically to `localStorage` in your browser. Nothing is sent to a server.

---

## Data Persistence

| What | Where |
|---|---|
| Registered pieces | Browser `localStorage` |
| Owned instruments | Browser `localStorage` |
| Custom master instruments | Browser `localStorage` |
| Spec notes | Browser `localStorage` |

Data persists across sessions in the same browser. Use **System Reset** (top-right) to wipe everything and start over.

---

## Screenshot

> *(Add a screenshot of each tab here)*

---

## Tech Stack

- Vanilla HTML / CSS / JavaScript — zero frameworks, zero build tools
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- [Google Fonts](https://fonts.google.com/) — Roboto Mono + Noto Sans JP

---

## License

MIT
