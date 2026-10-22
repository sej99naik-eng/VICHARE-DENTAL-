# Vichare Dental Clinic – Patient Records app (iPhone and Android)

Patient registration, medical and dental history, and signed treatment consent.
It installs on iPhone and Android from a link, works without internet, and keeps
records only on the phone where it is used.

## 1. Put the app online (once, free, about 10 minutes)

1. Sign in at https://github.com (create a free account if needed).
2. Click **New repository**. Name it `vichare-dental`, choose **Public**, and create it.
   Public is needed for free hosting. Only the app itself is public: patient records
   are never uploaded anywhere, they stay on each phone.
3. On the new repository page click **uploading an existing file**, drag in all the
   files from this folder, and click **Commit changes**.
4. Open **Settings → Pages**. Under *Build and deployment* choose
   **Deploy from a branch**, pick **main** and **/(root)**, and click **Save**.
5. After a minute or two the page shows your app's link, like
   `https://YOUR-NAME.github.io/vichare-dental/`. That link is what staff open.

## 2. Install on each phone

**iPhone (must use Safari):** open the link → tap the **Share** button →
**Add to Home Screen** → **Add**. Open the app from the home screen icon from then on.
Records typed in Safari itself are kept separately from the installed app, so install first.

**Android (Chrome):** open the link → tap **Install app** on the banner, or the
⋮ menu → **Install app** / **Add to Home screen**.

After the first open, the app works without internet.

## 3. Keep records safe

- Records live only on that phone. If the phone is lost, reset, or the app is
  deleted, its records are gone.
- Tap **Backup** on the patient list every week (or every day) and save the file to
  Google Drive, iCloud Drive, email, or a computer.
- On a new phone, install the app and tap **Restore** to load a backup file.
- Two phones do not share records automatically. To move records between them,
  back up on one and restore on the other.

## Updating the app

Edit `index.html` (the consent wording is under "Patient declaration"), then in
`sw.js` change `VERSION` (for example to `vdc-1.0.1`), and upload both files again.
Phones pick up the new version the next time the app is opened twice.
Records are not affected by updates.

## Files

- `index.html` – the whole app
- `sw.js` – lets the app work offline
- `manifest.webmanifest` and the `icon-*.png` files – home-screen name and icon
