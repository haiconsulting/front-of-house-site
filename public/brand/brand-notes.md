# Front of House: The Open Door

October 2026 · Marketing-site concept for local review

## Idea

Hospitality begins with an invitation. A geometric arch and open doorway make
that invitation recognizable at any size, from a browser icon to a storefront.
The stacked lowercase **front of / house.** wordmark feels direct and welcoming.
Together they give Front of House a distinctive signature that can work across
the marketing site and, after approval, its related applications.

The redesign puts restaurant character and real work first. Its commercial
promise stays intact: a custom website the restaurant owns, supported by a
clearly priced annual care plan.

## Palette

| Color | Hex | Purpose |
|---|---|---|
| Front of House red | `#a52e24` | Identity and primary actions |
| Ink | `#29251f` | Type and dark surfaces |
| Paper | `#f7f5ee` | Main background |
| Bone | `#eeece3` | Supporting background |

Supporting colors and interaction states are defined in `src/styles/global.css`.

## Type

**Archivo Variable** carries the wordmark and primary headlines.
**Inter Variable** carries body text and interface controls.
**Cormorant italic** is a restrained editorial accent.
The combination gives the studio a confident voice while retaining hospitality's
warmth. The canonical implemented logo is `src/components/Logo.astro`.

## Image provenance

The local redesign includes a fictional restaurant scene generated with the
built-in **ImageGen** tool. It is concept imagery, not a photograph of an FOH
client, a completed FOH photo shoot, or an identifiable real restaurant.
Actual portfolio projects retain their own project imagery and attribution.

Exact ImageGen prompt:

> Premium editorial photograph of a fictional independent neighborhood restaurant at golden hour. Walnut tables and chairs, oxblood leather banquette, wine glasses, warm table lamps, softly blurred guests, and doorway framing toward the back. Portrait 4:5 composition, foreground table in natural focus, subtle analog grain, balanced warm lighting, cream and burgundy palette. No text, logos, watermarks, named client, or identifiable location.

## Asset files

- Primary logo: `public/brand/foh-logo-red.svg`
- Ink and reversed logos: `foh-logo-ink.svg`, `foh-logo-reversed.svg` in the same folder.
- Standalone marks: `foh-mark-red.svg`, `foh-mark-reversed.svg`.
- All logo and mark exports also have high-resolution transparent PNG versions.
- Lettering is outlined in the SVG exports, so no font installation is required.
- Favicon: `public/favicon.svg` and `public/favicon.ico`.
- Social image: `public/og/front-of-house-redesign.png` (1200 × 630), with SVG source.
- Generated hero master: `public/images/brand/hospitality-editorial.png`. Responsive WebP derivatives are used on the site.

## Intended rollout

1. Review the complete marketing-site concept locally at `http://localhost:4999`.
2. Refine the identity and site from the user's feedback, then obtain approval.
3. Publish the approved marketing site to `fohrestaurants.com`.
4. Apply the approved identity to relevant FOH applications, social assets,
   documents, and client-facing materials in a separately reviewed rollout.

This concept is pending approval. Creating these assets does not approve
production deployment or changes to other applications.
