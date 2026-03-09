# Quick Customization Guide

This is a quick reference for customizing your wedding invitation website after the English refactoring.

## 🚀 Quick Start

1. Open `index.html` in your text editor
2. Search and replace the placeholders below
3. Save and test in your browser

---

## 📝 Essential Customizations

### 1. Couple Names
**Search for:** `Bride Name` and `Groom Name`  
**Replace with:** Your actual names

**Locations in file:**
- Line ~8: Page title
- Line ~10: Meta tags
- Line ~99: Hero section
- Line ~195: Full names section

---

### 2. Wedding Date & Time
**Current:** Saturday, March 21, 2020

**Search for:** `03/21/2020 17:00:00`  
**Replace with:** Your wedding date in format: `MM/DD/YYYY HH:MM:SS`

**Locations:**
- Line ~129: Countdown timer script
- Line ~102: Display date in hero
- Line ~224: Date display in Time section

**Also update:**
- Ceremony time: Line ~233 (currently `5:00 PM`)
- Reception time: Line ~241 (currently `7:00 PM - 9:00 PM`)

---

### 3. Venue Information

#### Venue Name
**Search for:** `[Venue Name]` or `Venue Name`  
**Replace with:** Your actual venue name

#### Address
**Search for:** 
- `[Area Name]`
- `[City Name]`
- `Street Address No.9, RT.001/RW.006A`
- `District XXX, City XXX, Province XXX`

**Replace with:** Your complete venue address

**Location in file:** Line ~275-280

---

### 4. Google Maps

**Search for:** The `<iframe>` tag starting with `https://www.google.com/maps/embed`

**How to get your map:**
1. Go to Google Maps
2. Search for your venue
3. Click "Share" → "Embed a map"
4. Copy the iframe code
5. Replace the entire iframe in line ~282

**Also update the directions link:**
- Line ~287: Replace the href URL with your venue's Google Maps link

---

### 5. WhatsApp Contact

**Search for:** `628xxxxxxxxxx`  
**Replace with:** Your actual WhatsApp numbers (with country code, no + sign)

**Locations:**
- Line ~405: Bride's WhatsApp
- Line ~413: Groom's WhatsApp

**Format:** Country code + number (e.g., `1234567890` for US)

---

### 6. Instagram Handles

**Search for:** `@instagramaccount`  
**Replace with:** Your actual Instagram handles

**Locations:**
- Line ~432: Bride's Instagram
- Line ~436: Groom's Instagram

**Also update the URLs:**
- Replace `https://instagram.com/instagramaccount` with your actual profile URLs

---

### 7. Google Calendar Link

**Search for:** `https://calendar.google.com/event?action=TEMPLATE...`

**How to create:**
1. Go to Google Calendar
2. Create your wedding event
3. Click the event → More actions → "Publish event"
4. Or use: https://calendar.google.com/calendar/render?action=TEMPLATE
5. Fill in the parameters

**Location in file:** Line ~259

---

### 8. Photo Gallery

**Images to replace:**
- `beatriz-perez-moya-M2T1j-6Fn8w-unsplash.jpg`
- `evelina-friman-hw_sKmjb0ns-unsplash.jpg`
- `jeremy-wong-weddings-464ps_nOflw-unsplash.jpg`
- `jeremy-wong-weddings-K8KiCHh4WU4-unsplash.jpg`
- `nathan-dumlao-5BB_atDT4oA-unsplash.jpg`
- `samantha-gades-x40Q9jrEVT0-unsplash.jpg`

**Options:**
1. Replace these files in the `image/` folder with your own photos (keep same filenames)
2. Or update the CSS file (`wedding.css`) lines 555-624 with your new image paths

**Photo captions to update:** Lines ~312-365

---

## 🎨 Color Customization

### Main Color Scheme
Open `css/wedding.css` and search for the color codes:

**Primary colors:**
- `#996E6D` - Dark dusty pink (main theme color)
- `#BC8887` - Lighter pink
- `#D8A9A8` - Dusty pink
- `#EDD2D1` - Light pink
- `#F4E2E2` - Lightest pink

**Find and replace** these hex codes with your preferred colors throughout the CSS file.

**Main locations:**
- Line ~29: Active navbar border
- Line ~290: Section titles
- Line ~298: Name styling
- Line ~402: Buttons
- Line ~432: Preloader background

---

## ⚙️ Timezone

**Search for:** `offset: +7`  
**Location:** Line ~130 in the countdown script

**Replace with:** Your timezone offset
- UTC+0: London
- UTC-5: New York (EST)
- UTC-8: Los Angeles (PST)
- UTC+7: Bangkok
- etc.

---

## 🖼️ Background Image

**Search for:** `https://picsum.photos/id/381/1920/1080`  
**Location:** Line ~38 in CSS (`.hero` class)

**Replace with:** Your own hero background image URL or local path

---

## ✅ Testing Checklist

After customization:

- [ ] Names are correct everywhere
- [ ] Wedding date and time are accurate
- [ ] Countdown timer works
- [ ] Venue address is complete
- [ ] Google Maps shows correct location
- [ ] WhatsApp numbers work (click to test)
- [ ] Instagram links work
- [ ] Google Calendar link works
- [ ] All photos display correctly
- [ ] Colors match your theme
- [ ] Test on mobile device
- [ ] Test all navigation links

---

## 📱 Mobile Testing

Test these breakpoints:
- Desktop: 1920px
- Tablet: 768px
- Mobile: 375px

The site uses Bulma CSS which is responsive by default.

---

## 🆘 Common Issues

### Countdown not working
- Check the date format: `MM/DD/YYYY HH:MM:SS`
- Verify timezone offset
- Make sure date is in the future

### Map not showing
- Check if iframe code is complete
- Verify the venue exists on Google Maps
- Check for any console errors

### WhatsApp not opening
- Verify phone number format (no spaces, no + sign)
- Test on a device with WhatsApp installed

### Images not loading
- Check file paths are correct
- Verify images exist in `/image/` folder
- Check image filenames match exactly (case-sensitive)

---

## 🔧 Advanced Customization

For more advanced changes, refer to:
- `REFACTORING_SUMMARY.md` - Complete list of all changes
- `README.md` - Project overview
- Bulma documentation: https://bulma.io/documentation/

---

## 📁 File Structure

```
simple-wedding-invitation/
├── index.html              ← Main file to edit
├── css/
│   └── wedding.css         ← Styles and colors
├── js/
│   └── wedding.js          ← JavaScript functionality
├── image/                  ← Replace photos here
└── README.md
```

---

**Last Updated:** March 10, 2026  
**Language:** English  
**Original:** Indonesian (refactored)

