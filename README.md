# 🎁 Giftly — Gift Shopping Website

A simple, modern, beginner-friendly gift shop built with **only HTML, CSS, and vanilla JavaScript**. No frameworks, no build step.

## ✨ Features

- Multi-page layout (Home, Products, Product Details, Cart, Checkout, About, Contact)
- Responsive design (Flexbox + CSS Grid)
- Dynamic product rendering from JS arrays
- Search, category filter, and sort
- LocalStorage-backed shopping cart with quantity controls
- Toast notifications, mobile menu, smooth scroll, light animations
- Form validation on checkout & contact pages
- Image URLs centralized in `js/imageData.js`

## 📁 Project Structure

```
gift-shop/
├── index.html
├── products.html
├── product-details.html
├── cart.html
├── checkout.html
├── about.html
├── contact.html
├── css/
│   ├── style.css
│   ├── responsive.css
│   └── animations.css
├── js/
│   ├── main.js
│   ├── products.js
│   ├── cart.js
│   ├── checkout.js
│   └── imageData.js
├── assets/
│   ├── icons/
│   └── banners/
└── README.md
```

## 🚀 How to Run

Just open `index.html` in your browser.

For best results (so relative paths and `fetch` work correctly), serve the folder with a tiny local server:

```bash
# Python
python3 -m http.server 8000

# or Node
npx serve .
```

Then visit `http://localhost:8000`.

## 🖼️ Replacing Images

All image URLs live in `js/imageData.js`. Swap any URL there to update images site-wide.

## 🛒 How the Cart Works

- Items are stored in `localStorage` under the key `giftly_cart`.
- Add items via the "Add to Cart" buttons on product cards or the details page.
- The cart page lets users update quantities or remove items.
- Checkout simulates an order and clears the cart.

## 📝 Notes

- The `assets/icons` and `assets/banners` folders are placeholders — drop your own files here if you want to host images locally instead of using Unsplash URLs.
- This is a **static** project — no backend, no database. All data is in JavaScript arrays.

Enjoy! 🎁
