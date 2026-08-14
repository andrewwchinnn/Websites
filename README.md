# Aerolift homepage — design variants

Open `index.html` to compare all five side by side.

## How to preview (with your photos showing)

Double-clicking the HTML file works for most things. But if photos don't show up,
run a tiny local web server instead — this is the reliable way:

```bash
cd "/Users/andrewwchinnn/Documents/Claude Projects /Website" && python3 -m http.server 5173 --directory design
```

Then open **http://localhost:5173** in your browser. Press `Ctrl+C` in the terminal to stop it.
Refresh the browser after adding a photo and it appears — no restart needed.

| File | Direction |
|---|---|
| `v1.1-refined-industrial.html` | Your V1, cleaned up. Yellow/black industrial. |
| `v1.2-editorial-light.html` | White, airy, serif-led. Premium consultancy feel. |
| `v1.3-engineering-spec.html` | Technical spec-sheet. Monospace data, blueprint grid. |
| `v1.4-dark-premium.html` | Dark throughout, full-bleed photography, amber accents. |
| `v1.5-swiss-modular.html` | Strict grid, flat colour blocks. Includes a quote form. |

---

## How to add pictures

**You do not need to edit any code.** Every image on the page is a slot that currently
shows a grey box with a filename written in it. Put a file with that exact name into the
`images/` folder and it appears. Remove the file and the grey box comes back.

Same filenames work across all five variants — add each photo once and every version updates.

### Filenames to use

Put these in `design/images/`:

| Filename | Where it appears | Recommended size |
|---|---|---|
| `logo.png` | Header + footer logo mark | 400×400, transparent PNG or SVG |
| `hero.jpg` | Main hero image | 2400×1400 (v1.4), 1400×1600 portrait (v1.2, v1.5) |
| `service-mobile-crane.jpg` | Services — mobile crane card | 1200×800 |
| `service-skylift.jpg` | Services — skylift card | 1200×800 |
| `service-planning.jpg` | Services — planning card | 1200×800 |
| `project-1.jpg` … `project-6.jpg` | Projects gallery | 1600×1200 for `project-1`, 1200×840 for the rest |
| `about.jpg` | About section | 1200×1400 portrait |

### Rules of thumb

- **Format:** `.jpg` for photos, `.png` or `.svg` for the logo. If you only have `.png` photos,
  tell me and I'll switch the filenames over.
- **Size:** keep each photo under about 400 KB or the page gets slow on mobile data.
  Squoosh (squoosh.app) will shrink them without visible quality loss.
- **Crop:** the slots crop to fill, centred. Keep the crane roughly centred in frame.
- **Logo:** a transparent PNG works best. If you send me the logo file I'll build the header
  around its actual shape and colours rather than the placeholder mark.

---

## Data still needed

Everything highlighted in **yellow** on the pages is a placeholder. Here is the full list:

### Needed to go live
1. **Years operating** — or the year the company was founded.
2. **Company registration number** (the Sdn Bhd number for the footer).
3. **Max reach / boom length** for each capacity band: 25–50T, 50–150T, 150–300T, 300–500T.
4. **Certifications** — exact DOSH registration, CIDB grade, ISO if any, insurance cover and limit.
   Only what you can actually evidence.
5. **Project details** — for 5–6 jobs: project name (or client type if confidential),
   tonnage lifted, machine used, location, year. One photo each.

### Nice to have
6. Typical mobilisation time (hours) for a standard job.
7. Number of machines in the fleet — only if you're comfortable publishing it.
8. Whether you still offer **crawler cranes**. V1 advertised them; you didn't mention them,
   so I have left them out of all five variants.
9. Where enquiries should go — email inbox, WhatsApp, or a CRM.

### Deliberately left out
- **Safety statistics / LTI record.** Not published in any variant. These are only worth
  putting on a website if they are verified and you are willing to stand behind them.
- **"Lifts completed" counter.** Left out for the same reason — an invented number is a
  liability, not a selling point.

---

## Notes on what changed from V1

- Hero capacity corrected from **25–200T** to **25–500T**.
- **Skylift (20–55 m)** added as a full service — it was missing from V1 entirely.
- **Crawler cranes** removed pending your confirmation.
- Fleet section rebuilt around **capacity bands** instead of invented model names, so it is
  honest and still useful to a buyer filtering by tonnage.
- Your five trust claims (JKKP/DOSH-registered operators, qualified personnel, certified and
  inspected equipment, safety-focused operations, trusted experience) are used as a dedicated
  assurance section in every variant, and echoed in the hero and footer.
