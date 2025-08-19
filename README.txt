# RELA QR Code Generator (Static Site)

This is a single-file web app (`index.html`) that generates a QR code that opens an SMS draft with a prefilled message.

## Features
- Inputs: address, pickup day (dropdown), optional phone number, optional note, editable message prefix
- Generates a QR that uses the `sms:` URL scheme with a prefilled body (works on iOS)
- Download QR as PNG (auto file name based on the address)
- Fully offline (no external libraries)

## Quick Deploy Options

### Option A: GitHub Pages (free)
1. Create a new GitHub repository (public).
2. Upload `index.html` to the repo.
3. In repo **Settings → Pages**, set **Source** to `main` (or default) and root folder. Save.
4. Wait ~30s, then open the site URL GitHub shows under **Pages**.

### Option B: Netlify (drag & drop)
1. Sign in at Netlify and go to the **Sites** page.
2. Drag-and-drop the entire unzipped folder onto the page to deploy.

### Option C: iCloud/Dropbox/Drive public link
1. Upload `index.html` to your cloud storage.
2. Get a **public share link**.
3. Open that share link in Safari.

## Notes
- On iOS, local `.html` files opened from the Files app may not render in Safari. Host it using one of the methods above.
- The `sms:` link format used is: `sms:+1XXXXXXXXXX&body=...` which iOS supports.
