# Session Context

## Project
A rebuilt website for **Maple Grove Chick-fil-A** (`www.chickfilamaplegrove.com`), scraped from Squarespace on May 2, 2026 and fully rebuilt from scratch as clean HTML/CSS.

---

## Folder Structure
```
/Users/kimballhansen/Desktop/Folder/
├── context.md                  ← this file
├── site/                       ← ACTIVE SITE (work here)
│   ├── index.html              (Welcome / home page)
│   ├── catering.html
│   ├── joinourteam.html
│   ├── whoweare.html
│   ├── cfa-one.html
│   ├── our-food.html           (nav label: "Our Menu")
│   ├── stafflogin.html
│   ├── styles.css              (single shared stylesheet for all pages)
│   └── images/
│       ├── 230331_CFA_Logo_Script-Black_RGB_master.png   ← used in hero
│       ├── 230331_CFA_Logo_Script-White_CMYK_high-res.png
│       ├── 230331_CFA_Logo_Script-Outline-Red_PMS_high-res.png
│       ├── 230331_CFA_Logo_CSymbol-Square-Black_RGB_master.png
│       ├── 230331_CFA_Logo_One-Horiz-Black_RGB_master.png
│       └── 230331_CFA_Animation_Logo-Script_master.mp4   ← original (unused)
└── squarespace/                ← archived original scraped files (do not touch)
```

---

## Dev Server
Run from the `site/` folder:
```
cd /Users/kimballhansen/Desktop/Folder/site && python3 -m http.server 8080
```
Access at: `http://localhost:8080`

---

## Current State of the Site

### Design
- **Nav:** Red (`#E4002B`) sticky top bar with links to all 7 pages. Active page is highlighted.
- **Welcome page hero:** White background, split two-column layout. Left side: red title text ("Welcome to Chick-fil-A Maple Grove") in Playfair Display serif font + subtitle + two buttons. Right side: CFA black logo image (`230331_CFA_Logo_Script-Black_RGB_master.png`).
- **All other pages:** Red page header banner, white content sections, alternating off-white panels.
- **Shared stylesheet:** `styles.css` — all style changes apply site-wide.
- **Font:** Playfair Display (Google Fonts) for the hero title. System sans-serif everywhere else.
- **Colors:** Red `#E4002B`, white `#ffffff`, off-white `#f9f7f5`, muted gray `#555555`.

### Pages
| File | Nav Label | Status |
|------|-----------|--------|
| index.html | Welcome | Complete — hero with logo image |
| catering.html | Catering | Complete — packages + request form |
| joinourteam.html | Join Our Team | Complete — perks, open roles, apply form |
| whoweare.html | Who We Are | Complete — operator bio, values, history |
| cfa-one.html | CFA One | Complete — rewards tiers, app info |
| our-food.html | Our Menu | Complete — sandwiches, nuggets, sides, breakfast |
| stafflogin.html | Staff Login | Complete — simple login form |

### Tools Installed
- **ffmpeg** installed via Homebrew (used to strip audio from video; video later replaced with image)

---

## Session 2 Changes (May 6, 2026)

### Catering Page (`catering.html`)
- Added real photo to **Trays** card under "Two Ways to Cater": `Catering Lifestyle Image - New Year's - Chick-fil-A Nuggets Tray 03 1_master.png`
- Condensed breakfast + lunch/dinner into one **"What We Offer"** section (3-column grid): Breakfast Trays, Prepackaged Meals, Lunch & Dinner Trays. Removed Prepackaged Breakfast card.
- Replaced the catering request form entirely with a simple **"Ready to Order?"** CTA section — two buttons: "Order Online" (links to `chick-fil-a.com/catering`) and "Call (763) 307-0375"

### CFA One Page (`cfa-one.html`)
- Replaced the `<h1>Chick-fil-A One</h1>` heading with the **CFA One logo image** (`230331_CFA_Logo_One-Horiz-Black_RGB_master.png`)
- Fixed **"Download the App"** button — now links to the Chick-fil-A App Store listing (`apps.apple.com/us/app/chick-fil-a/id488818252`)

---

## What Still Needs Work
- All pages have **placeholder content** — real copy, photos, address, and operator info need to be filled in
- `img-placeholder` divs throughout pages are waiting for real photos
- `[Address]` on the welcome page needs the real address
- Staff login has no backend — purely visual for now
- Site has not been deployed to Vercel yet
