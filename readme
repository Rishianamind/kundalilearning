# Kal Purush Kundali

An interactive Vedic astrology learning tool. Visualize how a native's kundali overlays on the **Kal Purush** blueprint — the cosmic chart where Aries naturally rules H1, Taurus H2, and so on.

No backend, no birth-data calculation. This is a teaching aid, not a prediction tool.

## Features

- **Side-by-side charts** — Kal Purush (fixed) and native (rotates with lagna)
- **North Indian and South Indian** styles
- **Place planets** manually with one-click chip + house selection. Rahu/Ketu auto-axis.
- **Dignity badges** — exalted, mooltrikona, own sign, debilitated
- **Combustion (C) and retrogression (R)** toggles per planet, with descriptive notes
- **Drishti view** — visualized planetary aspects with planet-color-coded arrows
- **Dispositor chain** — trace each planet through its sign-lords to its anchor
- **Bhavat Bhavam** — read any house as the new 1st house. Built-in derivative readings for spouse, mother, father, children, etc.
- **Karakas** — natural significators per house
- **Yoga detection** — Gaja Kesari, Budha-Aditya, Vish, Grahan, and a dozen more

## Run locally

Just open `index.html` in a browser. No build step, no dependencies.

```bash
git clone <your-repo-url>
cd <repo>
open index.html      # macOS
# or: xdg-open index.html  on Linux
# or: start index.html     on Windows
```

## Deploy on GitHub Pages (free, permanent URL)

1. Create a new repository on GitHub (public).
2. Upload `index.html` and `README.md` to it (or commit them locally and push).
3. In the repo, go to **Settings → Pages**.
4. Under **Source**, choose `main` branch, `/ (root)` folder.
5. Save. Wait 1–2 minutes.
6. Your app is live at `https://<your-username>.github.io/<repo-name>/`.

## Deploy elsewhere

- **Netlify Drop** — drag `index.html` onto [netlify.com/drop](https://app.netlify.com/drop). Instant URL, no account needed for a quick share.
- **Vercel** — `vercel deploy` from the folder.
- **Cloudflare Pages** — connect to GitHub repo, no build settings needed.

## Customization

Everything is in one HTML file. Edit the JavaScript data objects near the top of the `<script>` block:

- `signs` — rashi metadata (element, modality, lord, qualities, style description)
- `houses` — bhava titles, themes, karakas
- `planets` — grahas with dignities, aspects, friendships, karaka text
- `yogaCatalogue` — yoga/dosha detection rules
- `combustionNotes`, `retroNotes` — state-effect descriptions per planet
- `derivativeCommonReads` — Bhavat Bhavam preset readings per base house

The CSS at the top defines design tokens (`--color-*`, `--border-radius-*`) and respects `prefers-color-scheme` for light/dark mode.

## Notes on the Vedic content

- Aspects (`drishti`) modeled: Sun, Moon, Mercury, Venus all aspect 7th only. Mars 4-7-8. Jupiter 5-7-9. Saturn 3-7-10. Rahu and Ketu use 5-7-9 (a common convention; some traditions differ).
- Rahu dignities: exalted in Taurus & Gemini, debilitated in Scorpio & Sagittarius, mooltrikona in Virgo and in the **4th house**.
- Ketu dignities: exalted in Scorpio & Sagittarius, debilitated in Taurus & Gemini, mooltrikona in Pisces and in the **10th house**.
- Combustion is user-toggleable since it requires actual planet-Sun degree distance to compute; treat it as a "what-if" study tool.
- Retrogression is similarly toggleable. Sun, Moon, Rahu, and Ketu cannot be retrograde in this model; Moon cannot be combust either by design (the chip toggles are hidden where not applicable).

## License

MIT — do whatever you want. Attribution appreciated but not required.

## Credits

Built iteratively as a learning tool. If you spot Vedic content errors or want to add features (sample charts, friendship grid, synastry, Raja-yoga detector, etc.), PRs welcome.
