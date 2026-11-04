# Sezavar Pishgaman — Canonical Company Website Brand Colors

Status: **LOCKED DESIGN REFERENCE — 2026-11-04**
Scope: **Company website** `sezavarpishgam.com` and its company-branded product / merchant disclosures. **Not** the independent ParvaLia Training app theme.

## Actual site source of truth (exact tokens)

Read directly from `assets/index-CYiGcNes.css` on the existing company website repository:

| Token | Exact source hex | Intended usage |
| --- | --- | --- |
| `--green` | **`#082D24`** | Corporate emerald green |
| `--deep` | **`#041D18`** | Deep emerald / dark background |
| `--gold` | **`#C7A25C`** | Primary metallic-style gold accent |
| `--cream` | **`#F5F0E5`** | Light cream surface and supplementary light text |
| `--ink` | `#14221D` | Dark body type on cream |
| `--muted` | `#68736E` | Muted secondary text |
| `--cyan` | `#00B8D9` | Reserved existing bright accent; **not** a substitute for corporate gold |

The company brand's dark/luxury display variant often uses the gradient and shadow combinations specified in the *actual* corporate site stylesheets. Do not flatten gradients to one screenshot pixel color.

Copy-ready root variables (must remain in sync with the actual site stylesheet, not become a divergent duplicate authority):

```css
:root {
  --green: #082d24;
  --deep: #041d18;
  --gold: #c7a25c;
  --cream: #f5f0e5;
  --ink: #14221d;
  --muted: #68736e;
  --cyan: #00b8d9;
}
```

## Owner-provided creative references (2026-11-04)

The approved reference artwork shows a nearly-black emerald background with warmer/luminous gold type and fine gold wave lines; the second screenshot shows the same aesthetic across five corporate/promotional slides.

**Important distinction:** pixel colors sampled from JPEG references are *appearance measurements*, affected by lighting, glows, anti-aliasing, compression and gradients. They do not override canonical site CSS tokens. For instance, visually dark background patches in the artwork cluster close to `#001810`, while the illuminated gold lettering varies around `#F8C878`; these are **image rendering / highlight examples, not replacement site variables**.

### Brand usage rules

1. **First inspect live website CSS and existing design tokens** before designing or editing a company-domain page. If public hosting and GitHub diverge, reconcile the **actual deployed host CSS** and update this record only with evidence.
2. Use the exact declared corporate green/gold/cream palette and match existing gradients, typography, spacing, border treatment and contrast. Do not substitute similar-looking greens like `#062D25` or gold like `#C8A45F` as the *source* brand tokens.
3. Match the approved company's dark-emerald/gold, modern premium presentation in a mobile Safari rendering; check 320/390px widths and 100%/200% text as relevant.
4. **Never regenerate or approximate the corporate logo.** Use the unchanged official logo file if available, placed without recoloring/cropping/distortion; otherwise omit it.
5. Preserve brand separation: ParvaLia Training **in-app** UI retains its black/purple/blue/turquoise identity and official app logo. The company merchant/product page uses company emerald/gold.
6. Keep commercial truth and safety intact: 21-day package introductory `298,000` toman; future regular `598,000` toman; no falsely asserted previous price; checkout disabled until merchant and fulfilment gates pass.
7. For future website work, use this document for token names, **but actual currently deployed production site CSS takes precedence** if there is verified divergence.

## Current merchant page status / next change

`products/parvalia-training-21day/index.html` was released on the official company domain and human-accepted on iPhone, using an earlier manually selected similar emerald/gold palette. **Do not change this already approved live page merely to adopt these canonical tokens.** Any later color correction must be a separate minimal reviewed change, based on actual current host backup and QA.

This document is a **documentation-only addition**. It does not publish, change live CSS or HTML, modify domain/DNS, or change the ParvaLia Training application.
