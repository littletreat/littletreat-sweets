# Little Treat - Premium Chocolates & Confections

A beautiful, mobile-friendly website for Little Treat chocolate shop in Ahmedabad.

## Features

- ✅ **Mobile-Friendly**: Fully responsive design that works on all devices
- ✅ **MVC Architecture**: Organized code structure (Model-View-Controller)
- ✅ **Dynamic Menu**: Menu items loaded from `data/menu.json`
- ✅ **Item Selection**: Add/remove items with +/- buttons
- ✅ **WhatsApp Integration**: Send orders directly via WhatsApp
- ✅ **Price Categories**: Plain chocolates split into white/dark/milk variants

## How to View the Website

### Option 1: Using a Local Server (Recommended)

**If you have Python installed:**
1. Double-click `serve.bat` (Windows)
2. Open your browser to: `http://localhost:8000`

**Alternative - Using Python manually:**
```bash
python -m http.server 8000
```

**Using Node.js:**
```bash
npx http-server -p 8000
```

### Option 2: Open Directly in Browser

You can also open `index.html` directly in your browser. The site includes fallback data that will load automatically if the JSON file cannot be fetched.

## File Structure

```
littletreat-sweets-main/
├── index.html              # Main HTML file
├── assets/
│   ├── css/
│   │   └── style.css       # All styles (mobile-responsive)
│   └── js/
│       └── app.js          # MVC JavaScript application
├── data/
│   └── menu.json           # Menu items with prices
├── serve.bat               # Quick server launcher for Windows
└── README.md               # This file
```

## Menu Structure

The menu is organized in `data/menu.json` with the following categories:

1. **Plain Chocolates** (₹10/piece)
   - Plain White Chocolate
   - Plain Dark Chocolate
   - Plain Milk Chocolate

2. **Signature Flavoured Bites** (₹10-12/piece)
   - Chilli Guava Bite
   - Pan Masala Pinata
   - Crispy Coffee Bite
   - Salted Caramel Bite
   - Pineapple Crush Bite
   - Strawberry Crush Bite
   - Mixed Berry White Chocolate

3. **Nutty Indulgence** (₹15-30/piece)
   - Almond Walnut Chocolate
   - Dates Almond Chocolate
   - Mini Coffee Cups
   - Ferrero Rocher Style

4. **Bars & Specials** (₹10-150/bar)
   - Designer Chocolate Bar
   - Salted Caramel Bar
   - Bonty Bar
   - Bubbly Chocolate Bar
   - Crunchy Hazelbar
   - Chew Toffee

## How to Update Menu Items

1. Open `data/menu.json`
2. Add/edit items following the existing structure:

```json
{
  "id": "unique-item-id",
  "name": "Item Name",
  "icon": "🍫",
  "description": "Item description",
  "price": 10,
  "unitLabel": "₹10 per piece"
}
```

3. Save the file and refresh the website

## WhatsApp Integration

When users click "Book Order on WhatsApp", it:
1. Collects all selected items with quantities
2. Calculates the total price
3. Opens WhatsApp with a pre-filled message to: **+91 7874914422**

## Deployment to GitHub Pages

1. Push all files to your GitHub repository
2. Go to repository Settings → Pages
3. Select branch (usually `main`) and root folder
4. Save and wait for deployment
5. Your site will be live at: `https://yourusername.github.io/repository-name/`

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (iOS & macOS)
- ✅ Mobile browsers

## Troubleshooting

**Menu items not loading?**
- If opening the HTML file directly, the fallback data embedded in `index.html` will load automatically
- For full functionality, use a local server (see instructions above)
- Check browser console (F12) for any error messages

**Images/icons not showing?**
- Make sure you have an internet connection (icons are loaded from Font Awesome CDN)
- Check that Google Fonts is accessible

## Credits

Lovingly crafted by **Foram & Parth** 🌟

---

© 2024 Little Treat. All rights reserved.

