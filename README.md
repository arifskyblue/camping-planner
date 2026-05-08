# ðŸ•ï¸ CampPlanner

A free, zero-cost camping organizer for you and your family. Works on any phone or browser â€” no app install needed.

## Features

- **Smart Meal Table** â€” Set check-in/check-out times and meals auto-grey out when you're not at camp (e.g. arrive at 4pm = no breakfast that day)
- **Ingredient Tracker** â€” Add ingredients to each meal, they flow automatically into your grocery list
- **Packing Checklist** â€” Pre-loaded categories with progress tracking. Add/remove items freely
- **Grocery List** â€” Auto-generated from your meal plan, organized by category (produce, meat, dairy, etc.)
- **Export** â€” Download Excel (.xlsx), copy to clipboard for WhatsApp, or print

## How to Use

1. Open the app at your GitHub Pages URL
2. Go to **Trip Setup** â€” enter check-in/check-out date and time
3. Go to **Meals** â€” plan what you're eating each day. Click "+ ingredients" to add what you need
4. Go to **Grocery** â€” your shopping list is ready, organized by category
5. Go to **Packing** â€” check items off as you pack

## Share with Family

Just send the URL. No login needed. 

> **Note:** Data saves in your browser locally. For real-time sync between you and your wife on different devices, connect a free Supabase backend (see instructions below).

## Deploy to GitHub Pages

1. Fork or clone this repo
2. Go to repo **Settings â†’ Pages**
3. Set source to **main branch / root**
4. Your app is live at `https://yourusername.github.io/camping-planner`

## Real-time Sync (Optional - Free)

To share live data between you and your wife's phones:
1. Create a free account at [supabase.com](https://supabase.com)
2. Create a table called `campdata` with a single `jsonb` column called `data`
3. Add your Supabase URL and anon key to the top of `index.html`
4. Uncomment the sync code block

## Tech Stack

- Pure HTML + CSS + JavaScript (no framework needed)
- [SheetJS](https://sheetjs.com) for Excel export (loaded from CDN)
- [Google Fonts](https://fonts.google.com) for typography
- localStorage for data persistence
