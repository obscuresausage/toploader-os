# 🛡️ Toploader OS

**Toploader OS** is a powerful, all-in-one desktop dashboard designed specifically for Trading Card Game (TCG) sellers and WhatNot streamers. Built with Python and CustomTkinter, it automates the most tedious parts of selling: calculating complex platform fees, optimizing break margins, managing dynamic inventory, and generating bulk-upload CSVs.

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![CustomTkinter](https://img.shields.io/badge/GUI-CustomTkinter-darkgreen.svg)
![Scryfall](https://img.shields.io/badge/API-Scryfall-purple.svg)

---

## ✨ Key Features

* **📦 Smart Inventory Management:** Import bulk CSVs directly from Manabox. Toploader OS automatically interfaces with the Scryfall API to fetch live market prices, high-quality card images, and specific foil/etched variants in the background.
* **📤 1-Click WhatNot CSV Exports:** Select items from your database grid and instantly generate a perfectly formatted WhatNot bulk-upload CSV. Customize listing types (Auction/Buy It Now), card conditions, and precise shipping profiles on a per-item basis.
* **🔨 Pack Break Builder & Optimizer:** Input your box costs and target margins to calculate the exact required sale prices for bundles or mixers. The app automatically accounts for UK WhatNot fees, payment processing, and VAT.
* **⚖️ Live Set Balancer:** Running an auction? Track your live sales during a stream. If a slot sells high, the built-in balancer will dynamically lower the required floor price for your remaining slots so you always hit your exact target margin.
* **📝 Live Break Recorder:** Easily assign usernames to randomized slots (Color Breaks or Digi Breaks) and generate a clean `.txt` Pull Sheet to use during shipping.
* **🎨 Dynamic Desktop UI:** Features a sleek dark-mode interface, custom sliding toast notifications, and a daily randomized MTG flavor text generator!

---

## 🚀 Downloading and Running the App

If you just want to use the application for your streams, you do not need to download the source code! 

1. Navigate to the **[Releases](../../releases)** tab on the right side of this repository.
2. Download the latest `Toploader_OS.exe` file.
3. Place the `.exe` in its own dedicated folder. *(Note: The app will generate a few local image folders and a `inventory.json` database file next to it when you start adding cards).*
4. Double-click to run and start optimizing your streams!

---

## ⚖️ Legal & Attributions

### Intellectual Property
Toploader OS acts as a third-party tool and interfaces with external APIs (Scryfall). Toploader OS is unofficial Fan Content permitted under the Fan Content Policy. Not approved/endorsed by Wizards. Portions of the materials used are property of Wizards of the Coast. ©Wizards of the Coast LLC.

### Third-Party Assets
UI Icons provided by Icons8.

Card data and imagery provided by the Scryfall API.

### License
This compiled software is provided as proprietary freeware. You may download and use the application for personal and commercial business use. You may not modify, decompile, sub-license, or sell this software. See the LICENSE.txt file for full terms and conditions.

### 💖 Acknowledgements
Created by Magic Sausage.

A massive thank you to the open-source Python community, the incredible team at Scryfall, and all the GitHub supporters who helped make this project a reality!
