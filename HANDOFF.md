# HONEY, I Do LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/honeyIDoLlc/ · **Repo:** https://github.com/10elizabethbell/honeyIDoLlc · **Built:** 2026-10-21 from Muse brief (run 2026-10-21, Facebook group scouting)

## What's built
- One page, phone first, in the calm band style: paper header (wordmark left, tap-to-call (609) 431-0036 top right) → navy hero → paper "We treat your home like it's ours" → navy services rows → deep-navy "How it works" → paper job form → navy close with the big number → deep-navy footer.
- Palette: no logo, so honey gold (#f2b134) is taken from the name, on workshop navy (#1d3a5c) and deep navy (#14243a); paper #f4f6fb; honey as text on light uses #875700.
- Hero: H1 "Your honey-do list, done." with the letter bounce-in, their own line as the eyebrow ("No job too big. No job too small.", spelling fixed from "to"), their own promise ("Shower looking tired? New caulk can make all the difference."), two buttons: Tell us about the job (to the form) and Text us.
- Hero background is a **generated example photo** of a clean white tub-and-tile bathroom under a navy overlay; the care section shows a **generated** close-up of a sealed tub corner. Neither is their work (see Images). Swap in the owner's own before/afters as soon as they send some.
- Services rows: Shower refresh, New caulk, Small repairs, Bigger jobs. Each row jumps to the form and pre-picks that job.
- Form: job chips (optional), name, what needs doing, town (optional) → composes a text to 609-431-0036. After submit it shows a fallback for desktops and in-app browsers where `sms:` does nothing: "Open in Messages", "Copy message", and the tap-to-call number.
- Floating honey text circle: hidden on the hero, shown below it, hidden while the form is on screen.
- Favicon / home-screen icon: an "H" on a honey hexagon (no logo exists). og.png 1200×630 for the Facebook preview.

## Assumptions I made
- **Voice "we/us"**: the ads say "call us today".
- **Colours** from the name (honey), not a brand: there is no logo or known colour.
- **Services list** beyond "shower refresh" and "caulk" is inferred: "Small repairs" and "Bigger jobs" come from "No job to big. No job to small" and the handyman category. No other trades named.
- **Care copy** is mine, in their voice: H2 "You ask. We say "I do."", lede "We leave your bathroom the way we'd want ours: clean lines, nothing left behind." Owner should confirm or rewrite.
- **How it works** (Call or text us / We talk it through / We cross it off your list) is mine; no prices, timing or quote policy claimed. The finish reviewer suggested cutting the band as generic process copy; I kept it short because the page has no other proof. Yours to cut.
- **Texting**: the brief says texts are unknown. The page offers text (hero button, form, floating circle) but the number is always tap-to-call in the header, in the close and after the form.
- **No place in the H1**: the calm style wants the town in the H1, but the brief says "do not publish a location". Close says "Not sure we come out to you? Call and ask."

## Placeholders and gaps
- No photos of their work → no proof/gallery section at all. The Facebook link sits in the "care" section instead of under photos.
- No logo, owner name, hours, service area, email (footer has no email line), reviews, prices, licence or insurance. None are mentioned on the page.

## Questions for the owner
1. Do you take texts at 609-431-0036? (If not: swap the Text buttons and floating circle to call.)
2. Which towns do you cover? (Goes in the H1 and the close.)
3. Before/after photos of shower refreshes and other jobs? (Replaces the generated photos and adds a work section.)
4. Your first name? ("I'm ___" reads more personal than "we".)
5. What else is on your list: tile, grout, drywall patching, fixtures, doors? Anything you won't do?
6. Licensed / insured in NJ? A logo? An email for the footer? Hours?

## Ideas not built (yours to pick)
- **Runner-up world (opt-in signature motion):** a honeycomb of fresh caulk: the hero's bottom edge drawn as a caulk bead you can "smooth" with your finger, a drip of honey from the "done." Other worlds considered: tile grid that straightens as you drag; a honey-do sticky-note list where items get crossed off; water beading off a fresh caulk line.
- A "Crossed off the list" before/after slider section once real pairs exist.
- Header shadow once you scroll past the hero (calm kit component 1); not built.
- Field fills (#e6ecf5 on white) are 1.19:1 against the card, failing WCAG 1.4.11 non-text contrast, as on every calm build. A 1px `rgba(20,36,58,.3)` inset border would fix it; your call since it changes the soft look.
- Impeccable flags kept on purpose (Ellie's calm-style choices): eyebrow pills, the H1 letter bounce-in, the floating text circle, Cal Sans, the faint diagonal band texture ("repeating-gradient stripes").

## Images
**Both photos are generated examples, not HONEY, I Do's work.** The close-up sits above "See us on Facebook" with no caption, so a visitor could read it as their job. Replace with the owner's photos before handing the site over, or keep it only if the owner is fine with an example.

| File | Shows | Source | Prompt (short) | Licence |
|---|---|---|---|---|
| img/hero-1600.webp (desktop), img/hero-900.webp (phone crop) | Clean white tub/shower with subway tile, window with a plant | Generated 2026-10-21 locally with Z-Image Turbo (`genimg --local`, seed 21) from `src-assets/gen/hero2.png` | "small, bright suburban bathroom, white tub and shower combo, white subway tile, fresh clean white caulk line, wide lens from the doorway" | Generated locally with Z-Image Turbo; no third-party photo rights |
| img/bead.webp | Corner of a white tub sealed to white tile, chrome spout | Generated 2026-10-21 locally with Z-Image Turbo (seed 11) from `src-assets/gen/bead2.png` | "corner of a white bathtub meeting white square tiles, seam sealed with a thin smooth line of fresh white silicone" | Same |
| og.png, apple-touch-icon.png, favicon.svg | Headline card; "H" on a honey hexagon | Rendered from the site's own type (no logo exists) | n/a | Ours |

Rejected: `src-assets/gen/hero.png` (plainer bathroom, rod floating off the wall), `src-assets/gen/bead.png` (a loose white tube lying on the tub; didn't read as caulk). OpenAI gpt-image-1 was the first choice but the account is out of credits (429 "credit_balance_exhausted").

## Impeccable sweep
- Ran: critique (finish reviewer, two rounds), audit (overflow at 360/390/430/1440, tap targets, input font size, contrast by math and pixel sampling, headings order, labels/autocomplete), harden (form errors, punctuation of composed text, sms fallback), clarify (care copy, removed a repeated eyebrow), adapt (phone hero gets its own crop via `<picture>`), optimize (page ≈ 30 KB + 58 KB of WebP, hero fetchpriority, bead lazy), typeset/layout/colorize via the detector (stripes and flat-type flags suppressed for index.html with reasons in `.impeccable/config.json`).
- Not run: live (needs you in the browser), onboard (no first-run flow), bolder/overdrive/delight (would fight the calm style; the runner-up world above is the "bolder" option).
- Applied from the reviewer: `<picture>` phone crop; desktop overlay restored to ≥.62 on the right; higher-quality hero WebP; form fallback (Open in Messages / Copy / call); care copy rewritten and its paper-band accent removed; "!."/"?." punctuation bug; duplicate form eyebrow removed; this image table.

## Not verified
- Real-device touch, real SMS handoff on iOS/Android (and inside Facebook's in-app browser).
- Frame rate of the bounce-in on old phones.
- WebKit/Safari: Playwright's WebKit isn't installed on this Mac, so checks ran in Chrome only.
- Hero photo on a real 3x iPhone (phone crop is 900px wide native, so slightly soft at 3x under the overlay).
