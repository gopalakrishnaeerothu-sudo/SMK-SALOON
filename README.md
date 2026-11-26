# The SMK Saloon — website

Single-page site for **The SMK Saloon**, a men's hair salon in Duddukuru, Andhra Pradesh (534313), founded by Sai Murali Krishna in 2020.

Everything lives in [`index.html`](index.html): inline CSS and JavaScript with no build step. Lenis (smooth scroll) and, only in video mode, mp4box.js load from jsDelivr at runtime.

The hero follows the RK portfolio layout: a giant wordmark, the founder's portrait in an arched frame that tilts towards the cursor, and a slowly turning 3D ring of brand cards behind it.

## Run locally

```sh
npx serve .
```

Then open the printed URL.

## Deploy

The repo is a static site. On Vercel, import the repo with no framework preset, no build command and the root as the output directory. Every push to `main` redeploys.

## Images and media (drop-in)

The page reads these exact paths. Any file that is missing is replaced by a designed fallback, so nothing appears broken.

| Path | What to put there |
|---|---|
| `assets/founder/smk-portrait.jpg` | Founder, side profile (black tee). Used as the hero portrait |
| `assets/founder/smk-sunset.jpg` | Founder, white shirt at sunset |
| `assets/founder/smk-ride.jpg` | Founder, blue shirt on scooter |
| `assets/promo/textured-crop.jpg` | Promo: textured crop on grey backdrop |
| `assets/promo/french-crop.jpg` | Promo: French crop with high fade |
| `assets/promo/salon-wood.jpg` | Promo: wooden salon interior (phone story image) |
| `assets/promo/salon-dark-teal.jpg` | Promo: dark salon with teal light (social share image) |
| `assets/styles/{fade,classic,textured,modern,korean,groomed}.jpg` | Optional: one portrait photo per hairstyle card |
| `assets/video/scene.mp4` | Optional: 10 s, 24 fps, 1280×720 H.264 clip that scrubs with scroll behind the hero and story. Used only if `CFG.scene` is set to `"video"` in `index.html` |

## Business facts used

- Hours: Mon, Wed, Thu, Sat, Sun · 6:00 AM–1:00 PM and 2:30 PM–8:30 PM. Closed Tuesday and Friday. The live open/closed badge uses India Standard Time.
- Phone and WhatsApp: +91 77992 99920
- Instagram: [@its_me.smk](https://www.instagram.com/its_me.smk)
- No prices, street address, awards or certifications are published. Services show "Contact for pricing".
