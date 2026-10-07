# Birdkanfly Aviation Website

A multi-page marketing website for a flight-training academy in Mysore.
It presents training programs, aircraft, admissions and contact information using Astro,
Tailwind CSS, Alpine.js and GSAP.

## Site map

| Route | Purpose |
| --- | --- |
| `/` | Academy introduction and program highlights |
| `/about` | Academy background |
| `/programs` | Training offerings |
| `/fleet` | Aircraft presentation |
| `/admissions` | Admissions information |
| `/contact` | Contact details and enquiry UI |

Pages are authored in [src/pages](src/pages); shared navigation and footer live in
[src/components](src/components). [Layout.astro](src/layouts/Layout.astro) wraps the pages.

## Local development

```bash
git clone https://github.com/DanushArun/birdkanfly.git
cd birdkanfly
npm ci
npm run dev
```

Open `http://localhost:4321`.

```bash
npm run build
npm run preview
```

The production build is written to `dist`. Dependencies are recorded in the package lockfile.
The repository has no test script or committed application backend.

## Content and verification

Academy accreditation, flying-day counts, course details and contact information are site copy.
This repository review does not independently verify those business claims.
Check them with the academy before publishing changes.

README links and package scripts were reviewed. No admissions submission, browser acceptance
suite or live hosting check was performed for this documentation update.
