# NorCal Truck Alignment — Professional Website

Best-in-class, mobile-first, conversion-optimized static website for NorCal Truck Alignment — a mobile semi truck / heavy-duty truck wheel alignment service serving Northern California (Santa Rosa / Sonoma, Bay Area, Sacramento Valley, and beyond).

**Tagline:** Mobile Semi Truck Alignment That Comes to You in NorCal – Save Tires, Fuel & Time.

## Key Features Delivered

- **Fully Branded** — Uses your actual logo files (NEW.png, variants) throughout header, favicon, etc.
- **Mobile-First & Fast** — Tailwind via CDN + vanilla JS. Extremely lightweight, loads instantly even on mobile data. Big tap targets, click-to-call everywhere.
- **Conversion Focused** — Prominent phone numbers (tel: links), multiple booking/quote forms (home quick form + full modal + dedicated contact page). Strong CTAs on every page.
- **Professional Trucking Aesthetic** — Deep navy (#0F172A), bold trucking red (#B91C1C), industrial high-contrast design. Clean typography. Custom AI-generated images matched to brand colors and feel.
- **SEO Optimized for Local Searches**:
  - Targeted titles & meta descriptions with primary keywords: "mobile semi truck alignment NorCal", "truck alignment Santa Rosa", "heavy duty alignment Bay Area", "mobile truck alignment Sacramento".
  - JSON-LD schema (LocalBusiness + Service) on homepage.
  - Proper heading structure, alt text, internal linking.
  - Blog/resources section for long-tail SEO (signs your semi needs alignment, fleet savings, etc.).
- **Trust Signals** — Stats (30% tire life, 2-5% fuel), real-feeling testimonials, equipment highlights, owner-operated emphasis, service area coverage.
- **Multi-Page Structure** (best practice for SEO & UX):
  - index.html (full landing with hero, benefits, how it works, services teaser, testimonials, quick quote, areas teaser)
  - services.html (detailed offerings + benefits + related inspections)
  - about.html (Miguel's story, values, equipment, commitment)
  - areas.html (interactive-feel map + detailed city/region lists)
  - resources.html (SEO content: articles/guides)
  - contact.html (full booking form + map + direct contact)
- **Forms** — Fully functional client-side (success states + simulated submission). Ready for production integration.
- **Accessibility & Performance** — High contrast, semantic HTML, responsive, sticky nav, floating call button on mobile.

## File Structure

```
site/
├── index.html          # Primary landing / home
├── services.html
├── about.html
├── areas.html
├── resources.html
├── contact.html
├── README.md           # This file
└── assets/
    ├── logos/          # Your original logo files (use NEW.png / Norcal...LOGO.png variants)
    └── images/         # Custom generated hero, equipment, tire comparison, fleet, highway shots
```

## Quick Start (Test Locally)

1. Open the `site/` folder.
2. Double-click `index.html` (or any page). It works completely offline (Tailwind loads from CDN on first view).
3. Test on your phone by hosting locally or using a tool like `npx serve site` (or Live Server in VS Code).

## Recommended Hosting & Deployment (Easiest & Best for You)

### Option 1: Netlify (Recommended — Free, Fastest, Best for Static)
- Go to https://netlify.com and sign up (GitHub/Google).
- Drag & drop the entire `site/` folder onto the Netlify dashboard.
- Instant free custom domain + SSL + CDN.
- Forms can be upgraded to real Netlify Forms with 1 line change (see below).
- Perfect for this use case.

### Option 2: Vercel, Cloudflare Pages, or GitHub Pages
- Similar drag-and-drop or connect Git repo.
- All give free SSL + global CDN.

### Option 3: Upgrade Later to Wix / Squarespace / WordPress
- The HTML/CSS is clean and can be used as reference or imported into Webflow/Framer if you ever want a visual builder on top.
- Or copy the copy/images into a Wix/Squarespace template.

**Domain Recommendation**: Point `norcaltruckalignment.com` (or .net) at Netlify. Buy via Namecheap/Google Domains or directly in Netlify.

## Connecting Real Forms (Important for Leads)

Current forms use JS alerts + visual success. To receive actual emails:

### Netlify Forms (easiest)
Add `data-netlify="true"` and a hidden input to forms, e.g. on contact.html:

```html
<form id="contact-form" data-netlify="true" ...>
  <input type="hidden" name="form-name" value="contact" />
  ...
```

Then redeploy. Leads appear in Netlify dashboard + email notifications.

### Alternatives
- Formspree.io (free tier)
- EmailJS (client-side)
- Google Form embed (quick but less branded)
- Zapier/Make.com to forward to email or CRM

## SEO & Google Business Tips

1. **Google Business Profile** (highest priority for local):
   - Claim/verify "NorCal Truck Alignment".
   - Add the new website URL.
   - Add service list + photos (use the ones in assets/images).
   - Post weekly (before/after tire photos, "Just aligned 6 trucks in Petaluma yard today").
   - Encourage reviews.

2. **On-Page SEO** (already done in code):
   - Update real phone/email everywhere.
   - Add real testimonials when you have them (replace the placeholder ones).
   - Create more blog posts on resources.html or add individual pages for keywords like "mobile-truck-alignment-santa-rosa.html".

3. **Technical**:
   - Submit sitemap to Google Search Console (create a simple `sitemap.xml` listing all .html pages).
   - Add Google Analytics 4 (paste script in all `<head>` or use Netlify plugin).

4. **Local Citations**: Get listed on Yelp, YellowPages, Facebook, trucking forums, etc. with consistent NAP (Name, Address= "Mobile — Santa Rosa, CA", Phone).

## Customization Checklist (Do These)

- [ ] Replace placeholder phone/email if changed.
- [ ] Update testimonials with real customer names/quotes + companies (powerful).
- [ ] Add real "years in business", number of trucks aligned, specific certifications if you have them.
- [ ] Replace or supplement AI-generated images with real photos of:
  - Your actual mobile unit / equipment
  - Real before/after tire photos (best conversion asset)
  - Miguel at work or with customers
  - Fleet trucks you've serviced
- [ ] Add pricing if you want to publish it (many mobile services prefer "Call for quote").
- [ ] Update service areas if you have specific zip codes or boundaries.
- [ ] Favicon: Convert NEW.png to proper .ico (use realfavicongenerator.net) and add link.
- [ ] Add Google Maps accurate embed (replace the placeholder iframes with one centered on your primary yard or a broad NorCal view).

## Color Palette (Branded from Your Logo)

- Primary Red (truck/swoosh): `#B91C1C`
- Navy / Dark: `#0F172A`
- Supporting: Clean whites, slate grays, high contrast text

## Images Included

5 custom-generated professional images in `assets/images/`:
- hero-alignment.jpg
- tire-comparison.jpg
- fleet-yard.jpg
- alignment-equipment.jpg
- semi-highway.jpg

These match the rugged/trustworthy/red+navy trucking aesthetic.

## Next-Level Enhancements (Future)

- Add online calendar (Calendly embed) on contact page.
- Google reviews widget.
- Before/after photo gallery page.
- Simple quote calculator (JS) showing estimated annual savings.
- Bilingual (English/Spanish) if needed for NorCal workforce.

## Support / Iteration

This site was built to exceed competitors like Mobalign (mobile focus) and local players (Eighteen Wheel Alignment) in clarity, mobile experience, and immediate lead capture.

Test thoroughly on real phones (iOS + Android). Have a few drivers/fleet managers click through and give feedback.

If you need refinements (new pages, different copy, pricing tables, more articles, different images, or help with actual deployment), provide feedback and we can iterate quickly.

**You now have a complete, professional, lead-generating website ready to launch.**

— Generated for NorCal Truck Alignment (Miguel) — 2026

---

**Deploy tip**: Start with Netlify drag-and-drop today. Get the domain live, update your Google Business Profile and Facebook/Instagram, and start collecting reviews and leads immediately.