# BIYAYA — Static Bakery Catalog

A responsive static HTML/CSS/JavaScript shop showcase ready for Vercel. No backend, accounts, database, or build process required.

## Configure the Facebook links

Open `script.js` and replace the empty values at the top:

```js
const FACEBOOK_PAGE_URL = 'https://www.facebook.com/YOUR_ACTUAL_PAGE';
const MESSENGER_URL = 'https://m.me/YOUR_ACTUAL_PAGE';
```

Do not use example URLs as live links. If you don't have a direct Messenger link, leave `MESSENGER_URL` empty and the order button will open the Facebook page instead.

## Customize products

In `script.js`, edit the `products` array. Product prices and all products other than the pictured chocolate loaf are examples. Replace sample emojis with real product images by adding files under `assets/` and using `image:'assets/your-file.jpg'` instead of `emoji`.

## Run locally

Open `index.html` in your browser. Or from the folder run `python -m http.server 8000` and visit `http://localhost:8000`.

## Deploy to Vercel via GitHub

1. Extract the ZIP.
2. Create a new GitHub repository, and upload the contents of the `biyaya-shop` folder to the repository root (not the enclosing folder).
3. Open Vercel > Add New > Project > Import Git Repository.
4. Select **Framework Preset: Other**. Keep the root directory as `./`, leave the build command blank, and deploy.
5. When you update your GitHub repository, Vercel automatically deploys the changes.

No environment variables are required.

## Files

- `index.html` — website structure
- `styles.css` — responsive styling
- `script.js` — product catalog, filters, dialog, and social links
- `assets/logo.jpg` — user-provided business logo
- `assets/chocolate-loaf.jpg` — user-provided product photograph
