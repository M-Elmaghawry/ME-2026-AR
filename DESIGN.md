# Design Customization Guide (Arabic RTL)

This guide explains how to customize the current Arabic/RTL version of the website.

## 1. Color System

The project uses CSS variables in `css/style.css`.

```css
:root {
    --primary: #003060;
    --secondary: #055c9d;
    --accent: #0e86d4;
    --soft: #68bbe3;
}
```

Recommended usage:
- `--primary`: headings, navbar, footer base
- `--secondary`: secondary headings and labels
- `--accent`: CTA buttons and highlights
- `--soft`: soft gradients and numeric highlights

## 2. Typography

Current primary font is Cairo.

- Font import is configured in `index.html`.
- Font variable is configured in `css/style.css` (`--font-primary`).

If changing fonts, choose one with strong Arabic support.

## 3. RTL Behavior Guidelines

The site is globally RTL. Keep these rules while customizing:

- Keep `lang="ar" dir="rtl"` in `index.html`.
- Prefer logical spacing where possible (`margin-inline`, `padding-inline`).
- If you must use directional properties, verify `right`/`left` behavior in all breakpoints.
- Re-test pseudo-elements and list markers after directional edits.

## 4. Layout Tuning

Key areas to tune in `css/style.css`:

- Hero section image sizing and content alignment
- Timeline and card grid min-width values
- Services/features list alignment in RTL
- Slider controls positioning for testimonials and certifications

## 5. Images and Media

Recommended sizes:

- Hero/profile image: square high-resolution (at least 800x800)
- Client logos: transparent PNG preferred, normalized visual height
- Project images: landscape ratio (around 3:2)
- Certificates: high-resolution JPEG/PNG with readable text

Always verify image paths in corresponding JSON files under `data/`.

## 6. Responsive Breakpoints

Main breakpoints are defined in `css/style.css`.

- Desktop: > 992px
- Tablet: 768px to 992px
- Mobile: < 768px

After any layout update, test:
- Navigation and mobile menu
- Hero content wrapping
- Timeline and cards overlap
- Sliders and controls touch behavior

## 7. Motion and Transitions

Global transition speed is controlled by CSS variables and component styles.
Keep animations subtle and readable for Arabic content density.

## 8. Quick QA After Design Changes

- Open `index.html` and inspect desktop/mobile layouts
- Open `test.html` to ensure data still loads
- Verify contrast and readability
- Verify no horizontal scroll appears on mobile

For project-wide setup and deployment details, see `README.md` and `DEPLOYMENT.md`.
