# PetSniper

A static, responsive Adopt Me listing comparison dashboard for GitHub Pages.

## Features
- Search and filter imported pet and account listings
- Sort by AUD price or price per potion
- CSV import, CSV template download, local browser storage
- Marketplace shortcuts (not live integrations)
- No fake live prices, no account credentials, no backend

## Deploy to GitHub Pages
1. Create a public repository called `PetSniper`.
2. Upload `index.html` and `README.md` to its root on the `main` branch.
3. Open **Settings → Pages**, select **Deploy from a branch**, `main`, `/ (root)`, and save.
4. Visit `https://YOUR-USERNAME.github.io/PetSniper/` after deployment.

## CSV format
`title,marketplace,type,priceAUD,url,variant,potions,description`

`type` must be `pets` or `accounts`. `priceAUD` must already be converted to AUD. `potions` is the total count used for unit-price comparison. Use the built-in template for examples.

## Limitations
This first version **does not** scrape marketplaces or retrieve live prices. GitHub Pages cannot run a server-side scraper. Imported listings are saved per browser and are not shared with friends. A future version needs permitted APIs or a separately hosted ingestion service and shared database to offer live public comparisons. Marketplace availability and trading policies must be checked independently.

Not affiliated with Roblox or Adopt Me. Third-party trading and account sales can violate platform rules and carry financial/account risks.