# Mahjoub Academy

A responsive, static course website based on the supplied Control Valve General Course outline. Includes all eight source modules, curriculum search and day filters, browser-local outline review progress, an illustrative valve characteristic lab, a proposed four-day schedule, instructor details and the original Word download.

## Run

Requires Node.js 20 or later. No dependencies or installation needed.

    npm run dev

Open http://127.0.0.1:4173. Run `npm run build` to validate. The deployable website is in `dist/`.

## Vercel

Import the Git repository in Vercel. Framework: Other; build command: `npm run build`; output directory: `dist`. These settings are included in vercel.json. Alternatively run `npx vercel --prod` from this directory with an authenticated Vercel account.

## Content and scope

The supplied document is a syllabus, not a full lesson textbook. Module wording, duration, prerequisites, audience and instructor bio come from the source. The four-day allocation is proposed. The lab is illustrative at constant pressure drop, not an engineering sizing calculator. Equal percentage uses rangeability 50, linear uses x, quick opening uses sqrt(x); no manufacturer performance is implied. No invented enrollment, payment, certification, reviews or contact information. Mahjoub Academy is the user-approved educational identity. Fonts use Google Fonts with local system fallbacks. Progress is saved only in the current browser; no accounts or server storage.

## Language and appearance
The complete interface and all eight module outlines support Turkish and English. The header language selector and valve-inspired light/dark switch save preferences in this browser. The original downloadable Word syllabus remains English. The theme follows the system preference until the visitor chooses a theme.

## Enrollment setup

The inquiry form validates name and email and currently downloads a text draft; it does not submit or store leads. Configure the academy-approved email and/or international WhatsApp number in `dist/contact-config.js` when available. Configured channels open a draft for the visitor to review and send; there is no automatic email, database or payment. Keep the contact values empty until approved. The original syllabus is English; the interface and module outline are bilingual.

## Course PDFs
Two separately localized, five-page course programs are included in dist/mahjoub-academy-course-en.pdf and dist/mahjoub-academy-course-tr.pdf. Both download links follow the selected site language. The four-day allocation is identified as suggested. The source Word remains in the repository for reference.

## SEO and measurement

Run `npm install` once and `npm run build`. Edit the page template in `src/index.html`; build.mjs generates fully rendered English and Turkish pages under /en/ and /tr/. Assets remain in dist/. Both routes include all eight modules before JavaScript, canonical and reciprocal hreflang, social metadata and Course/EducationalOrganization JSON-LD. Root canonicalizes to /en/. robots.txt, sitemap.xml and a factual llms.txt are generated. Change the origin in build.mjs when adopting a custom domain. Course dates, prices and accreditation are not invented. FAQ content describes known facts and explicitly unknown logistics. llms.txt is supplementary and gives no ranking guarantee.

Measurement IDs remain empty in dist/measurement-config.js pending owner input. There is no live Analytics or Ads reporting yet. Basic consent prevents loading Google tags until relevant consent; personalization stays denied. Privacy preferences can be changed from the footer. No names, emails, form messages, or arbitrary query parameters are sent by the custom tracking. Disable automatic form interactions/enhanced measurement in the real GA4 property before activating it; the intended events are explicit and contain only enumerated language/channel values. Ads IDs and the conversion label are reserved, but no conversion is fired until an actual server-confirmed lead flow is implemented. A download or draft opening is not a completed lead. This site does not create or run paid campaigns.

Events prepared: syllabus_download, enrollment_cta, inquiry_draft_download, contact_intent. Consent and preference tests passed with measurement disabled; actual Google delivery must be checked with Tag Assistant and GA4 DebugView once real IDs are supplied. Search Console ownership verification and sitemap submission remain owner-account tasks; no indexing or rank is guaranteed.
