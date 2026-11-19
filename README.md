# Personal Runway — working demo

Real AI try-on (FASHN): upload a full-body photo, add pieces from any store by link or photo,
the AI dresses you piece by piece, then "Walk it" makes a 5-second runway video.
Size estimates per piece from your measurements; Buy buttons link to each store.

## What you need
- Node.js 18 or newer
- A FASHN API key (app.fashn.ai → Billing → FASHN API tab → buy credits → Developer API → create key)

## Settings (environment variables)
- `FASHN_API_KEY` — your key (required)
- `DEMO_PASSCODE` — a passcode people must type to use the app (strongly recommended: it protects your credits)
- `PORT` — optional, default 3000

## Run (everything is in server.js)
    npm start
Then open http://localhost:3000

## Cost per use (FASHN list prices, Nov 2026)
- Each piece tried on: 1 credit (about $0.075)
- Runway video, 5 s at 720p: 3 credits

## Notes
- Some stores block apps from reading their product pages; the app then asks you to upload the product photo.
- The try-on handles dresses, tops, jackets, pants and skirts. Shoes and bags are not changed.
- Sizes are estimates from a standard US women's chart, adjusted per store ("runs small/large").
