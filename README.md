# Markdown Table Generator

Build a table visually and copy clean GitHub Flavored Markdown.

**Live demo:** https://0xelitesystem.github.io/markdown-table-generator/

## Use

1. Open the page. A small example table is already loaded.
2. Click any cell and type. Press Tab to move across, and Tab in the last cell to add a new row.
3. Use **Add row** and **Add column**, or the small controls on each row and column to move or delete it.
4. Set each column alignment (Default, Left, Center, Right) from the dropdown above it.
5. Toggle **Aligned output** to switch between padded, easy to read markdown and a compact version.
6. Click **Copy** to put the markdown on your clipboard, or **Download .md** to save it.

To start from an existing table, click **Import** and paste one of:

- A markdown table (the column alignment is read back from the separator row).
- Tab separated text, which is what a spreadsheet puts on the clipboard when you copy a range.
- CSV, including quoted fields that contain commas, quotes, or line breaks.

The format is detected automatically. Pipes and line breaks inside cells are escaped correctly, so the output is always valid.

## Why this exists

Most online table builders ship a tracker, an ad, or a sign up wall, and they send your data to a server you do not control. This one is a single HTML file with no surveillance and no network calls. You can read every line, save it, and run it offline forever. It is free and MIT licensed.

## Privacy

Everything runs in your browser. Your table never leaves your machine. There is no analytics, no telemetry, no cookie, and no network request of any kind. Open the file with your network disconnected and it still works.

## Run locally

```
git clone https://github.com/0xelitesystem/markdown-table-generator.git
cd markdown-table-generator
```

Then open `index.html` in any browser. That is all it takes. If you prefer to serve it over http:

```
python -m http.server
```

Then visit http://localhost:8000/.

## Build

There is no build step and no dependency. The whole tool is one `index.html` with inline CSS and JavaScript.

## License

MIT. See [LICENSE](LICENSE).

## Related

- https://github.com/0xelitesystem/jwt-inspector
- https://github.com/0xelitesystem/eeat-signals-reference
