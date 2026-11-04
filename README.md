# www_agent_sec — WASST 2027 website

This is the complete upload source for the `www-agent-sec/www-agent-sec.github.io` repository.
Expected website address: **https://www-agent-sec.github.io/**.

## Upload and publish

1. Upload all files and the `organisers/` folder in this directory, including `.nojekyll`, to the repository root.
2. Keep `index.html`, `styles.css`, `script.js`, the background image, favicon, fonts, font license, artwork prompt, and photo source record in the root. Keep the eight organiser portraits inside `organisers/`.
3. Verify that the page files and all eight portrait images are present before committing.
4. In **Settings → Pages**, use **Deploy from a branch**, `main`, and `/(root)`.
5. After deployment completes, open **https://www-agent-sec.github.io/**.

The original reviewed website content, layout, styles, JavaScript, and binary assets are preserved. Only the resource paths in `index.html` and `styles.css` have been changed to point to the flat directory structure. The workshop title remains WASST 2027.

---

# WASST 2027 workshop website

Local, responsive English website based on the supplied WASST 2027 workshop proposal and the layout of the Audio-AAAI 2027 reference site.

## Preview

Open `index.html` directly, or start a local server from this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Then visit http://127.0.0.1:8765.

## Files

- `index.html`: all workshop content; edit text, dates, email addresses, and submission details here.
- `styles.css`: responsive layout, type, colours, and spacing.
- `script.js`: mobile menu and current-section navigation.
- Root-level artwork, favicon, PT Sans font files, font license, and artwork prompt accompany the HTML, CSS, and JavaScript.

No build step, package installation, analytics, cookies, or external network requests are required. All assets use relative URLs so the site can later be hosted under a GitHub Pages repository path.

## Content status

The supplied PDF is a workshop proposal. The website preserves that status. Its sections follow the supplied Audio-AAAI reference: About, Topics, Submission Requirements, Format of Workshop, Attendance, Important Dates, and Workshop Organisers. At the user's request, Submission Requirements is concise and links directly to the official conference Workshops page. That link is labelled as official information, not a WASST paper submission portal. Conference information is supplemented from the official The Web Conference 2027 website, checked on 18 October 2026.

The conference is in Dublin, Ireland, 10–14 May 2027. The website explicitly labels that range as the parent conference dates and links it to the official announcement. Submission and publication guidance is provided through the official Workshops link; the site does not invent WASST-specific rules or a paper submission portal. Attendance links to the official Attending page. Important Dates links directly to the official timeline and programme, following the user's preference to keep changing deadlines at their official source.

Official sources:

- Conference city and date range: https://www2027.thewebconf.org/research-track-papers/
- Workshop paper timetable: https://www2027.thewebconf.org/important-dates/
- Workshop publication policy: https://www2027.thewebconf.org/workshops/
- Session programme status: https://www2027.thewebconf.org/programme/
- Attendance and registration updates: https://www2027.thewebconf.org/attending/

The official timeline was checked on 18 October 2026; it then listed workshop paper submission on 4 January 2027, author notification on 1 February 2027, and final version on 16 February 2027, with deadlines at 23:59 AoE. These dates are not duplicated in the page's Important Dates section; visitors follow the official link for the latest version. This is a source-link approach, not automatic data fetching. The 4-page ACM format and OpenReview link on the official Workshop CFP concern workshop proposals, so they are not used as WASST paper submission requirements or portal.

Keynote / invited speaker information and program committee members are omitted. The original PDF is deliberately not bundled, since it contains those excluded sections. Organiser affiliations and professional contact addresses come from the supplied PDF.

Attendance includes the PDF's estimate of 50–60 on-site participants, as the reference site also includes an attendance estimate. Submission-count estimates, acceptance-rate estimates, and resource requests are omitted. There is no extra contact section; professional contact addresses are provided with the organisers.

## Typography

PT Sans is distributed under the SIL Open Font License. See `PT-Sans-OFL.txt`.

The hero uses PT Sans Bold, while the main text and section headings use Arial, following the reference site's actual typography. Desktop text follows the reference's approximately 18.7 px body / 48 px section heading scale and 70 px content inset. Attendance is its own section.

## Background artwork

`hero-web-v2.png` was generated with the built-in image generation tool as an original, sharp blue/violet web-network visual. The generation prompt is preserved in `hero-web-v2-prompt.txt`.

The hero applies a gradual dark overlay to the lower portion so bright points remain visible without glare. The image file itself is preserved.

## Organiser photographs

Eight local WebP portraits accompany the organisers, with a two-column desktop layout and a single-column layout on phones. Xueyi Zhang's portrait was extracted from the user-supplied TICI2026 workbook, Sheet1 row 7. Other portraits come from the organisers' academic profiles, research centres, or the ICCV 2025 tutorial website. See `organiser-photo-sources.json` for the source record. Images are cropped and resized without changing facial features. The workbook itself is not bundled.
