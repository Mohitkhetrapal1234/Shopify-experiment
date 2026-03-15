# CODEX Handoff

## Project

- Brand: `Zariya`
- Store domain: `00met2-k0.myshopify.com`
- GitHub repo: `https://github.com/Mohitkhetrapal1234/Shopify-experiment.git`
- Local repo path: `/Users/mohitkhetrapal/shopify-experiment`

## What was set up

- Initialized local git repo and connected it to GitHub
- Installed Shopify CLI locally through `npm` and authenticated Shopify CLI
- Started a live Shopify theme dev session for the store
- Built a custom homepage section and a custom collection section
- Added a handoff import folder for Shopify product data

## Current theme/dev workflow

- Start dev server: `npm run dev`
- Validate theme: `npm run check`
- Pull from store: `npm run pull`
- Push theme: `npm run push`

## Shopify preview

- Active preview URL when dev server is running:
  `https://00met2-k0.myshopify.com/?preview_theme_id=159208767746`

## Brand and design direction

- Brand name shown in theme: `Zariya`
- Positioning: premium ethnic Indian womenswear
- Intended categories:
  - Lehengas
  - Sarees
  - Anarkalis
  - Sharara sets
  - Festive edit
  - Bridal collection

## Visual decisions made

- Overall direction shifted toward luxury editorial fashion
- Primary canvas is light ivory, not dark
- Burgundy and gold are used as accent colors and within image-led sections
- Serif typography is used for large editorial headlines
- Header is clean and minimal rather than heavy ecommerce chrome
- Homepage structure was rebuilt to follow the rhythm of the screenshots in `reference/`
- Motion was added conservatively:
  - slow promo/ticker movement
  - soft reveal-on-scroll
  - restrained hover lift/zoom on image panels

## Homepage sections currently built

File:
- `theme/sections/hello-world.liquid`

Current homepage structure:
- Pale top announcement band
- Split hero with two editorial image panels and centered copy
- Dark sale strip under the hero
- Large philosophy/editorial statement block
- Product/category rail with dark caption bars
- Pale promo strip
- Large feature banner
- Lower gallery/product-style image row

## Collection page currently built

File:
- `theme/sections/collection.liquid`

Current collection page structure:
- Reference-inspired collection listing layout
- Left filter rail
- Right product grid
- Sale badge styling
- Centered product information under cards

Special behavior:
- If collection handle/title matches `lehenga` and there are no real products yet, the theme shows a fallback demo grid with 10 lehenga cards

## Store/product data work done

Files:
- `shopify-import/lehenga-products.csv`
- `shopify-import/IMPORT_LEHENGAS.md`

Important store limitation discovered:
- CSV import is blocked on the current Shopify trial account
- Real product creation/import must be done manually in Shopify admin unless the account is upgraded

## References used today

Folders/files:
- `reference/landing page.png`
- `reference/Screenshot 2026-03-16 at 12.28.21 AM.png`
- `reference/Screenshot 2026-03-16 at 12.28.24 AM.png`
- `reference/Screenshot 2026-03-16 at 12.28.27 AM.png`
- `reference/Screenshot 2026-03-16 at 12.28.29 AM.png`
- `reference/products/Screenshot 2026-03-16 at 12.42.44 AM.png`

How they were used:
- The landing-page screenshots drove the homepage layout rhythm and spacing
- The product screenshot drove the collection page structure

## What is working now

- Git is configured and pushes to GitHub work
- Shopify CLI auth works
- Theme dev preview works
- Homepage is custom and much closer to the reference feel than the starter skeleton
- Collection page is custom and styled
- Theme checks pass with `npm run check`

## What still needs real content

- Real campaign photography with a consistent lighting/style direction
- Real product data in Shopify admin
- Real collections in Shopify admin:
  - `Lehengas`
  - `Sarees`
  - `Anarkalis`
  - `Sharara Sets`
- Real navigation/menu setup in Shopify admin
- Product descriptions, sizing, fabric info, care info, delivery timeline

## What still feels incomplete

- Homepage can still be improved through better image consistency
- Header/menu spacing could be fine-tuned further if needed
- Product page template is still mostly skeleton and does not yet match the reference quality
- Collection filters are visual only right now; they are not wired into Shopify filtering UX
- Homepage links should be connected to real collections once those collections exist

## Known constraints

- Trial account blocks CSV import
- Some parts of the current storefront still rely on theme fallback content because store data is missing
- The last attempted homepage header overlay change was reverted because it looked worse

## Recommended next session plan

1. Create real collections in Shopify admin
   - `Lehengas`
   - `Sarees`
   - `Anarkalis`
   - `Sharara Sets`

2. Manually create at least 10 real lehenga products in Shopify admin
   - Use the titles/pricing from the fallback/demo content if needed
   - Tag all with `lehenga`

3. Link homepage category cards to real collections

4. Rebuild the product page
   - Use the product screenshot reference more closely
   - Add gallery, pricing block, size selector, add-to-cart area, and product info hierarchy

5. Clean up the homepage once real products and real images exist
   - replace mixed Unsplash images with a consistent campaign set
   - remove any fallback/demo collection content

6. Tune navigation in Shopify admin
   - make sure menu items align with the homepage/category structure

## Most important files touched today

- `theme/sections/hello-world.liquid`
- `theme/sections/collection.liquid`
- `theme/sections/header.liquid`
- `theme/layout/theme.liquid`
- `theme/config/settings_schema.json`
- `theme/assets/critical.css`
- `README.md`
- `SETUP.md`
- `STORE_STRATEGY.md`
- `shopify-import/lehenga-products.csv`
- `shopify-import/IMPORT_LEHENGAS.md`

## End of day status

- Day 1 completed
- Theme work is saved locally
- Ready for commit/push with:
  `End of day 1 — Zariya homepage and collection page`
