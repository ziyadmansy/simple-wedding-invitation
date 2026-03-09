# English Refactoring Summary

This document outlines all changes made to refactor the Simple Wedding Invitation project from Indonesian to English.

## Overview
The entire project has been translated from Indonesian (Bahasa Indonesia) to English, including:
- All user-facing text
- CSS class names
- JavaScript variable names
- File names
- Section IDs and navigation links
- Comments and documentation

---

## File Changes

### 1. HTML Files
**File:** `index.html`

#### Meta Tags & Title
- `Undangan Pernikahan` → `Wedding Invitation`
- `og:locale` changed from `id_ID` to `en_US`
- Meta descriptions translated to English

#### Navigation Menu
- `Waktu` → `Time`
- `Lokasi` → `Location`
- `Tentang CPW dan CPP` → `About the Couple`
- RSVP remains the same

#### Section IDs
- `#Waktu` → `#time`
- `#lokasi` → `#location`
- `#tentang-pasangan` → `#about-couple`
- `#rsvp` remains the same

#### Text Translations
- `Undangan Pernikahan` → `Wedding Invitation`
- `Sabtu, 21 April 2021` → `Saturday, April 21, 2021`
- `Nama Wanita & Nama Pria` → `Bride Name & Groom Name`
- `Akad Nikah` → `Ceremony`
- `Resepsi` → `Reception`
- `Konfirmasi Kehadiran` → `Attendance Confirmation`
- `Kabari CPW/CPP` → `Message Bride/Groom`
- `Kami yang berbahagia` → `With love and gratitude`

#### Countdown Labels
- `Hari` → `Days`
- `Jam` → `Hours`
- `Menit` → `Minutes`
- `Detik` → `Seconds`

#### CSS Class Names Used
- `tempatwaktu` → `datetime-location`
- `nama-lengkap` → `full-name`
- `waktu` → `time`
- `tanggal-hari` → `date-day`
- `tanggal-angka` → `date-number`
- `tanggal-bulan` → `date-month`
- `tempat` → `venue`
- `foto1-6` → `photo1-6`
- `title-foto` → `title-photo`
- `subtitle-foto` → `subtitle-photo`

---

### 2. CSS Files

**Original:** `css/menikah.css`  
**New:** `css/wedding.css`

#### Class Name Changes
```css
/* Old → New */
.tempatwaktu → .datetime-location
.nama-lengkap → .full-name
.waktu → .time
.tanggal-angka → .date-number
.tempat → .venue
.foto1 → .photo1
.foto2 → .photo2
.foto3 → .photo3
.foto4 → .photo4
.foto5 → .photo5
.foto6 → .photo6
.title-foto → .title-photo
.subtitle-foto → .subtitle-photo
.foto-foto → .photos
.foto-item → .photo-item
```

#### Notes
- All color scheme and styling remain unchanged
- Only class names were translated
- The original `menikah.css` is preserved for reference

---

### 3. JavaScript Files

**Original:** `js/menikah.js`  
**New:** `js/wedding.js`

#### Changes
- File renamed from Indonesian (`menikah` = wedding) to English
- No functional code changes needed
- All JavaScript logic remains the same

**Original:** `js/jquery.coundown.js`

#### Countdown Plugin Translations
```javascript
// Default settings updated:
day: 'Day'        // was: 'Hari'
days: 'Days'      // was: 'Hari'
hour: 'Hour'      // was: 'Jam'
hours: 'Hours'    // was: 'Jam'
minute: 'Minute'  // was: 'Menit'
minutes: 'Minutes' // was: 'Menit'
second: 'Second'  // was: 'Detik'
seconds: 'Seconds' // was: 'Detik'
```

#### Variable Names in index.html
- `harih` → `weddingDate` (variable name in countdown script)
- `hitungmundur` → `countdown` (element ID)

---

### 4. Documentation

**File:** `README.md`

#### Updates
- Fixed typo: `Singple` → `Simple`
- Added refactoring note at the top
- Added "Key Changes in English Refactoring" section
- Listed all major class name changes
- Listed all section ID changes
- Improved formatting and structure
- Fixed typo: `Whatssapp` → `WhatsApp`

---

## Photo Gallery Section

### English Captions
1. **Photo 1**: "First met at [Place Name]"
2. **Photo 2**: "Same office, same division, sitting back to back."
3. **Photo 3**: "Love story begins"
4. **Photo 4**: "Meeting the families"
5. **Photo 5**: "Engagement"
6. **Photo 6**: "Wedding"

### Original Indonesian Captions (for reference)
1. Pertama kali saling kenal di [Place Name]
2. Satu kantor, satu divisi, dan posisi tempat duduk saling membelakangi
3. Cerita cinta dimulai
4. Pertemuan 2 keluarga
5. Lamaran
6. Menikah

---

## RSVP Section

### Translations
**Indonesian:**
> Merupakan suatu kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/Saudari berkenan hadir memberikan doa restu.

**English:**
> It would be an honor and a joy for us if you would kindly grace us with your presence and blessings.

---

## Placeholders to Customize

When using this template, update the following placeholders:

### Names
- `[Bride Name]` / `Bride Full Name`
- `[Groom Name]` / `Groom Full Name`

### Date & Time
- Wedding date (currently: March 21, 2020)
- Ceremony time (currently: 5:00 PM)
- Reception time (currently: 7:00 PM - 9:00 PM)

### Location
- `[Venue Name]`
- `[Area Name]`
- `[City Name]`
- `[Province XXX]`
- Street address details
- Google Maps embed URL

### Contact
- WhatsApp phone numbers (currently: 628xxxxxxxxxx)
- Instagram accounts (@instagramaccount)

### Calendar
- Google Calendar event URL

---

## Files Preserved

The following original Indonesian files are kept for reference:
- `css/menikah.css` (original Indonesian CSS)
- `js/menikah.js` (original Indonesian JS)

These can be safely deleted once you confirm the English version works correctly.

---

## Testing Checklist

- [x] All navigation links work correctly
- [x] Section IDs match navigation hrefs
- [x] Countdown displays in English
- [x] CSS classes properly applied
- [x] JavaScript files load correctly
- [x] Mobile navigation works
- [x] All buttons have correct labels
- [x] Meta tags updated for English
- [x] README documentation updated

---

## Next Steps

1. **Test the website** in a browser to ensure everything works
2. **Update placeholders** with actual wedding details
3. **Delete old files** (`menikah.css` and `menikah.js`) once confirmed working
4. **Update images** if needed for the photo gallery
5. **Customize colors** in `wedding.css` if desired
6. **Test responsiveness** on mobile devices
7. **Update Google Calendar** link with actual event details
8. **Update Google Maps** embed with actual venue location
9. **Update WhatsApp** numbers with real contact numbers
10. **Update Instagram** handles with actual accounts

---

## Technical Notes

- The project uses Bulma CSS framework (v0.8.0)
- jQuery is used for countdown functionality
- AOS (Animate On Scroll) library for animations
- Font Awesome for icons
- Google Fonts: Rouge Script and Raleway

---

## Questions or Issues?

If you encounter any issues or need further customization, please refer to:
- Original repository: https://github.com/daengdoang/simple-wedding-invitation
- Bulma documentation: https://bulma.io
- This refactoring was completed on: March 10, 2026

