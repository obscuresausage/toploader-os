# Toploader OS

**A local-first desktop app for trading card sellers and collectors.**

Toploader OS brings everything you need to run a card-selling operation and
manage a personal collection into one fast, private, offline-friendly desktop
application. It pairs marketplace-focused **Seller** tools — inventory,
fee-aware pricing, exports, shows and analytics — with a full **Collector**
workspace for binders, decks, set tracking, wishlists and trades.

> Built for Magic: The Gathering, powered by local card data from Scryfall, and
> designed so your collection and sales data stay on your own machine.

<!-- Replace these with real badges/links once published -->
![Platform](https://img.shields.io/badge/platform-Windows-blue)
![Built with](https://img.shields.io/badge/built%20with-Python%20%2B%20Qt%20(PySide6)-3776AB)
![Status](https://img.shields.io/badge/release-v1.4.9-brightgreen)

---

## Contents

- [What is Toploader OS?](#what-is-toploader-os)
- [Two modes](#two-modes)
- [Seller Mode](#seller-mode)
- [Collector Mode](#collector-mode)
- [Screenshots](#screenshots)
- [Download & install](#download--install)
- [Getting started](#getting-started)
- [Pricing & licensing](#pricing--licensing)
- [Your data & privacy](#your-data--privacy)
- [Building from source](#building-from-source)
- [Tech stack](#tech-stack)
- [Acknowledgements](#acknowledgements)
- [Disclaimer](#disclaimer)
- [Support](#support)

---

## What is Toploader OS?

Toploader OS is a Windows desktop application that helps you:

- **Sell cards** through marketplaces (with a focus on Whatnot workflows):
  manage stock, price with marketplace fees in mind, build shows, export
  listings, and track sales and profit.
- **Collect cards**: catalogue your collection in visual binders, track set
  completion, build and manage decks, keep a wishlist, and record trades.

It's **local-first** — your inventory, collection, deck, trade, cache and
settings data live on your own device unless you choose to export or back them
up. Card information and prices come from a local cache of Scryfall data that
updates itself in the background.

---

## Two modes

When you launch the app you choose a mode, and you can switch at any time. Each
mode is self-contained, so your selling tools and your collecting tools never
get in each other's way.

| | **Seller Mode** | **Collector Mode** |
|---|---|---|
| For | Running a card-selling business | Managing a personal collection |
| Core | Inventory, sales, shows, exports | Binders, decks, sets, wishlist, trades |
| Pricing | Fee-aware marketplace pricing | Market value in your display currency |

---

## Seller Mode

Everything you need to run marketplace sales, with a focus on Whatnot:

- **Inventory & stock management** — a fast, searchable inventory that stays
  responsive even with very large stock lists.
- **Fee-aware pricing** — pricing that accounts for marketplace fees, with
  configurable rounding (including threshold-based rounding for cheap cards).
- **Whatnot exports & reconciliation** — generate marketplace-ready listings and
  reconcile sales back against your inventory.
- **Platform exports** — export your singles to **TCGplayer**, **Cardmarket** and
  **eBay** CSV formats, with a card-picker so you choose exactly what's included.
- **Show Builder** — plan and prepare your selling shows.
- **Optimizer** — work out break/bundle economics from box cost, pack counts,
  bundle size and your target margin.
- **Event Builder & Live Tools** — utilities for running live selling sessions.
- **Seller analytics** — revenue trends and inventory distribution at a glance.
- **Scryfall-backed market pricing** for singles, converted into your currency.

---

## Collector Mode

A complete home for the cards you keep — new in v1.4.9.

### Visual binders
- Build unlimited binders and view cards as real images, not text rows.
- Add the **exact printing and finish** you own; nonfoil, foil and etched are
  tracked separately, and foil/special-treatment cards display with a shimmer
  overlay.
- **Favourites, tags and notes** on any card, plus pages and slots within a
  binder.
- **Duplicate finder** to surface extra copies across your collection.
- **Custom binder covers**, including card-art covers from your own collection.
- A rich **card inspector** showing value, location, deck demand and physical
  allocations.

### Card search & set tracking
- Browse any set's full card list.
- **Set completion tracking** with owned vs. missing and available counts.

### Deck builder
- Build decks for any format, including commander and all boards.
- **Import deck lists** in the standard `1x Card Name (SET) 123` text format.
- **Binder allocation** — reserve the physical copies from your binders into a
  deck so you always know what's sleeved where.
- Decks reflect the **actual printing you allocate** (foil, alternate art, etc.).
- **Jump to a deck** directly from any card that's allocated to it.

### Wishlist
- Track cards you're chasing, with target prices and total missing value.

### Trades
- A **visual trade builder**: search the cards you're receiving, and pick the
  cards you're giving directly from your binders.
- Committing a trade **updates your collection automatically** — cards traded
  away are removed, cards received are added to a binder you choose.
- Full **trade history** with running totals and net value.

### Analytics
- **Collection value over time**, recorded automatically.
- **Distribution charts** by finish and rarity.
- Per-binder, per-set and per-deck breakdowns.

### Card data & pricing
- A **local cache** of card data, images and rulings for fast browsing.
- **Automatic background updates** keep your cache current with no manual syncing.
- **Currency-correct pricing** that uses regional (Cardmarket/EUR-aligned) prices
  for UK and European users so values match the real market.

---

## Screenshots

> _Add screenshots here once you've captured them, e.g.:_
>
> | Seller inventory | Collector binders | Deck builder |
> |---|---|---|
> | `docs/screenshots/seller.png` | `docs/screenshots/binders.png` | `docs/screenshots/decks.png` |

---

## Download & install

1. Go to the [**Releases**](https://github.com/obscuresausage/toploader-os/releases) page.
2. Download the latest `Toploader-OS-vX_Y_Z-Windows.zip`.
3. Extract the folder anywhere you like.
4. Run **`Toploader OS.exe`**.

No installer and no admin rights are required — it's a self-contained folder.
Updating is as simple as replacing the folder with a newer release; your data
and licence are preserved automatically (see [Your data & privacy](#your-data--privacy)).

---

## Getting started

1. Launch the app and pick **Seller** or **Collector** mode (you can switch later).
2. **Sellers:** add stock to your inventory, set your fee/pricing preferences in
   Settings, then export or run a show.
3. **Collectors:** sync the card cache once from Collector → Settings, then start
   adding cards to a binder, browsing sets, or building a deck.

---

## Pricing & licensing

Toploader OS is free to try, with paid plans that lift the free-tier limits.

**Free tier includes:**

- Up to **100** seller inventory items
- Up to **3** collector binders
- Up to **5** decks
- Up to **1,000** collection cards

**Paid plans** (via [Lemon Squeezy](https://www.lemonsqueezy.com/)):

- **Collector** — unlocks Collector Mode limits and tools.
- **Pro** — unlocks everything, including the Seller tools (Whatnot
  reconciliation, exports, bulk pricing) and all Collector features.

Activate a licence from within the app. Licences are validated through Lemon
Squeezy's public License API.

---

## Your data & privacy

Toploader OS is **local-first**. Your collection, inventory, deck, trade, cache
and settings data are stored on your device.

- **Where it lives (Windows):** `%APPDATA%\Toploader OS\` (your user profile),
  kept separate from the app folder so updates never touch your data.
- **Automatic backups:** the app keeps rolling local backups of your databases,
  with one-click access to the backup folder and a workspace backup/restore that
  covers your databases, card cache and images.
- **Portable mode:** advanced users can run fully portable (data stored next to
  the executable) by placing a `portable.flag` file beside `Toploader OS.exe`.
- **Network use:** the app contacts Scryfall for card data, images and prices,
  GitHub to check for updates, and Lemon Squeezy to validate licences. Card and
  collection data are not uploaded as part of normal use.

---

## Building from source

The Windows release is produced with [PyInstaller](https://pyinstaller.org/) in
one-folder mode.

```bash
# 1. Create and activate a virtual environment (Python 3.12)
python -m venv .venv
.venv\Scripts\activate

# 2. Install dependencies
pip install pyside6 pillow certifi requests pyinstaller

# 3. Run the app from source
python app.py

# 4. Build the distributable folder
pyinstaller "Toploader OS.spec" --noconfirm --clean
# → dist/Toploader OS/Toploader OS.exe  (+ _internal/)
```

Then zip the **contents** of `dist/Toploader OS/` so the executable sits at the
zip root.

---

## Tech stack

- **Python 3.12**
- **PySide6 (Qt 6)** for the desktop UI
- **SQLite** (FTS5 + WAL) for inventory, sales and collector data
- **Scryfall** bulk data + API for card data, images, rulings and prices
- **Pillow**, **requests**, **certifi**
- **PyInstaller** for packaging
- Icons by **Lucide**

---

## Acknowledgements

- Card data, images and prices from **[Scryfall](https://scryfall.com/)**.
- Icons from **[Lucide](https://lucide.dev/)**.
- Licensing via **[Lemon Squeezy](https://www.lemonsqueezy.com/)**.

---

## Disclaimer

Toploader OS is **licensed, not sold**. It is provided without warranties to the
maximum extent permitted by law.

Magic: The Gathering card names, images and related data belong to their
respective rights holders. Toploader OS is **not endorsed by or affiliated with**
Wizards of the Coast, Scryfall, Whatnot, Cardmarket, TCGplayer, GitHub or Lemon
Squeezy.

---

## Support

- **Issues & bug reports:** please use the GitHub
  [Issues](https://github.com/obscuresausage/toploader-os/issues) page.
- **Releases & changelog:** see
  [Releases](https://github.com/obscuresausage/toploader-os/releases).
