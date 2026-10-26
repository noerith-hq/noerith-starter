# NOERITH brand assets

Copies of the NOERITH brand kit for this repository. The source of truth, with every size, the
usage rules and the build, is [`brand/` in the organization `.github` repository](https://github.com/noerith-hq/.github/tree/main/brand).
Do not edit these files here: update the kit there and copy the result.

| File | Use |
| --- | --- |
| `noerith-logo-horizontal-on-light.svg`, `noerith-logo-horizontal-on-dark.svg` | The NOERITH footer at the end of `README.md`, and documentation |
| `noerith-mark-on-light.svg`, `noerith-mark-on-dark.svg`, `noerith-mark-mono.svg` | The mark alone, at 48 px and up |
| `noerith-social-preview-1280x640.png` | The repository social preview (Settings → General → Social preview) |
| `web/` | Favicon and app icons for a website or documentation site |

## Website

Copy the files in `web/` to the root of the site, then add:

```html
<link rel="icon" href="/favicon.ico" sizes="32x32">
<link rel="icon" href="/favicon.svg" type="image/svg+xml">
<link rel="apple-touch-icon" href="/apple-touch-icon.png">
<link rel="manifest" href="/manifest.webmanifest">
```

with a `manifest.webmanifest` that lists the app icons:

```json
{
  "icons": [
    { "src": "/icon-192.png", "sizes": "192x192", "type": "image/png", "purpose": "any" },
    { "src": "/icon-512.png", "sizes": "512x512", "type": "image/png", "purpose": "any" },
    { "src": "/icon-maskable-512.png", "sizes": "512x512", "type": "image/png", "purpose": "maskable" }
  ],
  "theme_color": "#0C111D",
  "background_color": "#0C111D"
}
```

## Rules

- These are the organization's marks. A project is named in its README title; it does not get a
  variation of the NOERITH mark. Do not recolour, rearrange or combine the mark with a project logo.
- Minimum sizes: horizontal logo 200 px wide; mark 48 px. For smaller sizes use the small and 16 px
  versions of the mark from the kit.
- A project that should not carry NOERITH branding can delete this folder and the footer at the end
  of `README.md`.
