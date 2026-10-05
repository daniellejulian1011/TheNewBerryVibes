# Berry Vibes Studio × CCD — V5

A multi-page HTML/CSS/JavaScript GitHub website for the Berry Vibes Cozy Core Diet workflow, with an optional Node backend for cross-device authentication, uploads, shared social features and server-synced data.

## V5 update

### Food
- Recovered CCD food/recipe vault + reactive Breakfast/Lunch/Snack/SOTD/Dinner filtering.
- **Add My Own Food** studio for brand-new recipes and brand-new snacks.
- Custom foods support name, meal type, serving/yield, ingredients, taste/notes, calories/macros, photo, edit/delete, and load-to-log.
- **Recipe Modification Calculator** keeps the text prompt: `THE ONLY THING I CHANGED FROM THE RECIPE I CREATED WAS....`
- Modifications can add/remove ingredient quantities from the CCD pantry or custom Grocery ingredients.
- Calories and macros recalculate against the original recipe and show the exact calorie difference.

### Account
- The former Profile UI is consolidated into `account.html`.
- Account contains profile photo, display name, height in feet/inches such as `5'2`, weight, reason for using the site, full themes, sign-in status and sign out.
- `profile.html` is now only a compatibility redirect to Account.

### Navigation
- Less-crowded authenticated top bar.
- Core pages stay visible.
- A hamburger **MENU** opens the complete site navigation in a slide-over panel.
- The cinematic homepage keeps its transparent navigation over the animated header.

### Hydration
- Replaced the old tall bottle graphic with a compact horizontal Hydration Flow card.
- Visual 5-step droplet meter, current bottle count, quick add/undo controls and status message.

### Calendar
- Existing plans, log edit/delete, water adjustment and monthly calendar remain.
- New **Photo of Food I Made** uploader saves an image and food/recipe name directly to the selected date.
- Saved calendar food photos appear as image thumbnails in that day’s history.

## Existing major pages
Today, Food, Recipes, SOTD, Movement, Fasting, Restaurants, Grocery, Food Battle, Facts, Calendar, Period Tracker, Social, Account, Settings and About, plus authentication/recovery screens.

## GitHub Pages vs backend
The static GitHub Pages version uses browser-local account/data fallbacks. The included Node backend enables true server authentication, upload storage and cross-account shared social behavior when deployed and connected in `config.js`.

## Run locally with backend
```bash
npm install
node server.js
```

## GitHub Pages deployment
Upload the root contents to a GitHub repository and enable **Settings → Pages → Deploy from a branch → main / root**.

## V5.1 recipe-remix layout fix
- Recipe modification/calorie comparison was moved out of the narrow sticky food-log sidebar into its own full-width responsive card.
- Original vs modified calories, ingredient action, quantity, ingredient picker, Apply, Save Modified Version, and Clear controls now have dedicated width and stack cleanly on smaller screens.
- The food logging sidebar remains focused on servings, drink, time, photos, and logging.
