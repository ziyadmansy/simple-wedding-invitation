# ✅ Post-Refactoring Checklist

Use this checklist to track your progress after the English refactoring.

---

## Phase 1: Initial Testing (Do This First!)

- [ ] Open `index.html` in a web browser
- [ ] Verify the page loads without errors
- [ ] Check browser console for any JavaScript errors (F12)
- [ ] Test all navigation menu links (Home, Time, Location, About, RSVP)
- [ ] Verify countdown timer is working
- [ ] Check that all text appears in English
- [ ] Test on mobile device or mobile view
- [ ] Verify all images are loading
- [ ] Test WhatsApp buttons (should open WhatsApp)
- [ ] Test Google Maps link

**If all items above pass, proceed to Phase 2!**

---

## Phase 2: Content Customization

### Names & Branding
- [ ] Replace "Bride Name" with actual bride name (search entire file)
- [ ] Replace "Groom Name" with actual groom name (search entire file)
- [ ] Update page title in `<title>` tag
- [ ] Update meta tags (og:title, og:description)

### Wedding Date & Time
- [ ] Update wedding date in countdown script (line ~129)
  - Current: `03/21/2020 17:00:00`
  - Format: `MM/DD/YYYY HH:MM:SS`
- [ ] Update date display in hero section (line ~102)
- [ ] Update date in Time section (line ~224)
- [ ] Update ceremony time (line ~233)
- [ ] Update reception time (line ~241)
- [ ] Verify timezone offset (line ~130)

### Venue Information
- [ ] Replace `[Venue Name]` with actual venue
- [ ] Update venue address (lines ~275-280)
- [ ] Update `[Area Name]` placeholder
- [ ] Update `[City Name]` placeholder
- [ ] Update `[District XXX]` placeholder
- [ ] Update `[Province XXX]` placeholder

### Google Maps
- [ ] Get Google Maps embed code for venue
- [ ] Replace iframe code (line ~282)
- [ ] Update directions link URL (line ~287)
- [ ] Test map displays correctly
- [ ] Test directions button works

### Contact Information
- [ ] Update Bride's WhatsApp number (line ~405)
  - Format: Country code + number (no + sign)
  - Example: `14155552671` for US number
- [ ] Update Groom's WhatsApp number (line ~413)
- [ ] Test both WhatsApp links on mobile
- [ ] Update Bride's Instagram handle (line ~432)
- [ ] Update Bride's Instagram URL
- [ ] Update Groom's Instagram handle (line ~436)
- [ ] Update Groom's Instagram URL
- [ ] Test all Instagram links

### Google Calendar
- [ ] Create Google Calendar event
- [ ] Get calendar event template link
- [ ] Replace calendar link (line ~259)
- [ ] Test "Add to Calendar" button

---

## Phase 3: Photo Gallery

### Replace Photos
- [ ] Prepare 6 wedding/engagement photos
- [ ] Optimize images (recommended: max 1920px width)
- [ ] Option A: Replace files in `/image/` folder with same names:
  - [ ] `beatriz-perez-moya-M2T1j-6Fn8w-unsplash.jpg`
  - [ ] `evelina-friman-hw_sKmjb0ns-unsplash.jpg`
  - [ ] `jeremy-wong-weddings-464ps_nOflw-unsplash.jpg`
  - [ ] `jeremy-wong-weddings-K8KiCHh4WU4-unsplash.jpg`
  - [ ] `nathan-dumlao-5BB_atDT4oA-unsplash.jpg`
  - [ ] `samantha-gades-x40Q9jrEVT0-unsplash.jpg`
- [ ] Option B: Update CSS paths in `wedding.css` (lines 555-624)

### Update Photo Captions
- [ ] Update Photo 1 caption (line ~312)
- [ ] Update Photo 1 location link
- [ ] Update Photo 2 caption (line ~320)
- [ ] Update Photo 3 caption (line ~330)
- [ ] Update Photo 4 caption (line ~345)
- [ ] Update Photo 5 caption (line ~353)
- [ ] Update Photo 6 caption (line ~361)

---

## Phase 4: Styling & Branding (Optional)

### Colors
- [ ] Review current color scheme
- [ ] If changing colors, update in `css/wedding.css`:
  - [ ] Primary color: `#996E6D`
  - [ ] Secondary color: `#BC8887`
  - [ ] Light color: `#F4E2E2`
  - [ ] Button colors
  - [ ] Navbar colors

### Background Image
- [ ] Review hero background image
- [ ] If changing, update CSS line ~38
- [ ] Test new image looks good on mobile

### Fonts
- [ ] Review font choices (Rouge Script & Raleway)
- [ ] If changing, update Google Fonts link
- [ ] Update font-family in CSS

### Favicon
- [ ] Create custom favicon (16x16, 32x32, 64x64)
- [ ] Replace `image/favicon.png`
- [ ] Clear browser cache and test

---

## Phase 5: Final Testing

### Desktop Testing
- [ ] Test in Chrome
- [ ] Test in Firefox
- [ ] Test in Safari
- [ ] Test in Edge
- [ ] Check all animations work
- [ ] Verify countdown updates every second
- [ ] Test all links open correctly
- [ ] Check for typos or grammar errors

