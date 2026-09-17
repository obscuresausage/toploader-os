# Toploader OS

**A local-first desktop app for trading card sellers and collectors.**

Toploader OS brings everything you need to run a card-selling operation and
manage a personal collection into one fast, private, offline-friendly desktop
application. It pairs marketplace-focused **Seller** tools — inventory,
fee-aware pricing, exports, shows and analytics — with a full **Collector**
workspace for binders, decks, set tracking, wishlists and trades, a parallel
**Pokémon** collecting experience, and a webcam-powered **Camera Card
Scanner** for getting physical cards into the app fast.

> Built for Magic: The Gathering and Pokémon TCG, powered by local card data
> from Scryfall and TCGDex, and designed so your collection and sales data
> stay on your own machine.

<!-- Replace these with real badges/links once published -->
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS-blue)
![Built with](https://img.shields.io/badge/built%20with-Python%20%2B%20Qt%20(PySide6)-3776AB)
![Status](https://img.shields.io/badge/release-v1.6.0-brightgreen)

---

## Contents

- [What is Toploader OS?](#what-is-toploader-os)
- [Modes](#modes)
- [Seller Mode](#seller-mode)
- [Collector Mode](#collector-mode)
- [Pokémon Mode](#pokémon-mode)
- [Camera Card Scanner (Scanning Lab)](#camera-card-scanner-scanning-lab)
- [Live Tools & OBS overlays](#live-tools--obs-overlays)
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

Toploader OS is a Windows and macOS desktop application that helps you:

- **Sell cards** through marketplaces (with a focus on Whatnot workflows):
  manage stock, price with marketplace fees in mind, build shows, export
  listings, and track sales and profit.
- **Collect cards**: catalogue your collection in visual binders, track set
  completion, build and manage decks, keep a wishlist, and record trades —
  for both Magic: The Gathering and Pokémon TCG.
- **Scan physical cards** straight into your inventory or collection with a
  webcam, instead of searching for each one by hand.

It's **local-first** — your inventory, collection, deck, trade, cache and
settings data live on your own device unless you choose to export or back
them up. Card information and prices come from a local cache of Scryfall
(Magic) and TCGDex (Pokémon) data that updates itself in the background.

---

## Modes

When you launch the app you choose a mode, and you can switch at any time.
Each mode is self-contained, so your selling tools and your collecting tools
never get in each other's way.

| | **Seller Mode** | **Collector Mode** | **Pokémon Mode** |
|---|---|---|---|
| For | Running a card-selling business | Managing an MTG collection | Managing a Pokémon TCG collection |
| Core | Inventory, sales, shows, exports | Binders, decks, sets, wishlist, trades | Binders, search, wishlist |
| Pricing | Fee-aware marketplace pricing | Market value in your display currency | Market value in your display currency |

The **Camera Card Scanner** and **Live Tools overlays** work across Seller
and Collector Mode — see their own sections below.

---

## Seller Mode

Everything you need to run marketplace sales, with a focus on Whatnot:

- **Inventory & stock management** — a fast, searchable inventory that stays
  responsive even with very large stock lists.
- **Fee-aware pricing** — pricing that accounts for marketplace fees, with
  configurable rounding (including threshold-based rounding for cheap cards).
- **Whatnot exports & reconciliation** — generate marketplace-ready listings
  and reconcile sales back against your inventory.
- **Whatnot Ledger import** — import a Whatnot Ledger CSV export directly:
  sales, payouts, tips, rewards and giveaway/break costs matched against your
  inventory in one pass, including automatic break-spot grouping for box
  breaks streamed live.
- **Platform exports** — export your singles to **TCGplayer**, **Cardmarket**
  and **eBay** CSV formats, with a card-picker so you choose exactly what's
  included.
- **Show Builder** — plan and prepare your selling shows.
- **Event Builder** — configure a live-sale event (box break or surprise
  set), then pull items into it from any of your inventory profiles with
  search, filtering and bulk "Add All".
- **Optimizer** — work out break/bundle economics from box cost, pack counts,
  bundle size and your target margin.
- **Live Tools** — OBS browser-source overlays for streaming (see
  [Live Tools & OBS overlays](#live-tools--obs-overlays)).
- **Seller analytics** — revenue trends and inventory distribution at a
  glance.
- **Scryfall-backed market pricing** for singles, converted into your
  currency.

---

## Collector Mode

A complete home for the Magic: The Gathering cards you keep.

### Visual binders
- Build unlimited binders and view cards as real images, not text rows.
- Add the **exact printing and finish** you own; nonfoil, foil and etched are
  tracked separately, and foil/special-treatment cards display with a shimmer
  overlay.
- **Favourites, tags and notes** on any card, plus pages and slots within a
  binder.
- **Duplicate finder** to surface extra copies across your collection.
- **Custom binder covers**, including card-art covers from your own
  collection.
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

## Pokémon Mode

A parallel collecting experience for Pokémon TCG, alongside your Magic
collection — not merged into it.

- **Visual binders** for your Pokémon cards, with the same real-card-image
  browsing as Collector Mode.
- **Search** the local Pokémon card database to add singles.
- **Wishlist** tracking for cards you're chasing.
- **Local card cache** synced from **TCGDex**, with pricing in your display
  currency (EUR/Cardmarket and USD/TCGPlayer, converted automatically).

---

## Camera Card Scanner (Scanning Lab)

Point a webcam at a physical card and Toploader OS matches it against a
locally-cached card index (perceptual image hashing plus real card-boundary
detection via OpenCV) — no manual searching required. Available from both
Seller and Collector Mode. *(Pro feature.)*

- **Auto-scan** captures automatically once a card settles in frame, with a
  settling gate (waits for the card to stop moving), blur rejection
  (out-of-focus captures are skipped), a live on-screen detection outline,
  and a duplicate-scan guard so the same card in frame isn't re-captured
  repeatedly.
- **Scan filters**: Ignore Promos, Prefer Foil, and Set Lock (pin matching to
  specific sets when a card has been printed in more than one you own).
- **Staged review** — scanned cards land in a batch list where you can adjust
  variant, finish, condition and quantity, with the matched card's art shown
  before committing. Correcting a mixed foil/nonfoil or mixed-printing stack
  splits the copies apart automatically rather than reassigning all of them.
- **Three destinations**: straight into an inventory profile, into a
  collector binder, or live onto the **Live Card Scan** stream overlay
  (with an auto-send toggle so scanned cards appear on stream with no manual
  click).
- A **chime plays on every successful scan**, pitched to the card's market
  value.
- The card index updates itself automatically in the background — no manual
  downloads required.

---

## Live Tools & OBS overlays

Independent browser-source overlays for streaming a live selling show, each
running on the same local overlay server so activating one doesn't interrupt
the others:

- **Pack Top Hits** — a carousel/gallery of the best cards pulled during box
  breaks.
- **Singles Reel** — a themed showcase of singles available now, either
  auto-generated (top by price) or hand-picked, from one inventory profile or
  all of them combined.
- **Members Board** — shoutouts/member call-outs, added and reordered live
  with an on-screen preview before it goes out.
- **Live Card Scan** — pushes each card scanned with the Camera Card Scanner
  live onto stream as it's captured.

---

## Screenshots

> _Add screenshots here once you've captured them, e.g.:_
>
> | Seller inventory | Collector binders | Camera Card Scanner |
> |---|---|---|
> | `docs/screenshots/seller.png` | `docs/screenshots/binders.png` | `docs/screenshots/scanner.png` |

---

## Download & install

1. Go to the [**Releases**](https://github.com/obscuresausage/toploader-os/releases) page.
2. Download the build for your platform:
   - **Windows** — either `Toploader-OS-vX.Y.Z-Windows-Setup.exe` (installer,
     no admin rights required, adds a Start Menu/desktop shortcut and a
     proper uninstaller) or `Toploader-OS-vX.Y.Z-Windows.zip` (portable, no
     install step — just extract and run).
   - **macOS** — `Toploader-OS-macOS-Apple-Silicon.dmg` (M-series Macs) or
     `Toploader-OS-macOS-Intel.dmg` (Intel Macs).
3. Windows portable zip: extract the folder anywhere and run
   **`Toploader OS.exe`**. macOS: open the DMG and drag **Toploader OS** into
   Applications.

Updating is as simple as installing/replacing with a newer release; your data
and licence are preserved automatically (see
[Your data & privacy](#your-data--privacy)).

---

## Getting started

1. Launch the app and pick **Seller**, **Collector**, or **Pokémon** mode
   (you can switch later).
2. **Sellers:** add stock to your inventory, set your fee/pricing preferences
   in Settings, then export or run a show.
3. **Collectors:** sync the card cache once from Collector/Pokémon →
   Settings, then start adding cards to a binder, browsing sets, or building
   a deck.
4. **Scanning cards:** open the Camera Card Scanner from Seller or Collector
   Mode, pick a destination (inventory, binder, or the live overlay), and
   point a webcam at your cards.

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
  reconciliation, Whatnot Ledger import, exports, bulk pricing), all
  Collector features, and the Camera Card Scanner.

Activate a licence from within the app. Licences are validated through Lemon
Squeezy's public License API.

---

## Your data & privacy

Toploader OS is **local-first**. Your collection, inventory, deck, trade,
cache and settings data are stored on your device.

- **Where it lives:**
  - Windows: `%APPDATA%\Toploader OS\` (your user profile), kept separate
    from the app folder so updates never touch your data.
  - macOS: `~/Library/Application Support/Toploader OS`.
- **Automatic backups:** the app keeps rolling local backups of your
  databases, with one-click access to the backup folder and a workspace
  backup/restore that covers your databases, card cache and images.
- **Portable mode:** advanced users can run fully portable (data stored next
  to the executable) by placing a `portable.flag` file beside the app.
- **Network use:** the app contacts Scryfall (Magic card data/images/prices),
  TCGDex (Pokémon card data/images/prices), GitHub (update checks and the
  Camera Card Scanner's card-index updates), and Lemon Squeezy (licence
  validation). Card and collection data are not uploaded as part of normal
  use.

---

## Building from source

The Windows and macOS releases are produced with
[PyInstaller](https://pyinstaller.org/) in one-folder mode.

```bash
# 1. Create and activate a virtual environment (Python 3.11 or 3.12)
python -m venv .venv
.venv\Scripts\activate        # Windows
source .venv/bin/activate     # macOS

# 2. Install dependencies, including the Camera Card Scanner's
pip install -r requirements-release.txt

# 3. Run the app from source
python app.py

# 4. Build the distributable folder
pyinstaller Toploader_OS.spec --noconfirm --clean
# → dist/Toploader OS/Toploader OS.exe  (+ _internal/)
```

Windows: `build_release_windows.ps1` automates the steps above and can also
produce a portable zip (`-CreateZip`) or an Inno Setup installer
(`-CreateInstaller`, requires [Inno Setup](https://jrsoftware.org/isinfo.php)).
macOS: `build_release_macos.sh` does the equivalent, producing a signed `.app`
and DMG.

---

## Tech stack

- **Python 3.11 / 3.12**
- **PySide6 (Qt 6)** for the desktop UI
- **SQLite** (FTS5 + WAL) for inventory, sales and collector data
- **Scryfall** bulk data + API for Magic card data, images, rulings and prices
- **TCGDex** for Pokémon card data, images and prices
- **OpenCV**, **NumPy** and **imagehash** for the Camera Card Scanner's card
  detection and perceptual-hash matching
- **Pillow**, **requests**, **certifi**
- **PyInstaller** for packaging, **Inno Setup** for the Windows installer
- Icons by **Lucide**

---

## Acknowledgements

- Magic: The Gathering card data, images and prices from
  **[Scryfall](https://scryfall.com/)**.
- Pokémon TCG card data, images and prices from
  **[TCGDex](https://tcgdex.dev/)**.
- Icons from **[Lucide](https://lucide.dev/)**.
- Licensing via **[Lemon Squeezy](https://www.lemonsqueezy.com/)**.

---

## Disclaimer

Toploader OS is **licensed, not sold**. It is provided without warranties to
the maximum extent permitted by law.

Magic: The Gathering and Pokémon card names, images and related data belong
to their respective rights holders. Toploader OS is **not endorsed by or
affiliated with** Wizards of the Coast, The Pokémon Company, Scryfall,
TCGDex, Whatnot, Cardmarket, TCGplayer, GitHub or Lemon Squeezy.

---

## Support

- **Issues & bug reports:** please use the GitHub
  [Issues](https://github.com/obscuresausage/toploader-os/issues) page.
- **Releases & changelog:** see
  [Releases](https://github.com/obscuresausage/toploader-os/releases).
