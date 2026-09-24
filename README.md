# OMD International

A single-page site for OMD International, the operating group of Blue Ocean
Business Trust. Static HTML with no build step: open `index.html`, or serve the
repository root.

## Structure

| Path | What it is |
| --- | --- |
| `index.html` | The home page. Styles and script are inline, so there is one file to edit. |
| `privacy.html` | Privacy policy. Self-contained: it repeats the design tokens rather than sharing a stylesheet, so a palette change has to be made in both files. |
| `assets/omd-logo.png` | Wordmark, cropped and keyed to transparency from the source logo. |
| `assets/omd-team.webp` | Team portrait supplied by the client. |
| `assets/omd-boardroom.jpg` | Boardroom band used in the group section. |
| `assets/fonts/` | Self-hosted Marcellus and Archivo (latin subset). |
| `assets/OMD logo.png`, `assets/OMD team.png`, `assets/team photo.webp` | Original source files, kept for reference. |

## Design notes

**Colour** is sampled directly from the supplied logo rather than picked by eye.
The ground `#1F1F1F` is the exact grey behind the wordmark, and `#DDB157` with a
`#F8D175` highlight are the golds in the lettering. Sampling keeps the page and
the logo in the same family instead of approximately near each other.

**The organising idea is British hallmarking** — the punch marks struck into
precious metal to certify what it is and who stands behind it. It ties together
gold, luxury, a UK business and the word Trust. Section headings and the five
service tiers each carry a punch mark rather than a typographic label.

**The five services are shown as a ladder, not a grid**, because they are a real
sequence: each one involves the group more deeply in a client's business, from
running campaigns to holding equity. The bar on the right of each row encodes
that depth, and it is the one piece of motion on the page besides the hero.

**Type** is Marcellus for display, chosen for its inscriptional Roman capitals,
which suit stamped and engraved marks. Archivo carries body and interface text.

**Fonts are self-hosted**, so no visitor IP is passed to Google on page load.
That matters for a UK and EU audience.

## Accessibility

Text colours are checked against the `#1F1F1F` ground: body and secondary text
clear 4.5:1, and the small gold labels use `#C09A4E` at 6.26:1. The hero
animation freezes to a single frame under `prefers-reduced-motion`, and the
depth bars render at full length rather than animating. The small-screen menu is
a standard disclosure button with `aria-expanded` and closes on Escape.

## Before the privacy policy is relied on

The policy at `privacy.html` is a working draft, not legal advice. It has not been
reviewed by a solicitor. Fill in every value marked in gold on the page, and note:

- Registered office address, company number, and the Australian entity name and ACN.
- Retention periods. The figures given are common defaults, not your actual practice.
- **A cookie consent banner does not exist yet.** The policy states that analytics and
  advertising cookies are set only with consent, which is what UK GDPR and PECR require.
  Until a consent tool gates Google Analytics, Google Ads and the Meta Pixel behind an
  opt-in, the page describes something the site does not do.

## Placeholder content to confirm

- `contactus@omd-international.com` is the contact address.
- Office cities under "The people" are assumed from the group's stated reach.
- Copy describes capability in general terms and makes no numeric claims, so it
  needs a read-through before launch rather than fact-checking.