### Mobile Testing
- [ ] Test on iOS (iPhone)
- [ ] Test on Android
- [ ] Test mobile navigation menu
- [ ] Verify text is readable on small screens
- [ ] Check images scale properly
- [ ] Test WhatsApp buttons on mobile device
- [ ] Verify map is interactive on mobile
- [ ] Test in portrait and landscape modes

### Responsive Testing
- [ ] 320px (small mobile)
- [ ] 375px (standard mobile)
- [ ] 768px (tablet)
- [ ] 1024px (small desktop)
- [ ] 1920px (large desktop)

### Content Verification
- [ ] All placeholder text replaced
- [ ] No "TODO" comments remaining
- [ ] All links work correctly
- [ ] All images load
- [ ] No console errors
- [ ] No broken links
- [ ] Grammar and spelling checked
- [ ] Contact information is correct
- [ ] Date and time are correct

---

## Phase 6: Performance Optimization

### Image Optimization
- [ ] Compress all JPEG images
- [ ] Ensure images are web-optimized
- [ ] Check total page load size (aim for <5MB)
- [ ] Test page load speed

### Code Cleanup
- [ ] Remove unused CSS (if any)
- [ ] Remove unused JavaScript (if any)
- [ ] Delete original Indonesian files:
  - [ ] `css/menikah.css`
  - [ ] `js/menikah.js`
- [ ] Minify CSS (optional)
- [ ] Minify JavaScript (optional)

---

## Phase 7: SEO & Meta Tags

- [ ] Update meta description with your wedding details
- [ ] Update og:title
- [ ] Update og:description
- [ ] Update og:image (add your photo URL after deployment)
- [ ] Update og:url (add your domain after deployment)
- [ ] Add structured data for events (optional)

---

## Phase 8: Deployment

### Pre-Deployment
- [ ] Final review of all content
- [ ] Test once more on multiple devices
- [ ] Get feedback from friends/family
- [ ] Fix any issues found

### Deployment to Netlify (Recommended)
- [ ] Create Netlify account
- [ ] Connect GitHub repository (if using Git)
- [ ] Or drag & drop project folder
- [ ] Configure custom domain (optional)
- [ ] Test deployed version
- [ ] Check all links work on live site
- [ ] Update og:url and og:image with live URLs

### Alternative Hosting
- [ ] Choose hosting provider
- [ ] Upload files via FTP/SFTP
- [ ] Configure domain
- [ ] Test live site
- [ ] Enable HTTPS

---

## Phase 9: Post-Deployment

### Sharing
- [ ] Get final URL
- [ ] Share with family and friends
- [ ] Share on social media
- [ ] Send in wedding invitations
- [ ] Test shared links render correctly

### Monitoring
- [ ] Set up Google Analytics (optional)
- [ ] Monitor site performance
- [ ] Check for broken links
- [ ] Monitor RSVP responses via WhatsApp

---

## Phase 10: Maintenance

### Before Wedding
- [ ] Update countdown as needed
- [ ] Add any last-minute changes
- [ ] Keep contact information current
- [ ] Monitor for technical issues

### After Wedding
- [ ] Consider adding wedding photos
- [ ] Update "Thank You" message
- [ ] Keep site live as a memento
- [ ] Download backup of site

---

## Troubleshooting Checklist

If something isn't working:

- [ ] Check browser console for errors (F12 → Console)
- [ ] Verify all file paths are correct
- [ ] Check that all external resources load (jQuery, Bulma, etc.)
- [ ] Clear browser cache and reload
- [ ] Test in incognito/private browsing mode
- [ ] Verify countdown date format is correct
- [ ] Check timezone offset setting
- [ ] Ensure all CSS/JS files are linked correctly
- [ ] Validate HTML (use W3C Validator)
- [ ] Check for typos in URLs or file names

---

## Quick Reference

**Key Files:**
- `index.html` - Main content
- `css/wedding.css` - Styling
- `js/wedding.js` - Interactive features
- `js/jquery.coundown.js` - Countdown timer

**Important Line Numbers:**
- Line 129: Countdown date
- Line 130: Timezone offset
- Line 259: Google Calendar link
- Line 282: Google Maps embed
- Line 405-413: WhatsApp numbers
- Line 432-436: Instagram handles

**Documentation:**
- `CUSTOMIZATION_GUIDE.md` - How to customize
- `REFACTORING_SUMMARY.md` - What changed
- `TRANSLATION_REFERENCE.md` - Translation details
- `README.md` - Project overview

---

## Completion Status

**Overall Progress:** [ ] 0% → Target: 100%

### Progress by Phase
- [ ] Phase 1: Initial Testing (0/10)
- [ ] Phase 2: Content Customization (0/28)
- [ ] Phase 3: Photo Gallery (0/13)
- [ ] Phase 4: Styling & Branding (0/12)
- [ ] Phase 5: Final Testing (0/27)
- [ ] Phase 6: Performance Optimization (0/10)
- [ ] Phase 7: SEO & Meta Tags (0/7)
- [ ] Phase 8: Deployment (0/13)
- [ ] Phase 9: Post-Deployment (0/7)
- [ ] Phase 10: Maintenance (0/7)

**Total Tasks:** 134

---

**Last Updated:** March 10, 2026  
**Status:** Ready for Customization  
**Language:** English

---

**Print this checklist or keep it handy as you work through the customization process!**

