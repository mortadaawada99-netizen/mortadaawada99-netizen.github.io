# Sub-Zero Owner PWA

Installable iPhone owner dashboard for the existing Sub-Zero POS Supabase cloud database.

## What it does
- Read-only owner dashboard
- Uses the same Supabase Project URL, Publishable Key, Shop ID and Sync Secret as Windows
- Dashboard, sales, stock and debts
- Refreshes cloud data every 30 seconds
- Pulls the latest cloud state when the page is opened
- Stores the last cloud snapshot for offline viewing
- Can be installed from Safari using Add to Home Screen

## Free hosting options
Recommended: GitHub Pages, Cloudflare Pages, or Netlify.

### GitHub Pages
1. Create a GitHub account.
2. Create a new PUBLIC repository, e.g. `subzero-owner`.
3. Upload all files from this folder to the repository root:
   - index.html
   - manifest.webmanifest
   - sw.js
   - icon-192.png
   - icon-512.png
4. Open repository Settings > Pages.
5. Under Build and deployment:
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /(root)
6. Save.
7. GitHub will show a public HTTPS URL.
8. Open that URL in Safari on iPhone.
9. Tap Share > Add to Home Screen > Add.

IMPORTANT: this PWA stores the Sync Secret in browser localStorage on the device. Do not use this on a shared/public device. The Windows POS remains the main writer.

## Connection
On first launch enter the same values as Windows:
- Supabase Project URL
- Publishable Key
- Shop ID: subzero-main
- Sync Secret

The Windows POS must have uploaded a cloud copy at least once.
