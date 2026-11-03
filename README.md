# cristianodecesari.github.io

Personal academic website of Cristiano De Cesari, served by GitHub Pages.
The whole site is one static page: no framework, no build step.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The website: content, and the styles in the `<style>` block at the top |
| `cv_decesari.pdf` | The CV linked from the site |
| `assets/portrait.jpg` | Photo (720 × 900 px, 4:5) |
| `assets/*.png` | Paper figures shown under the abstracts |
| `assets/fonts/` | Source Serif 4 and Source Sans 3, self-hosted (SIL Open Font License) |
| `favicon.ico`, `assets/favicon.svg`, `assets/apple-touch-icon.png` | Browser and phone icons |

## Common updates

All edits are in `index.html`. Each part of the page starts with a comment such as
`<!-- ===== Research ===== -->`, so you can search for it.

- **Replace the CV.** Upload the new PDF with the same name, `cv_decesari.pdf`. If the content changed, also update the matching entries in the *Curriculum vitae* section.
- **Add a working paper.** Copy a whole `<article class="paper"> ... </article>` block, paste it where it should appear, and edit title, co-authors and abstract. The figure is optional: delete the `<figure> ... </figure>` part if there is none.
- **Add a PDF or SSRN link to a paper.** Put the PDF in a `papers/` folder, then replace the `PLACEHOLDER (paper links)` comment inside that paper with
  `<p class="paper-links"><a href="papers/FILE.pdf" target="_blank" rel="noopener">PDF</a></p>`.
- **Add a presentation.** In *Presentations*, copy one inner `<li> ... </li>` inside the right year, or copy a whole year block for a new year.
- **Add a CV entry.** Copy one `<li> ... </li>` in the relevant list: date on the left (`class="label"`), then the title (`class="what"`) and the place (`class="where"`).
- **Turn on hidden parts.** Search for `PLACEHOLDER`: Google Scholar, ORCID and GitHub links, the Work in progress list, and the Teaching section are ready and only need the comment markers removed. For Teaching, also un-comment its link in the menu at the top.
- **When the Bundesbank internship ends**, update the second line under the name, the *Research experience* entry, the *Currently* row in *Contact*, and the `affiliation` list in the structured data at the top of the file.
- **Change the photo.** Replace `assets/portrait.jpg` with a 4:5 image of about 720 × 900 px. Remove location data (EXIF/GPS) from phone photos before uploading.
- **Change colours or fonts.** Edit the variables at the top of the `<style>` block (`--ink`, `--accent`, ...). The dark-mode colours are right below.
- **Footer.** Update “Last updated” when you change the page.

## Preview and publish

- **Preview:** open `index.html` in a browser by double-clicking it. Everything loads from the folder, so it also works offline.
- **Publish:** on GitHub, *Add file → Upload files*, drag the changed files (folders keep their structure), then *Commit changes*. The site updates in about a minute.
