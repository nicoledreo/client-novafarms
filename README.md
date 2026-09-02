# novafarms.com

Cloned from source on 2026-09-02T06:01:51.537Z.
Static, no build step.

## Pages

| File | Source |
| --- | --- |
| `index.html` | `https://novafarms.com/` |
| `locations.html` | `https://novafarms.com/locations/` |
| `attleboro-ma.html` | `https://novafarms.com/locations/attleboro-ma/` |
| `dracut-ma.html` | `https://novafarms.com/locations/dracut-ma/` |
| `framingham-ma.html` | `https://novafarms.com/locations/framingham-ma/` |
| `newbritain-ct.html` | `https://novafarms.com/locations/newbritain-ct/` |
| `woodbury-nj.html` | `https://novafarms.com/locations/woodbury-nj/` |
| `greenville-me.html` | `https://novafarms.com/locations/greenville-me/` |
| `visit-us.html` | `https://novafarms.com/visit-us/` |
| `best-cannabis-dispensary-near-barrington-ri.html` | `https://novafarms.com/visit-us/best-cannabis-dispensary-near-barrington-ri/` |
| `recreational-cannabis-dispensary-near-plainville-ma.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-plainville-ma/` |
| `recreational-cannabis-dispensary-near-seekonk-ma.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-seekonk-ma/` |
| `best-cannabis-dispensary-near-providence-ri.html` | `https://novafarms.com/visit-us/best-cannabis-dispensary-near-providence-ri/` |
| `recreational-cannabis-dispensary-near-pawtucket-ri.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-pawtucket-ri/` |
| `closest-ma-cannabis-dispensary-to-rhode-island-border.html` | `https://novafarms.com/visit-us/closest-ma-cannabis-dispensary-to-rhode-island-border/` |
| `closest-nj-cannabis-dispensary-to-pennsylvania-border.html` | `https://novafarms.com/visit-us/closest-nj-cannabis-dispensary-to-pennsylvania-border/` |
| `recreational-cannabis-dispensary-near-philadelphia-pa.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-philadelphia-pa/` |
| `recreational-cannabis-dispensary-near-umass-lowell-ma.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-umass-lowell-ma/` |
| `recreational-cannabis-dispensary-near-deptford-nj.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-deptford-nj/` |
| `recreational-medical-cannabis-dispensary-near-west-hartford-ct.html` | `https://novafarms.com/visit-us/recreational-medical-cannabis-dispensary-near-west-hartford-ct/` |
| `recreational-medical-cannabis-dispensary-near-southington-ct.html` | `https://novafarms.com/visit-us/recreational-medical-cannabis-dispensary-near-southington-ct/` |
| `recreational-medical-cannabis-dispensary-near-farmington-ct.html` | `https://novafarms.com/visit-us/recreational-medical-cannabis-dispensary-near-farmington-ct/` |
| `recreational-medical-cannabis-dispensary-near-newington-ct.html` | `https://novafarms.com/visit-us/recreational-medical-cannabis-dispensary-near-newington-ct/` |
| `recreational-cannabis-dispensary-near-lawrence-ma.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-lawrence-ma/` |
| `best-cannabis-dispensary-near-rowan-university.html` | `https://novafarms.com/visit-us/best-cannabis-dispensary-near-rowan-university/` |
| `recreational-cannabis-dispensary-near-wilmington-de.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-wilmington-de/` |
| `recreational-cannabis-dispensary-near-camden-nj.html` | `https://novafarms.com/visit-us/recreational-cannabis-dispensary-near-camden-nj/` |

## Files

```
novafarms.com/
├── README.md
├── audit.json
├── chrome.css                 (shared chrome stylesheet)
├── index.html
├── locations.html
├── attleboro-ma.html
├── dracut-ma.html
├── framingham-ma.html
├── newbritain-ct.html
├── woodbury-nj.html
├── greenville-me.html
├── visit-us.html
├── best-cannabis-dispensary-near-barrington-ri.html
├── recreational-cannabis-dispensary-near-plainville-ma.html
├── recreational-cannabis-dispensary-near-seekonk-ma.html
├── best-cannabis-dispensary-near-providence-ri.html
├── recreational-cannabis-dispensary-near-pawtucket-ri.html
├── closest-ma-cannabis-dispensary-to-rhode-island-border.html
├── closest-nj-cannabis-dispensary-to-pennsylvania-border.html
├── recreational-cannabis-dispensary-near-philadelphia-pa.html
├── recreational-cannabis-dispensary-near-umass-lowell-ma.html
├── recreational-cannabis-dispensary-near-deptford-nj.html
├── recreational-medical-cannabis-dispensary-near-west-hartford-ct.html
├── recreational-medical-cannabis-dispensary-near-southington-ct.html
├── recreational-medical-cannabis-dispensary-near-farmington-ct.html
├── recreational-medical-cannabis-dispensary-near-newington-ct.html
├── recreational-cannabis-dispensary-near-lawrence-ma.html
├── best-cannabis-dispensary-near-rowan-university.html
├── recreational-cannabis-dispensary-near-wilmington-de.html
├── recreational-cannabis-dispensary-near-camden-nj.html
└── <mirrored-source-asset-tree>/
```

## Tech notes for development

- Pure static, no build step, no dependencies.
- Shared chrome CSS in `chrome.css` (linked from each page).
- Page-specific styles in inline `<style>` block in each HTML.
- Internal nav hrefs rewritten to point at sibling pages.
- Asset paths mirror source URL structure verbatim (per scope §K.1).
- Tracking scripts (GA, GTM, FB pixel, Hotjar, etc.) stripped at emit.

## License / ownership

This is a clone of source content. Verify rights before publishing.
