# 📦 TopLoader OS: A WhatNot TCG Streamer ERP & Profit Calculator

A professional-grade, offline-first ERP, inventory manager, sales tracker, and profit calculator built specifically for Trading Card Game streamers selling on WhatNot.

TopLoader OS helps remove the guesswork from stream preparation by managing single-card and sealed inventory, pulling live Magic: The Gathering card data from Scryfall, calculating WhatNot fees, preparing WhatNot-compatible CSV exports, building profitable breaks, and tracking live sales performance.

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![PySide6](https://img.shields.io/badge/GUI-PySide6-41CD52.svg)
![Scryfall](https://img.shields.io/badge/API-Scryfall-purple.svg)
![Lucide](https://img.shields.io/badge/Icons-Lucide-orange.svg)
![WhatNot](https://img.shields.io/badge/Export-WhatNot%20CSV-red.svg)

---

## ✨ Key Features

### 🎨 Dynamic Interface & Themes
- **System-Aware Theming:** Toploader OS natively reads your Windows OS settings and adapts to Light Mode or Dark Mode instantly.
- **Custom Overrides:** Force the app into Light or Dark mode from the Settings menu.
- **Modern PySide6 Framework:** Fast, responsive UI with sidebar navigation, stacked pages, and custom Lucide vector icons.

### 🗃️ Inventory Management
- **Visual inventory grid:** Image-first inventory cards showing item image, card/product name, set and collector number, foil status, quantity in stock, and target sale price.
- **Table inventory view:** A compact spreadsheet-style view for fast scanning, database-style sorting, and bulk actions.
- **Toggleable views:** Switch between **Visual Grid** and **Table** directly from the Inventory page.
- **Smart item types:** Separate handling for **Single Cards**, **Booster Packs**, and **Sealed Boxes**.
- **Live search, filtering, and sorting:** Search inventory, filter by item type, and sort by name, quantity, or price.
- **Sidebar inspector:** Review item details, pricing, margins, and sale controls without leaving the Inventory page.
- **Hover Tooltips:** Hover over any visual card to instantly view a high-resolution preview of the product.

### 🔮 Scryfall Integration
- **Magic card autocomplete:** Search Magic: The Gathering cards as you type.
- **Variant & Promo tracking:** Pull specific printings, including exact Set Codes, collector numbers, and foil/etched finishes.
- **Market price lookup:** Use Scryfall pricing data to help calculate target sale prices.
- **Image retrieval:** Download and cache official Scryfall card images locally for visual inventory cards.

### 📥 Manabox CSV Import
- Import scanned collection data from Manabox CSV files.
- Automatically process imported cards into the local inventory database, perfectly formatting variant strings to prevent API mismatches.

### 🧮 Event & Break Builders
- **Unified Event Builder:** A dual-pane tool that combines Box Breaks and Surprise Sets. Type your desired slot quantity, and easily move bulk inventory back and forth to calculate exact floor pricing.
- **Break Optimizer:** Enter box cost, target margin, and slot details to calculate profitable bundle pricing for loose packs.
- **Live Break Recorder:** Track finalized randomizer assignments during a live stream.
- **Live Set Balancer:** Track auction sales during a break and dynamically recalculate the required minimum price of remaining slots to guarantee profitability.

### 📊 Sales Analytics
- **Daily sales summary:** Track gross revenue, total payout, net profit, and items sold.
- **7-day trend graph:** View recent performance as either a bar chart or line chart that matches your current app theme.
- **Editable sales records:** Correct transaction details from the Analytics page when needed.

### 📤 Smart WhatNot CSV Export
- Export selected inventory items to a WhatNot-compatible CSV upload file.
- **Smart Title Formatting:** Toggle exactly what gets included in your exported item titles directly from Settings (e.g., include/exclude Set Names, Collector Numbers, and Finishes to save character space).
- **Flawless Image Mapping:** Explicit `[SET_CODE]` parsing guarantees that "The List" cards and Promos export the correct image to WhatNot without dropping rows.
- Uses configurable category, subcategory, condition, listing type, and shipping profile defaults.

---

## 📦 Installation & Setup

TopLoader OS is distributed as a standalone Windows executable. 

1. Download the latest `ToploaderOS_vX.X.exe` from the Releases page.
2. Move the `.exe` to a dedicated folder on your PC (it will generate your local database files in whatever folder it lives in).
3. Double-click to run!

**⚠️ Note on Windows SmartScreen:**
Because Toploader OS is an independently developed tool, the executable is not signed with an expensive corporate Microsoft certificate. Windows may show a blue "SmartScreen" warning that says *Unknown Publisher* the first time you open it. To proceed, simply click **More Info** -> **Run Anyway**. 

---

## 🗂️ Project Structure & Local Data

TopLoader OS is offline-first. Your core data is stored locally in JSON files and image folders right next to your `.exe`. 

```text
TopLoader-Directory/
├─ ToploaderOS_v1.1.exe        # Main application
├─ inventory.json              # Local inventory data (auto-generated)
├─ sales.json                  # Local sales history (auto-generated)
├─ toploader_settings.json     # UI, fee, and default settings (auto-generated)
└─ inv_images/                 # Cached local card/product images
The app only requires internet access for online lookups such as Scryfall card searches, live exchange-rate checks, and fetching images.

🧮 Fee Calculation
TopLoader OS includes configurable WhatNot fee calculations so you can model your real payout accurately based on current UK/US rates.

Platform commission %

Payment processing %

Flat transaction fee

VAT on fees

Fee settings are configurable from the Settings page and saved locally to your database.

✅ Main App Sections
Inventory (Database, Quick Sales, and Item Creation)

Optimizer (Pack-based Bundle Math)

Event Builder (Box Breaks & Surprise Sets)

Live Tools (Break Recorder & Set Balancer)

Analytics (Financial Dashboards)

Settings (Fees, App Themes, & Export Defaults)

About

🔒 Legal & Disclaimer
TopLoader OS is an independent tool and is not affiliated with WhatNot, Scryfall, Manabox, Wizards of the Coast, or Lucide.

Scryfall: Data and images are used through Scryfall-powered lookups.

Lucide: Icons are used under the Lucide ISC license.

PySide6: Used under the GNU LGPLv3 license.
