# ME-2026-AR - Engineering and BIM Portfolio (Arabic RTL)

Single-page portfolio website for Engineering, BIM, and infrastructure services.
The current version is fully Arabic and RTL, with dynamic content loaded from JSON files.

## Features

- Arabic-first interface (`lang="ar"`, `dir="rtl"`)
- Fully responsive layout (desktop, tablet, mobile)
- Dynamic content rendering from JSON data files
- WhatsApp integration and EmailJS contact form
- Testimonial slider, certifications slider, and training showcase
- Vanilla JavaScript implementation (no framework)

## Project Structure

```text
ME-2026-AR/
|-- index.html
|-- test.html
|-- css/
|   `-- style.css
|-- js/
|   |-- data-loader.js
|   |-- main.js
|   `-- counter.js
|-- data/
|   |-- hero.json
|   |-- experience.json
|   |-- services.json
|   |-- clients.json
|   |-- courses.json
|   |-- projects.json
|   |-- certifications.json
|   |-- qualifications.json
|   |-- testimonials.json
|   |-- tools.json
|   `-- training-courses.json
`-- assets/
```

## Content Updates

Update content directly in `data/*.json`.

- Personal profile and contact: `data/hero.json`
- Career timeline: `data/experience.json`
- Services: `data/services.json`
- Courses: `data/courses.json`
- Projects: `data/projects.json`
- Testimonials: `data/testimonials.json`
- Certifications and qualifications: `data/certifications.json`, `data/qualifications.json`

## Design Customization

- Main styles: `css/style.css`
- Color tokens: `:root` CSS variables
- Primary font: Cairo
- RTL behavior is already enabled globally; keep directional edits RTL-safe

## Contact Form (EmailJS)

The contact form uses EmailJS from the browser.

1. Create EmailJS account and service.
2. Create template with keys: `from_name`, `from_email`, `phone`, `service`, `message`, `reply_to`, `sent_at`.
3. Update form dataset attributes in `index.html`:
   - `data-emailjs-public-key`
   - `data-emailjs-service-id`
   - `data-emailjs-template-id`

## Local Preview

Open `index.html` in browser, or run a local static server for best compatibility.

Use `test.html` to validate that all JSON files load correctly.

## GitHub Pages Deployment

1. Push repository to GitHub.
2. Go to repository Settings > Pages.
3. Source: `Deploy from a branch`.
4. Branch: `main`, Folder: `/ (root)`.
5. Save and wait for deployment.

Live URL pattern:
`https://<username>.github.io/ME-2026-AR/`

## Browser Support

- Chrome (latest)
- Edge (latest)
- Firefox (latest)
- Safari (latest)

## Notes

- This is a static site with no backend.
- Keep media file names stable to avoid broken JSON image paths.
