# LearningNuclearMedicine.com

Case-based education in PET, SPECT, and molecular imaging.  
Free. Evidence-based. Built for residents, fellows, and nuclear medicine physicians.

## Site Structure

```
index.html                    → Home page
how-to-read-a-pet.html        → Systematic approach guide
tracers.html                  → Tracer library
normal-variants.html          → Normal variants by tracer
reporting-criteria.html       → Deauville, PERCIST, PROMISE, etc.
virtual-classroom.html        → Recorded sessions
about.html                    → About the contributors

cases/
  index.html                  → Filterable cases index
  case-001-hodgkin.html
  case-004-dotatate.html
  ...

assets/
  style.css                   → Shared styles (nav, footer, base)
  images/                     → Site images
```

## Adding a New Case

1. Copy `cases/case-004-dotatate.html` as a template
2. Rename it: `cases/case-XXX-diagnosis.html`
3. Fill in the clinical history, scan details, images, findings, diagnosis, pearls, differential, references
4. Add a card to `cases/index.html` with the correct `data-tracer`, `data-system`, `data-diff`, and `data-title` attributes
5. Upload to GitHub → site updates within ~30 seconds

## Metadata Tags (for filtering)

Each case card in `cases/index.html` must have:
```html
data-tracer="FDG"           <!-- FDG | DOTATATE | PSMA | Amyloid | Tau | FET | NaF | MIBG -->
data-system="Oncology"      <!-- Oncology | Neurology | Cardiac | Thyroid | Infection -->
data-diff="Intermediate"    <!-- Beginner | Intermediate | Advanced -->
data-title="Case title"     <!-- searchable text -->
```

## Disclaimer

For educational use only. Not for clinical decision-making.  
No part of this curriculum replaces proper medical training or clinical judgment.
