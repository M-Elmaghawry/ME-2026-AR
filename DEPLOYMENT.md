# Deployment Checklist

Use this checklist before publishing the Arabic RTL website.

## 1. Content Verification

- [ ] Review `data/hero.json` (name, subtitle, contact info, WhatsApp settings, social links)
- [ ] Review `data/experience.json`
- [ ] Review `data/services.json`
- [ ] Review `data/courses.json`
- [ ] Review `data/projects.json`
- [ ] Review `data/testimonials.json`
- [ ] Review `data/certifications.json`
- [ ] Review `data/qualifications.json`
- [ ] Review `data/clients.json` and `data/tools.json`
- [ ] Review `data/training-courses.json`

## 2. Assets Validation

- [ ] Confirm all image paths referenced in JSON exist under `assets/`
- [ ] Verify client logos in `assets/clients/`
- [ ] Verify project images in `assets/projects/`
- [ ] Verify certificates in `assets/certificates/`
- [ ] Verify hero and training images load correctly

## 3. RTL and UI Validation

- [ ] Confirm `index.html` has `lang="ar" dir="rtl"`
- [ ] Confirm typography is Cairo and readable across sections
- [ ] Check navbar, hero, timeline, services, projects, testimonials, and footer alignment in RTL
- [ ] Check mobile menu behavior in RTL

## 4. Functional Testing

- [ ] Open `test.html` and verify all JSON files pass
- [ ] Test navigation anchors
- [ ] Test WhatsApp links
- [ ] Test project filtering and sliders
- [ ] Test contact form validation
- [ ] Test EmailJS send flow from contact form

## 5. SEO and Metadata

- [ ] Update page title in `index.html`
- [ ] Update meta description and keywords in `index.html`
- [ ] Add/verify favicon in root
- [ ] (Optional) Add Open Graph and Twitter Card tags

## 6. GitHub Pages Deployment

- [ ] Push latest `main` branch to GitHub
- [ ] Repository Settings > Pages
- [ ] Source: Deploy from a branch
- [ ] Branch: `main`, Folder: `/ (root)`
- [ ] Save and wait for build completion
- [ ] Verify live URL works on desktop and mobile

## 7. Final QA

- [ ] Cross-browser check: Chrome, Edge, Firefox, Safari
- [ ] Mobile check: Android and iOS browsers
- [ ] Performance check (image sizes and page load)
- [ ] Accessibility check (contrast, keyboard navigation, headings)

---

Note: This is a static site. Backend behavior depends on third-party integrations such as EmailJS.
