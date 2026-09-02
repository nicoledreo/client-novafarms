# client-novafarms — internal preview

Static preview of a Nova Farms site rebuild. **Not the live site.** The live site is the
client's own; this repo exists for internal review only.

- **Preview URL:** https://sgencms.github.io/client-novafarms/
- **Repo visibility:** private. GitHub Pages on a private repo is available on the org's
  Team plan, so the preview is visible only to people with access to this repo.
- **Pages in this snapshot:** 27 of 46 in scope (Home, Locations hub + 6 stores,
  `/visit-us/` hub + 18 landers). The remaining 19 are pharmacy, medical-CT, loyalty,
  shop and standalone pages. Blog is out of scope entirely.

## Why this preview is neutered

A pixel-accurate copy of a live business site is an impersonation and SEO hazard if
published as-is. Before deployment the following were stripped or rewritten — none of
them render, so the verified pixel output is unchanged:

| Change | Count | Reason |
|---|---|---|
| JSON-LD `application/ld+json` removed | 53 | carried the real business name, address, phone, review ratings as machine-readable data |
| `og:image` removed | 81 | social unfurlers ignore robots meta and would render the real brand's card |
| `twitter:*` removed | 162 | same |
| `robots` → `noindex,nofollow` | 27 pages | keep it out of search results |
| `canonical` → preview URL | 27 pages | canonicalising to the live domain would tell Google the client's own site is the duplicate — active SEO harm |
| `og:url` → preview URL | 27 pages | same |

`robots.txt` also disallows all crawling, and `.nojekyll` is present because GitHub Pages
would otherwise strip the `_xorigin/` directory (Jekyll excludes paths beginning with `_`).

## What still calls out to the internet

Three third-party embeds cannot be localised — they are live services, not files:

- Google Maps embeds (location and visit-us pages)
- Terpli widget (all pages)
- Canva embeds (attleboro, dracut, woodbury)

Captured copies of unreferenced cross-origin payloads (Canva fonts, Maps tiles, gstatic)
were pruned: 129 MB → 63 MB. Only the two `_xorigin` scripts the pages actually reference
were kept.

## Verification at time of publish

- Stage 4 pixel gate vs live, 6 viewports: passing pages 95.8–100.000%
- Stage 5 audit: 12/12 acceptance gates, 0 hard issues, 0 soft issues
- Offline check, all 27 pages with every non-`file://` request blocked: root font-size
  16px, 0 broken images, 0 horizontal overflow, 0 uncaught page errors, 0 broken local
  requests

See `README.md` for the bundle's own file/token documentation.
