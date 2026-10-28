# Portfolio redesign — first working version

A fast, static, nature-inspired software development portfolio for GitHub Pages. No build step or external dependencies. The new HTML, CSS, JS and SVG were created for this redesign; the forest background is copied from the existing portfolio.

## Preview locally

- Open `index.html` in your browser, or use VS Code Live Server.
- Alternatively, from this folder run `python -m http.server 8000` and open http://localhost:8000.

## Before publishing — verify these items

1. **Name:** The old source uses `Erik Dahlberg`, but you mentioned that your name was misspelled. To avoid preserving an unverified surname, the new page says **Erik**. Replace it with your preferred full name and update the page title, meta description, and footer if needed.
2. **Contact:** In `index.html`, search for `YOUR_EMAIL@gmail.com` and replace **both occurrences** with your actual Gmail address (one is displayed on the page, the other is in the `mailto:` link). Until you replace them, the contact email is a placeholder. Old phone, street address, date of birth, and age remain removed; GitHub is also linked.
3. **Education:** Check whether "upper-secondary diploma" and "vocational software development studies" accurately describe your credentials. Add exact qualifications/dates only when confirmed.
4. **Military experience:** Verify the description is suitable for public disclosure and accurately represents your duties.
5. **Unity game:** "Ward Defense" is marked as a **working title** and **in development**; add real screenshots, the definitive project name, and a link to its repository or demo once ready.
6. **Hero image:** The original forest background `assets/img/hero-bg.jpg` is just 299×168 pixels. It's reused with a soft blur for now; replace `assets/img/forest-path.jpg` with a higher-resolution image you have permission to use. Verify the rights to your existing image before publishing.
7. **Language:** English is the default because you haven't selected a language; change it to Finnish or add translation if you prefer.

## Replace the old template safely

1. Make sure you're on your `portfolio-redesign` branch, and preserve any unrelated uncommitted changes.
2. Copy this new folder's files into the **root** of your cloned GitHub Pages repository, overwriting `index.html`.
3. Remove the old template assets and pages (`assets/vendor`, old CSS/JS, old subprojects, forms, `inner-page.html`, `portfolio-details.html`) once you confirm you no longer need them. IMPORTANT: the old pages contain outdated information and remain publicly accessible if left on GitHub Pages.
4. Run the site locally and review both desktop and mobile widths.
5. Run `git status`, `git add -A`, `git commit -m "Redesign portfolio"`, and `git push -u origin portfolio-redesign`.
6. Open a pull request into your **actual GitHub Pages publishing branch** (your original repository appears to use `master`, not `main`). Merge only after confirming your Pages configuration.

### License note

The new site does not import BootstrapMade template HTML/CSS/JS or vendor libraries. The old template's license and attribution obligations still apply to any old template material you choose to keep or publicly serve. Check rights for any reused photograph separately. Retain the old template files/license notices in your own archive if needed; do not pass this new design off as using the original template.

## Where to edit

- `index.html` — page copy, navigation and timeline entries.
- `assets/css/site.css` — palette (`:root`), layout and responsive styles.
- `assets/js/site.js` — mobile navigation, active section links, reveal animations.
- `assets/img/forest-path.jpg` — hero forest image.

The timeline uses inline SVG for each curved branch, based on your Paint sketch. To add another entry, duplicate a `.timeline-item` element and update its text and branch number.
