# Cairo Classifieds 🗂️

🌐 **Live Demo:** https://cairo-classifieds.pages.dev


A multi-page classifieds directory built using **pure HTML5**, laid out entirely with old-school `<table>`-based structure instead of modern CSS layout.

The project presents a fictional classifieds platform where users can browse listings by category, read detailed individual ads, post a new classified ad, and get in touch with the site's team — all styled the way websites were commonly built before CSS became standard.

## Overview

Cairo Classifieds is a table-layout HTML project created to practice building a complete multi-page website the way it was done in the pre-CSS era: using nested `<table>` elements to structure the page skeleton (header, navigation sidebar, content, and footer), rather than semantic layout tags.

The goal of this project was to focus on:
- Table-based page layout and nested tables
- Multi-page site structure and consistent navigation
- Forms laid out using table rows for label/input alignment
- Media elements
- Linking within and across pages, including anchor-based jump links
- Proper use of legacy presentational HTML attributes

## Pages

### 🏠 Home Page
- Full page skeleton built from a single outer `<table>` (header row, nav + content row, footer row)
- Site logo and title in the header
- Embedded HTML5 video with poster fallback
- "Today's Featured Listings" table with photos, titles, category, price, and location
- Reasons to use the site as a bullet list

### 📋 Browse Categories Page
- Four category sections (Jobs, For Sale, Housing, Services), each in its own `<table>`
- In-page jump links using the legacy `<a name="...">` anchor style
- Listings link across files directly into specific sections of `listing-detail.html`

### 📖 Listing Details Page
- Three individual listings, each inside its own nested layout table (photo cell + details cell)
- A details table per listing for category, price/rent/rate, condition, location, and posting date
- Embedded Google Maps `<iframe>` on the housing listing
- Contact email links per listing

### 📝 Post an Ad Page
- A full classified ad submission form laid out entirely with a table, aligning labels and inputs by row
- Wide range of input types: text, number, select, textarea, email, tel, file, radio, checkbox
- Submit and reset buttons

### ✉️ Contact Us Page
- A contact form using the same table-aligned label/input pattern
- An "Office Details" table for address, email, and hours
- Embedded Google Maps `<iframe>` for the office location

## Technologies Used

- HTML5

No external libraries, frameworks, CSS, or JavaScript were used.

## Table & Legacy Elements Practiced

This project relies on `<table>` for layout rather than semantic sectioning, alongside deprecated presentational tags and attributes that were common before CSS:
- `<table>` / `<tr>` / `<td>` (nested, for both page layout and data display)
- `border`, `cellpadding`, `cellspacing`
- `bgcolor`, `align`, `valign`, `width`
- `<font face="..." size="...">`
- `<a name="...">` for in-page anchors
- `colspan`
- `<form>`, `<label>`, `<select>`, `<textarea>`, `<button>`
- `<iframe>`, `<video>` / `<source>`
- `<address>`, `<time>`

## Notes

Deprecated tags and attributes such as `<font>`, `border`, `cellpadding`, and `cellspacing` were used intentionally, since no CSS exists anywhere in this project. They were the only way to give the page any visual structure without external styling, and are included purely to practice this older layout technique.

Every page repeats the same outer table skeleton (header, nav sidebar, footer) by hand across all five files, since no templating, CSS, or JavaScript was used. Links between pages use relative paths, so all files and the accompanying `images/` folder must stay together for the site to work correctly.

## Project Purpose

This project is part of my HTML learning journey, focused specifically on understanding how websites were structured using table-based layouts before CSS existed, in contrast to the semantic HTML5 approach used in my other projects.

## Future Improvements

Possible improvements:
- Rebuild the layout using semantic HTML5 and modern CSS (Flexbox/Grid)
- Add JavaScript form validation
- Connect the post-ad and contact forms to a backend
- Add dynamic listing data using an API
- Add Web Accessibility (ARIA roles and attributes)

## Author

**Fares Mohamed**

© 2026 Cairo Classifieds