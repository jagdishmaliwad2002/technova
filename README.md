# TechNova – Smart Thermos Store

A single-page, responsive storefront for **TechNova**, a smart thermos and tumbler brand. Built with plain HTML, CSS and JavaScript. No frameworks, no build step, no dependencies.

Developed by **Mahisagarsoft**.

## Quick start

1. Put `index.html` anywhere on your computer or web host.
2. Double-click it to open in a browser.

That's all. The product photos are embedded inside the file, so no other files are needed. An internet connection is only used to load the Inter and Sora fonts from Google Fonts. Without it, the page falls back to system fonts.

## What's on the page

| Section | Details |
|---|---|
| Top bar and header | Welcome note, contact, language and currency, search, account, cart with live count. The header sticks to the top, blurs and shrinks on scroll. |
| Menu and ticker | Dark navigation bar, plus a slow scrolling strip of store promises. |
| Hero slider | 3 auto-playing slides with progress dots, arrows and a subtle mouse parallax. Hovering pauses it. |
| Features strip | Free shipping, returns, secure payment, support, original products. |
| Shop By Category | Six category cards. |
| Promo bar | First-order discount code (TN10). |
| Deals Of The Day | Two deals with stock bars and live countdown timers. |
| Banner grid | Ice cold, leak proof, smart LED, BPA free, and a Black Friday panel. |
| Brand band | "Made to keep your day at the right temperature", with count-up numbers. |
| Featured Products | 5 products with badges, ratings, prices and Add to Cart. |
| Tumbler Collection | 5 tumblers with colour dots. Click a photo to view it full screen. |
| Newsletter and service strip | Email sign-up bar and delivery, checkout, quality and returns notes. |
| Footer | Brand block, link columns, contact details, payment badges, copyright, developer credit. |

### Interactions

- Scroll-reveal animation on every section
- 3D tilt, shine sweep and lift on product cards
- Heart button to save products (shows a message)
- Add to Cart bumps the cart counter and shows a message
- Full-screen photo viewer (click any product photo, close with a click or Esc)
- Slow fill-in hover effect on buttons, with a slight magnetic pull on desktop
- Scroll progress bar and back-to-top button
- Reduced-motion setting is respected (animations are switched off)

## Responsive behaviour

| Screen | Layout |
|---|---|
| Large desktop (1500px and up) | Wider content area |
| Laptop | 5 product columns, full navigation |
| Tablet (up to 1100px) | 3 product columns |
| Phone (up to 900px) | Search moves under the logo, menu scrolls sideways, hero and banners stack, 2 product columns |
| Small phone (up to 520px) | Tighter spacing, 2 category columns, single-column deals |

## Customising

Everything is inside `index.html`. Search for these names to find each part.

**Brand colours**: edit the CSS variables at the top of the `<style>` block: `--blue`, `--navy`, `--org`, `--gold`.

**Hero slides**: edit the `S` array in the script (title, text, three photo keys, background colours).

**Products**: edit the `pr` array (Featured Products) and the `tm` array (Tumbler Collection). Each entry is: badge, name, price, old price, photo key, colours.

**Deals, banners, categories, footer text**: edit the HTML directly. Look for the section comments or class names such as `deals`, `ban`, `cats`, `foot`.

**Contact details**: the email, phone number and address in the top bar and footer are placeholders. Replace them with your real details.

### Replacing photos

Photos live in the `IMG` object, as base64 WebP strings (keys such as `p03`, `p15`, `t1`).

To use separate image files instead, which makes the page load faster:

1. Save your images in an `images` folder next to `index.html`.
2. Change a value, for example `p03:"data:image/webp;base64,..."` to `p03:"images/mint-bottle.webp"`.
3. Keep the `images` folder together with `index.html` when you upload.

Tall photos with a 2:3 or 3:4 shape look best, because the cards show the whole image without cropping.

## Performance notes

- File size is about 750 KB, mostly the embedded photos (recompressed to WebP).
- The hero shows a loading shimmer until the script runs.
- For a live store, separate image files on your hosting will load faster than embedded ones.

## Known limits (this is a front-end design)

- The cart, wishlist, search, newsletter form and login are visual only. Nothing is saved or sent anywhere.
- Menu items, category cards and footer links point to `#`. Connect them to real pages.
- Prices, product names, ratings and stock numbers are sample content.
- Some sample photos show other companies' logos (such as Stanley, Milton, UZSPACE). Replace them with your own product photos, or photos you have rights to, before going live.

## Browser support

Current versions of Chrome, Edge, Firefox and Safari, on desktop and mobile.

## Credits

- Design and development: **Mahisagarsoft**
- Fonts: [Inter](https://fonts.google.com/specimen/Inter) and [Sora](https://fonts.google.com/specimen/Sora) via Google Fonts
