# ANCARE HEALTHCARE AT HOME

A mobile-first static website prototype for healthcare service enquiries in Bathinda, Punjab. Includes a separate **demo-only** admin interface.

## Files
- `index.html` — public website
- `style.css`, `script.js` — public styling and interactions
- `config.js` — public business/service configuration (never put secrets or customer data here)
- `admin.html`, `admin.css`, `admin.js` — demo admin interface
- `assets/` — original SVG illustrations
- Legal pages — draft informational templates

## Preview locally
Open `index.html` in a browser. For a more reliable local preview, use a local static server such as VS Code Live Server. Open `admin.html` separately to explore the demo dashboard.

## Publish the public website on GitHub Pages
1. Upload all project files and the complete `assets` folder to the root of your repository.
2. Confirm `index.html` is in the repository root.
3. Open repository **Settings → Pages**.
4. Under Build and deployment, choose **Deploy from a branch**, branch `main`, folder `/(root)`, then Save.
5. Wait for the GitHub Pages deployment status and open the exact URL shown there.
6. Test the website on mobile, including WhatsApp, call, email and form validation.

### Important about the demo dashboard
`admin.html` is a front-end prototype and is **not secure**. It uses a fake demo entry flow with no real authentication; do not enter real personal data. GitHub Pages cannot password-protect a single page just because it is named `/admin.html`. For a public static deployment, consider not uploading `admin.html`, `admin.js`, and `admin.css` until you have a secure backend, or deploy the demo separately and keep it clearly labelled.

## Update the public site
- Edit services, descriptions, images, service areas and contact details in `config.js`.
- Replace SVG illustrations in `assets/` or update the image path in `config.js`.
- Offers are intentionally empty until real terms are verified.
- Commit changes to GitHub. Pages redeploys automatically after a short delay.

## Current functional scope
- Responsive service catalogue and search/filter
- Enquiry form prepares a WhatsApp message, email draft, and copyable details
- Partnership enquiry prepares WhatsApp/email draft
- Call, WhatsApp and email links
- FAQ accordion and mobile action bar
- Demo admin screens for overview, service catalogue, offers, FAQs and settings

## Not implemented / backend required
- Secure login, admin roles and MFA
- Database persistence and live enquiry dashboard
- Real staff assignment, customer records, reports and notifications
- Secure prescription upload/storage
- Online payments, GPS, automated email delivery and real booking confirmation
- Production AI features
- Admin edits publishing to the public website

Static forms do not send or store submissions automatically. Users must manually press Send in WhatsApp or email. Prescription files must not be placed in public directories or transmitted through public URLs.

## Healthcare and privacy
Service availability and pricing must be confirmed by Ancare. Medicine services must use appropriate licensed pharmacy partners. Sample collection and clinical services must be delivered by qualified/authorised providers. Hospital attendants provide non-clinical support only and do not replace clinicians or hospital staff. For emergencies, contact local emergency services.

Legal content is draft text and should be reviewed by a qualified professional before launch. Images are for representation only; they do not depict verified Ancare staff or patients.
