# Toploader OS

**Toploader OS** is a Windows desktop workflow app for Magic: The Gathering sellers, breakers, streamers, and card-inventory builders. It helps you manage stock, price inventory, prepare Whatnot/eBay exports, reconcile sales, track profit, and keep your card workflow organised from one local desktop app.

Toploader OS is built for people who handle real stock: singles, sealed product, accessories, breaks, bundles, stream inventory, and seller admin.

> Toploader OS is not produced by, endorsed by, supported by, or affiliated with Wizards of the Coast, Scryfall, Whatnot, eBay, Cardmarket, GitHub, or Lemon Squeezy.

---

## Download

Download the latest public Windows release from GitHub Releases:

https://github.com/obscuresausage/toploader-os/releases

For the first public Windows release, download:

```text
Toploader-OS-v1.4.6-Windows.zip
```

Extract the ZIP and run:

```text
Toploader OS.exe
```

Keep `Toploader OS.exe` and the `_internal` folder together. This is a PyInstaller one-folder build, so moving the executable away from `_internal` will break the app.

### Windows security notice

Toploader OS may currently show a Windows “Unknown Publisher” or SmartScreen warning because the early release builds are not code-signed yet. Only download Toploader OS from the official GitHub Releases page or the official Toploader OS store links.

Checksums are provided with each release so users can verify the downloaded file.

---

## Upgrade to Pro

Toploader OS has a Free mode and a Pro mode.

Upgrade to Pro here:

https://toploaderos.lemonsqueezy.com/

After purchase, Lemon Squeezy provides a licence key. Open Toploader OS, go to **Settings → Toploader OS Pro**, paste your key, and activate it.

Once Pro is active, the app stores the licence state locally and validates the same device activation during normal use. Updating Toploader OS should not require a new activation as long as the user does not delete their local app data.

---

## Free vs Pro

### Free mode

Free mode is designed so users can try the core workflow before upgrading.

Free mode includes:

- Core inventory use.
- Manual item entry.
- Single-card lookup support.
- Pricing and fee tools.
- Basic analytics and local data storage.
- Up to 100 inventory items.

### Pro mode

Pro unlocks the full seller workflow:

- Unlimited inventory.
- Multiple inventory profiles/workspaces.
- ManaBox CSV import.
- Whatnot CSV export.
- eBay CSV export for single-card inventory.
- Whatnot sales reconciliation.
- Bulk edit workflows.
- Advanced inventory/export validation.
- Seller workflow tools designed for larger live-selling and stock-management use.

---

## Main features

### Inventory management

Toploader OS supports inventory for:

- Single cards.
- Booster packs.
- Sealed boxes.
- Card sleeves.
- Deck boxes.
- Playmats.
- 3D printed accessories.
- Binders and portfolios.
- Storage boxes.
- Toploaders and card savers.
- Card stands.
- Dice, counters, and tokens.
- Bundles/lots.
- Graded cards.
- Other TCG products and accessories.

The inventory view includes search, sorting, quick filters, visual cards, table mode, stock adjustment, duplicate-single handling, and product-specific pricing fields.

### Scryfall-powered card lookup

For Magic: The Gathering singles, Toploader OS uses Scryfall to fetch card suggestions, exact printings, images, set data, collector numbers, finish data, artists, Cardmarket links, and market price metadata.

Useful single-card tools include:

- Autocomplete card search.
- Exact printing/finish selection.
- Local image caching.
- Public image URL storage for marketplace CSVs.
- Market-price refresh.
- Manual target sale-price override when no market price exists.
- Duplicate-card merge prompts.

### Inventory analytics

Toploader OS includes stock analytics for understanding the shape and value of your inventory.

Analytics can include:

- Total stock value.
- Singles value.
- Sealed/product value.
- Estimated payout.
- Estimated profit.
- Missing images.
- Missing prices.
- Zero-quantity lines.
- Ready-for-export counts.
- Card analytics such as mana colour density, set distribution, and rarity split where Scryfall metadata is available.

### Sales analytics

The app can log sales and track seller performance over time.

Sales analytics include:

- Gross revenue.
- Total payout.
- Net profit.
- Items sold.
- Date-range views.
- Charted sales trends.
- Transaction editing/deleting with stock restoration support.

### Whatnot workflow support

Toploader OS is designed around real live-selling prep.

Whatnot-related tools include:

- Whatnot CSV export.
- Export validation before upload.
- Public image URL checks.
- Listing title and description templates.
- Shipping profile defaults.
- Listing type defaults.
- Condition defaults.
- SKU/mapping memory for reconciliation.
- Whatnot sales reconciliation from CSV.

