# App Catalogue — Ahmed ElFirgany

A single public page that shows the mobile apps I have shipped: what each one does,
the hard engineering problem behind it, and a store link you can open right now.

**Live:** https://saqrelfirgany.github.io/apps-catalogue/

## How to change it

Everything lives in **`data.js`**. `index.html` never needs editing.

- `internal:true` replaces the store buttons with a note that the app runs inside a
  client's company. Use it for systems with no public listing.
- Leave `shots:[]` and the gallery shows a short note instead of an empty box.
- Every number here must exist in `canon.yml` in the Brand HQ. No hand-typed numbers.

## Images

Screenshots and icons are the **public store listing images**, loaded straight from
Google's and Apple's CDNs. Nothing is copied into this repo.

If a store image ever changes or disappears, the page does not break: a failed icon
falls back to an initials tile, and a gallery whose images all fail is replaced by a
one-line note. That behaviour is deliberate — a broken image on a portfolio reads worse
than no image.

## Language

Arabic and English, toggled from the top right. The choice is remembered, and it is in
the URL, so `?lang=ar` sends someone straight to the Arabic version.

