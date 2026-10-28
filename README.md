# Control Valve Academy

A responsive, static course website based on the supplied Control Valve General Course outline. Includes all eight source modules, curriculum search and day filters, browser-local outline review progress, an illustrative valve characteristic lab, a proposed four-day schedule, instructor details and the original Word download.

## Run

Requires Node.js 20 or later. No dependencies or installation needed.

    npm run dev

Open http://127.0.0.1:4173. Run `npm run build` to validate. The deployable website is in `dist/`.

## Vercel

Import the Git repository in Vercel. Framework: Other; build command: `npm run build`; output directory: `dist`. These settings are included in vercel.json. Alternatively run `npx vercel --prod` from this directory with an authenticated Vercel account.

## Content and scope

The supplied document is a syllabus, not a full lesson textbook. Module wording, duration, prerequisites, audience and instructor bio come from the source. The four-day allocation is proposed. The lab is illustrative at constant pressure drop, not an engineering sizing calculator. Equal percentage uses rangeability 50, linear uses x, quick opening uses sqrt(x); no manufacturer performance is implied. No invented enrollment, payment, certification, reviews or contact information. FIELDNOTES is a proposed site identity, not a claimed organization. Fonts use Google Fonts with local system fallbacks. Progress is saved only in the current browser; no accounts or server storage.
