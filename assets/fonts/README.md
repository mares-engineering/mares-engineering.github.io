# Eurostyle/Eurostile Webfont

This directory contains the self-hosted `woff2` font required for the root site logo
headline to render with the `Mares Display` face even when visitors do not have the
font installed.

If you need to replace it, keep the filename as:

- `assets/fonts/eurostile-extended-black.woff2`

Do not add commercial font files without license permission.

The home page CSS expects this file via:

```css
@font-face {
  font-family: 'Mares Display';
  src: url('assets/fonts/eurostile-extended-black.woff2') format('woff2');
}
```
