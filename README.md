# BO/PO Stock Match — South Region

This site is now **two files**:

- **`index.html`** — the page (layout, filters, PDF, WhatsApp). **This never changes.**
- **`data.json`** — the stock-match rows. **This is the only file you replace each update.**

## How to update (every other day)
1. Get the new `data.json` (generated from the day's Excel).
2. Replace the old `data.json` in your repo with the new one. Keep the name exactly `data.json`.
3. Done. The page picks up the new data automatically on refresh.

That's one small file changed — no need to touch `index.html`.

## Important
- The page reads `data.json` over the web, so **open it from its web address**
  (your GitHub Pages / Cloudflare Pages URL), not by double-clicking the file.
- Both files must sit in the **same folder**.

## Hosting note
On GitHub Pages or Cloudflare Pages there are no per-deploy charges, so replacing
`data.json` as often as you like costs nothing. (This is the fix for the Netlify
credit problem — each Netlify deploy was spending credits regardless of file size.)
