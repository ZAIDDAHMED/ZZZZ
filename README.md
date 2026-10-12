# Naseeb Marbles Website

A single-page website for Naseeb Marbles. The main page loads its sections and product data from separate files in this folder.

## Website Chalu Kaise Karein

Chrome mein `indexx.html` ko seedha double-click na karein. Browser local files se `fetch()` requests block karta hai, isliye sections aur products load nahi honge. Python 3 installed hona chahiye.

1. Is folder mein PowerShell ya terminal kholein.
2. Local server start karein:

   ```powershell
   py -m http.server 8000
   ```

3. Chrome mein yeh address kholein: <http://localhost:8000/indexx.html>
4. Server band karne ke liye terminal mein `Ctrl+C` dabayein.

## Files

- `indexx.html` - Main page, CSS styles, business settings, and JavaScript functionality.
- `header.html` - Site header and navigation.
- `home.html` - Hero and highlights.
- `products.html` - Product section layout.
- `products.json` - Product names, categories, descriptions, and image paths.
- `services.html` - Services section.
- `about.html` - About section.
- `gallery.html` - Gallery images.
- `contact.html` - Contact information, enquiry form, and map.
- `footer.html` - Footer and floating contact links.
- `*.jpeg` - Local product images.

## Content Edit Karna

- **Business details:** `indexx.html` mein `BUSINESS` object edit karein. WhatsApp number country code ke saath digits-only format mein rakhein, jaise `919588010003`.
- **Products:** `products.json` mein ek naya object add karein. `id` unique rakhein; `image` mein image file ka naam ya image URL dein. Nayi category filter aur enquiry form mein automatically aa jayegi.
- **Images:** Local image files isi folder mein rakhein aur `products.json` ke `image` value mein exact filename likhein.
- **Page sections:** Upar diye gaye matching `.html` file ko edit karein. Section ke IDs aur JavaScript dwara use kiye ja rahe element IDs ko bina corresponding script update kiye rename na karein.
- **Colors and layout:** `indexx.html` ke `<style>` block mein CSS edit karein.

Section files ko alag edit kiya ja sakta hai, lekin unhe load karne ke liye website local server ke through chalani hogi.