Generated CSVs should always be reviewed before upload because marketplace templates and requirements can change.

### eBay CSV export

Toploader OS includes an eBay Seller Hub-style CSV exporter for selected single-card inventory rows.

The exporter supports:

- UK/US marketplace settings.
- Category ID configuration.
- Title and description templates.
- Item-specific fields.
- Public image URLs.
- Condition settings.
- Business policy fields.
- CSV validation before export.

Generated eBay CSV files should be checked against your own eBay Seller Hub template before upload.

### Show Builder and live tools

Toploader OS includes workflow tools for preparing and managing seller events, including:

- Show inventory planning.
- Selected item export prep.
- Bundle and break tools.
- Surprise set calculations.
- Pack break calculations.
- Slot pricing helpers.
- Live sale logging and analytics integration.

### Update checks

Toploader OS checks the public GitHub Releases feed for newer versions. When an update is available, the app can open the GitHub release page so the user can download the latest build.

The app does not silently replace itself. Users should download the new release, close Toploader OS, and replace/update the app files manually.

---

## Updating without losing your licence

Users do **not** need to deactivate their licence before updating.

Recommended update process:

```text
1. Close Toploader OS.
2. Download the latest ZIP from GitHub Releases.
3. Extract the new version.
4. Replace the old app files or run the new version.
5. Open Toploader OS again.
```

Normal updates validate the existing Lemon Squeezy device activation. They should not consume another activation unless the user deletes local licence data, moves to a new computer, reinstalls Windows, or manually activates again on another device.

For portable users, extract the new ZIP over the existing Toploader OS folder or back up/copy the existing data folder before deleting anything.

---

## Data storage

Toploader OS stores most data locally on the user’s machine.

Local data may include:

- Inventory profiles.
- Inventory items.
- Sales records.
- Shows.
- Export history.
- App settings.
- Local images.
- Backups.
- Generated CSVs.
- Licence state.
- Optional analytics consent state.

Packaged non-portable builds store user data in the operating system’s per-user app-data folder.

Portable mode can be enabled by placing this file next to the executable before first launch:

```text
portable.flag
```

or by launching with:

```text
TOPLOADER_PORTABLE=1
```

---

## Privacy

Toploader OS is designed so inventory and sales data stay local unless the user deliberately exports, uploads, backs up, or shares them.

The app may contact third-party services for specific features:

- Lemon Squeezy for licence activation, validation, and deactivation.
- GitHub for public update checks and release downloads.
- Scryfall for card lookup, metadata, images, and prices.
- Exchange-rate services for currency conversion support.
- Optional owner analytics infrastructure if anonymous analytics are enabled by the user.

The release bundle includes:

```text
PRIVACY_POLICY.txt
EULA.txt
THIRD_PARTY_NOTICES.txt
QT_LGPL_SOURCE_OFFER.txt
THIRD_PARTY_LICENSE_REPORT.txt
LICENSES/
```

---

## Third-party services and attribution

Toploader OS uses and/or interacts with several third-party services and libraries.

Important notes:

- Card data and images are provided via Scryfall.
- Magic: The Gathering, card names, card images, mana symbols, and related marks are owned by Wizards of the Coast LLC and/or their respective rights holders.
- Marketplace exports are helper files only. Users are responsible for checking generated CSVs before uploading them to Whatnot, eBay, or any other service.
- Toploader OS uses PySide6/Qt for the desktop interface. The Windows release includes third-party licence notices and Qt/PySide6 LGPL source-offer information.
- Toploader OS uses Lucide icons under the ISC licence.

See the bundled legal and third-party notice files for details.

---

## Licence and legal terms

Toploader OS is distributed subject to the included EULA and third-party notices.

The app itself is licensed, not sold. Third-party components remain governed by their own licences.

Nothing in the Toploader OS EULA removes rights users may have under applicable open-source licences for bundled third-party components.

---

## Support and feedback

For support, feedback, bug reports, release issues, or licence questions:

- Use the official GitHub Issues page for public bug reports and release issues.
- Join the official Toploader OS Discord: https://discord.gg/EyYMvq6eSA
- Use the official Lemon Squeezy store/customer flow for purchase and licence-related order issues.

When reporting a bug, include:

```text
Toploader OS version
Windows version
What you were doing
What happened
What you expected
Screenshots if useful
Whether you are using normal or portable mode
```

Do not post licence keys, private inventory files, customer details, or marketplace account data publicly.

---

## Special thanks

Special thanks to:

- MikeTheMagicMan
- ThePackDaddies

Thank you for helping test Toploader OS and shape the release workflow.
