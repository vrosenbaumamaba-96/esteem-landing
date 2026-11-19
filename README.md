# Esteem Academy of Beauty — Landing Page Build

Build the paid-ads landing page and thank-you page to match the approved staging build 1:1, then connect the form and tracking. The full developer handoff doc (sections, specs, checklist) is shared separately; this README is the short version.

- Staging: https://esteemlp.provenlayout.com/ (thank-you: /thank-you.html)
- `index.html` — landing page · `thank-you.html` — confirmation page · `images/` — logos
- All styles are inline or in one `<style>` block per page. Icons are inline SVG.

## Pages
- Landing page: **esteem-academy.com/more-info**. Thank-you: **/more-info/thank-you** (suggested).
- No main-site navigation or footer menus on either page.

## Design
| Token | Value | Use |
| --- | --- | --- |
| Deep Teal | #27464C | Top bar, dark bands, headings, secondary buttons |
| Mauve | #BB8391 | Primary buttons (text #1B1B1B), final CTA band |
| Mauve Dark | #8A5263 | Eyebrows, icons on light backgrounds |
| Pink Light | #F2C9D2 | Eyebrows/checks on dark or photo backgrounds |
| Blush | #FFEFF0 | Icon circles, Why Esteem cards, reviews band |
| Light Gray | #F5F3F3 | Alternate bands |
| Footer | #1E3539 | Footer |

Fonts: Poppins 500/600/700 (headings, buttons), Nunito 400–800 (body). Max width 1200px, 32px side padding (16px on phones). One H1 only.

## Form
Fields (all required): Program of Interest (Cosmetology/Barbering, Master Esthetician, Nail Technology, Master Barbering/Hair Design, Eyelash & Eyebrow Technology, Instructor Training, Not Sure Yet), First Name, Last Name, Email, Phone. Hidden: UTM source/medium/campaign/term/content, gclid, fbclid.

Consent text, word for word: `*I agree to be contacted by an Esteem Academy of Beauty representative. Message and data rates apply.` No privacy policy link.

Send to info@esteem-academy.com and Prestige CRM, then redirect to the thank-you page. The staging form only redirects.

## Before launch
- [ ] Connect the form (email + Prestige, with program and UTM fields)
- [ ] Replace the hero photo (womanwithboldeye.jpg) and salon photo (curlinghair.jpg) — both are loaded from esteem-academy.com as placeholders. Host Esteem's own photos locally; hero at least 2000px wide.
- [ ] Build the Instagram feed (6 latest @esteemacademy posts) in place of the placeholder squares
- [ ] Add a sticky mobile bar: "Call" (tel:8016893031) + "Get Info" (scrolls to #form)
- [ ] Install GTM; fire Google Ads + Meta lead conversions on the thank-you page
- [ ] Set indexing for live (staging is noindex) — confirm with the paid team
- [ ] Check desktop, tablet and phone; no horizontal scroll from 360px up
- `images/bbb-accredited-logo.png` and `images/esteem-e-logo.png` are not used on the page.

## Staging deploy (cPanel)
`.cpanel.yml` copies the pages and `images/` to `$HOME/esteemlp.provenlayout.com/`. In cPanel → Git Version Control → Manage → Pull or Deploy: Update from Remote, then Deploy HEAD Commit.
