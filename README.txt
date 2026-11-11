DUST & DATE — OFFLINE EMAIL SIGNUP KIOSK

FILES
- index.html: branded customer signup screen and admin panel
- dust-date-logo.jpg: supplied Dust & Date logo, cropped for kiosk display
- manifest.webmanifest + sw.js: installable web-app metadata and offline cache

OFFLINE DATA
All email addresses are stored locally in IndexedDB on the iPad. There is NO online spreadsheet, no sync endpoint, and no network request for customer submissions. Admin can export a CSV later. Open that CSV in Apple Numbers to create/view a spreadsheet.

SETUP FOR RELIABLE IPAD OFFLINE USE
1. Upload all four files to an HTTPS static web host (same folder).
2. Open the HTTPS address in Safari on the iPad while online.
3. Wait for the page and logo to load completely; this also installs the offline cache.
4. In Safari, tap Share → Add to Home Screen.
5. Open the new Dust & Date home-screen icon.
6. Test: turn on Airplane Mode, close and reopen the home-screen app, submit a test email, and verify it is retained after closing/reopening.
Note: the initial load/install needs internet. Do not rely on opening the HTML directly from Files; iPadOS local-file storage and service-worker behavior can vary. The HTTPS-installed web app is the recommended approach.

EXPORT AFTER EVENT
1. Tap the subtle Admin link at the bottom-right.
2. Enter the admin PIN (default 2468; change CONFIG.ADMIN_PIN in index.html before deployment).
3. Tap Export CSV.
4. Open the downloaded CSV in Apple Numbers. Save as a Numbers spreadsheet if desired.
5. Verify the export before clearing Safari website data or resetting the iPad.

KIOSK LOCKDOWN
Settings → Accessibility → Guided Access → On. Set a passcode. Open the kiosk, triple-click the top button (or Home button on older iPads), and start Guided Access. Set Auto-Lock to Never during the event.

BEFORE THE EVENT
- Change the admin PIN.
- Test with several non-real addresses.
- Test in Airplane Mode, including closing/reopening the kiosk.
- Export a test CSV and open it in Numbers.
- Keep the iPad charged.
- Do not clear browser website data before exporting.
- The signup checkbox records affirmative consent to receive marketing emails. Keep the consent language visible and honor unsubscribe requests.
