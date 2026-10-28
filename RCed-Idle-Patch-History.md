# RCed Idle — Patch History

Complete recorded release history through **0.25.0**, updated on **28 October 2026**. Earlier entries describe the features and balance at that time; later updates may replace those rules. Historical verification dates are retained, while these GitHub archive entries were added on 27 October 2026.

[Download the latest game](https://github.com/iRCed7/rced-idle-releases/releases/latest) · [Main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)

**About 0.11.0:** no separately verified release artifact is recorded. Its staged Warrior, drop and interface work was combined into 0.12.0, which was verified as an update from 0.10.0. That work is covered in the 0.12.0 notes below.

## Release index

| Version | Main update |
| --- | --- |
| [0.25.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.25.0) | Platform movement, monster encyclopedia and loot filters |
| [0.24.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.24.0) | Animated opening, compact Hunt and inventory improvements |
| [0.23.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.23.0) | Attack potions, regional music and faster forecasts |
| [0.22.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.22.0) | Hair colors and Classic item controls |
| [0.21.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.21.0) | Expanded NX catalog and shared storage |
| [0.20.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.20.0) | Special shop and boss rewards |
| [0.19.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.19.0) | Magicians, progression bosses and NX |
| [0.18.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.18.0) | Thief, Assassin and Bandit |
| [0.17.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.17.0) | Live minimap, scroll shop and Journey |
| [0.16.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.16.0) | Classic navigation and per-skill attack rules |
| [0.15.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.15.0) | Keep grinding with full bags |
| [0.14.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.14.0) | Faster planning, reset coupons and Victoria quests |
| [0.13.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.13.0) | Inventory tools and stronger armor choices |
| [0.12.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.12.0) | Warriors, crafting and progression |
| [0.10.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.10.0) | Classic interface and character slots |
| [0.9.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.9.0) | Hunter, faster inventory and clearer quest tracking |
| [0.8.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.8.0) | Three characters, shared storage and Classic quests |
| [0.7.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.7.0) | Classic windows, activity quests and routes |
| [0.6.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.6.0) | Character styling, farming tools and alerts |
| [0.5.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.5.0) | Level estimates and equipment comparisons |
| [0.4.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.4.0) | Focused battles and scrolling history |
| [0.3.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.3.0) | Armor progression and supply planning |
| [0.2.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.2.0) | Full Crossbowman skill book and source artwork |
| [0.1.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.1.0) | First playable adventure |

---

## RCed Idle 0.25.0 — Platform movement, monster encyclopedia and loot filters

Released 28 October 2026. App version **0.25.0**, content version **1.21.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **Settings** before updating.
2. Download the attached APK and open it on your Android phone. Allow installation from your browser or file app if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** The application ID and signing certificate are unchanged.
4. Choose **Settings → Review content update → Back up & upgrade** separately for each existing character to activate content 1.21. Pending progress settles under the old rules, a recovery backup is created, and grinding pauses before migration. New characters start on 1.21.0.

Characters on content 1.20 or earlier retain their original simulation until upgraded. App interface improvements arrive with installation.

### Movement and targeting on content 1.21

- Travel now uses Speed, map distance and connections between platforms. Characters walk into attack range and pay the time needed to traverse a connection.
- Finish a valid focused target, then favor the nearest eligible monster on the current platform. New attacks cannot hit monsters through a different platform.
- Multi-target thresholds use each skill's actual range and eligible local targets. If no route can satisfy the configured attack policy, the chosen basic fallback is honored or grinding pauses with an explanation.
- Mage Teleport can shorten a same-platform walk at its normal MP cost; it cannot bypass cross-platform connections.
- The minimap follows saved movement and freezes while paused. Controlled comparisons start at each map's own entrance.
- Once damage already kills in one hit, more damage cannot remove spawn cooldowns or travel time. Tests confirmed identical kills when already-lethal damage was increased tenfold.

Platforms and connections are RCed approximations based on the bundled spawn coordinates. They do not reproduce every original collision foothold, rope or monster movement.

### Loot and restocking

- Ordinary **equipment and HP/MP restoration item drop chances are reduced by 50%** on content 1.21. Restoration drops contain **one item**.
- Boss tables and challenge rewards, global NX, scrolls, materials and arrows retain their previous chances.
- Restocking matters more. Some costly skill rotations can still lose net mesos on some maps; compare supply costs when choosing a route.
- Universal cosmetic drops remain **1 in 60,000 kills** across the existing pool; hairstyle coupons remain **1 in 120,000**. There is no global pity timer. First-clear guaranteed NX and six-hour boss victory cooldowns are unchanged.

### Monster encyclopedia

Browse all **45 registered monsters** and inspect their drop sources, including ordinary drops, global rewards, accepted-quest items, Steal, boss rewards and first-clear rewards. Open the current map's drop book from Hunt or browse Monsters in Settings. Lists load lazily and opening the book does not simulate grinding.

### Inventory and interface

- Advanced Auto-sell combines equipment-level, usable-job and equipment-category filters. Conditions within a rule must all match; any matching rule can select an eligible drop.
- Auto-sell retains the claimed level-40 unlock and affects **future loot only**. Existing inventory and protected target, wishlist, quest, NX, equipped, locked and scrolled items retain their protections.
- Stack sales have an **All** quantity shortcut and explicit confirmation.
- Hunt uses compact Start/Pause controls, places Home beside Maps and removes the duplicate Restock strip. Armor progression moves to Settings; redundant buttons beneath the equipment grid are removed.
- **Hungry Ronnie**, available at level 32, brings the active Classic quest list to **16**. Existing quest records are preserved.

### Verification and saved progress

**1,230 automated Flutter tests and 38 content/source checks passed**, with clean analysis. In-place installation and save preservation passed. A subsequent emulator graphics correction allowed the unchanged APK to pass two normal cold launches and native opening, Hunt, monster-book, Inventory and Settings checks. All 27 checked gameplay groups, profile, shared storage and nine retained backups were preserved.

The initial launch failure was isolated to the test emulator's software graphics setup; correcting that setup required no game-code or APK change. These checks do not establish physical-phone performance or compatibility with every device.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)
- [Grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) — its original tables describe content 1.19; the new compatibility note explains 1.21 movement and loot changes.

Feature and history snapshots are attached as Markdown files. Check GitHub manually for future updates.

---

## RCed Idle 0.24.0 — Animated opening, compact Hunt and inventory improvements

Released 28 October 2026. App version **0.24.0**, content version **1.20.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **HUD menu → Settings** before updating.
2. Download the attached APK and open it on your Android phone. Allow installation from your browser or file app if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** The application ID and signing certificate are unchanged.
4. Choose **Review content update → Back up & upgrade** separately for each existing character to enable content 1.20. Pending time settles under the old rules and a safety backup is kept. New characters start on 1.20.0; older characters keep their pinned rules until upgraded.

The opening, music and interface improvements arrive with the app update. Installing the APK alone does not change a character's content pack.

### Welcome to Victoria Island

- An animated opening uses the game's illustrated artwork and an **Enter Victoria Island** button.
- Classic login music accompanies the opening, then hands off to the current map's regional track after entry. The login track and ten regional tracks are bundled for offline play.

### More room for the hunt

- A compact Hunt layout brings the character, live minimap, map/details shortcuts and potion quickslots into the map area, with portrait and landscape layouts.
- Potion controls show their actual icons and owned counts, with quick access to supply setup.
- Hide individual tracked quests without abandoning them or losing progress or rewards. Tracking visibility is saved per character.
- Combat presentation distinguishes actual attacks from periodic damage and retaliation. Combat formulas, reward rules and random outcomes are unchanged.

### Inventory improvements on content 1.20

- Bow and crossbow arrows now stack to **5,000**. Throwing stars remain at 1,000; ammunition consumption, prices and drop quantities are unchanged.
- All six Special shop items now use the **NX pocket**: Full AP Reset, Full SP Reset, Hairstyle Coupon, Hair Color Coupon, Random NX Box and the two-hour 2× EXP coupon. Buying still does not activate an item.
- Existing quantities are preserved when upgrading. The NX pocket remains **200 slots**; existing overflow is retained, but cannot grow while over capacity.
- Ordinary zero-value items can be manually batch sold or selected for future Auto-sell, yielding **0 mesos**. Manual batches remove exactly the selected quantities and validate the whole selection before applying it.
- Equipped and locked equipment remains protected from manual sale; scrolled gear requires confirmation. Wishlist, farming-target and quest protections apply to automatic sales, while intentional manual sales remain available.
- Auto-sell still requires the claimed level-40 milestone and explicit item selection. It affects only future drops, never carried inventory, and retains its protections for NX/Special items, targets, wishlist items, quest materials and equipped, locked or scrolled gear.

### Combat bonuses and saved progress

The strongest positive skill bonus and strongest potion bonus still add per stat. Multiple bonuses within either group do not add together; permanent equipment and passive bonuses remain separate, and skill drawbacks still apply.

Regression checks and startup/music checks passed. Installing over 0.23.0 and restoring through the normal import flow preserved all 27 checked account values, shared storage and existing backups. Older content remains available until you opt in to the upgrade.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)
- [Grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) — the 0.23 combat formulas remain applicable; see these notes for the new inventory rules.

The feature guide and patch history are also attached as downloadable Markdown files. Check GitHub manually for future updates.

---

## RCed Idle 0.23.0 — Attack potions, regional music and faster forecasts

Released 28 October 2026. App version **0.23.0**, content version **1.19.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **HUD menu → Settings** before updating.
2. Download the APK attached to this release and open it on your Android phone. Allow your browser or file app to install it if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** The application ID and signing certificate are unchanged.
4. Existing characters retain their saved content rules. Choose **Review content update → Back up & upgrade** separately for each character to enable content 1.19, including timed attack potions and the weapon-shop restriction. Pending time settles under the old rules and a safety backup is kept. New characters start on content 1.19.0.

The forecast, Hunt interface and music improvements arrive with the app update. Installing the APK alone does not change a character's content pack.

### Timed attack potions

On content 1.19, two shop potions offer a ten-minute bonus:

| Potion | Effect | Duration | Shop price |
| --- | --- | --- | ---: |
| Warrior Potion | +10 Attack Power | 10 minutes | 500 mesos |
| Magic Potion | +10 Magic Attack | 10 minutes | 500 mesos |

**Attack Power is distinct from Weapon Attack.** The benefit depends on your attack and build; neither potion promises a fixed EXP increase.

- Use an owned potion from its item popup, or enable that character's optional automatic reuse. Automatic reuse consumes an owned copy at the next combat action when its effect is inactive; it does not buy stock.
- Both different potion types can be active together. An already-active copy cannot be consumed again to stack strength or extend its duration.
- Timers continue while grinding offline and while paused. Paused time does not consume replacements. Disabling automatic reuse keeps the remaining paid duration but prevents renewal.
- Empty optional potion stock does not stop grinding. Supply planning reports shortages, and forecasts include consumed potions' replacement costs. Drinking an already-purchased potion does not charge mesos again.

### Skill and potion bonuses work together

For each stat, the **strongest positive skill bonus and the strongest potion bonus add together**. Multiple skill bonuses to the same stat do not add together, and neither do multiple potion bonuses to that stat. Permanent gear and passive bonuses remain separate; skill drawbacks still apply.

For example, rank-20 Meditation gives +25 Magic Attack and Magic Potion adds +10. Rank-30 Rage gives +40 Attack Power and Warrior Potion adds +10, while Rage keeps its defense drawback. These are RCed's content 1.19 rules; older pinned content retains its previous behavior.

### Find higher-level weapons through play

The weapon shop now sells weapons requiring **level 30 or below** on content 1.19. The 55 weapons above that limit retain their existing monster-drop routes. Owned weapons, rolls, scrolling, stats, sale values and existing crafting recipes are preserved. Non-weapon equipment stock is unchanged.

### More responsive comparisons and maps

- Equipment, shop, skill, Ability Point and scroll comparisons reuse a shared controlled baseline. Immediate stat differences remain visible while the first hourly estimate finishes, and completed estimates are available when reopened.
- World Map prepares accessible primary routes in the background after relevant build changes, beginning with the current Hunt map. Closing and reopening the map keeps completed results and ongoing work.
- Unlocking a boss route adds its estimates without discarding the existing rates for that build. Earlier Routes calculates retired alternatives when requested.
- A failed forecast shows an error and can be retried. Ordinary stock changes do not restart controlled map comparisons; finite supply plans still use the quantities you actually own.

Controlled comparisons use consistent conditions, ample supplies and reset temporary effects. They help compare builds; live sessions can differ with stock, remaining buff time, accuracy, travel and other conditions.

### Compact Hunt controls

Hunt groups **Start grinding, Home and Restock** in rounded controls below the map, with complete labels and accessible touch targets at narrow widths and larger text sizes. Attack-potion controls show the available choices without consuming a potion merely by opening them, and guard against duplicate commands.

### Regional background music

**Ten locally bundled tracks cover all 38 maps**, with regional and biome assignments chosen for RCed. Settings provides a music toggle and volume slider, initially set to 30% volume. Moving within the same music region keeps the track playing without restarting it.

Music stops when the app leaves the foreground, loses audio focus or headphones disconnect. Returning to the foreground starts the assigned track again. Playback uses local files and needs no streaming or internet connection. This release adds background music; attack and monster sound effects are not included.

### Progress and verification

Existing character artwork, cosmetic rewards and saved progress are preserved. The completed verification covers **1,057 unique Flutter cases** across the full sweep and affected-file reruns: the sweep's two obsolete expectations were corrected, and the final affected run passed all 81 cases, including three added checks. This total is combined coverage, not a new all-green full-suite run.

Android update, comparison and music lifecycle checks passed on the QA emulator. Normal full-account restoration matched all 27 checked gameplay groups, profile and shared storage. Current-content potion behavior was covered by automated engine and interface tests while native checks retained the account's older pinned rules. Desktop forecast measurements and emulator playback checks do not establish physical-phone frame rates or audible speaker quality.

The game remains fully offline. Check GitHub manually for future updates.

### Game guides and release history

- [Read the main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Read the grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) for combat formulas, 35 variable groups and all 94 skills
- [Read the complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

The main game features and patch history are also attached below as downloadable Markdown assets. The grinding reference is a readable guide in the repository.

---

## RCed Idle 0.22.0 — Hair colors and Classic item controls

Released 28 October 2026. App version **0.22.0**, content version **1.18.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **HUD menu → Settings** before updating.
2. Download the APK attached to this release and open it on your Android phone. Allow your browser or file app to install it if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** The application ID and signing certificate are unchanged.
4. Existing characters retain their saved content rules. Choose **Review content update → Back up & upgrade** separately for each character to enable content 1.18 and the new style/color coupon rules. Pending time settles under the old rules and a safety backup is kept. New characters start on content 1.18.0.

### Separate hairstyles and hair colors

**Shop → Special** now offers two distinct choices:

| Item | Price | What it does |
| --- | ---: | --- |
| Hairstyle Coupon | 1,000,000 mesos | Unlocks a new hairstyle while keeping your current hair color |
| Hair Color Coupon | 500,000 mesos | Changes the color of your currently worn hairstyle |

- Saved hairstyles appear once in Styling. The catalog contains **190 source styles with 1,496 exact variants**, plus the two existing starter styles, Zeta and Unkempt Hair: **192 displayed style groups** in total.
- Switching to an owned style keeps your current color when that style has a matching variant. A style without that color is clearly unavailable; the game does not silently substitute another color.
- A color coupon is consumed only after a valid confirmation and saves the resulting exact variant for that character. Already-saved colors remain free to select on their matching currently worn style; the current color or an already-saved color cannot consume another coupon.
- Style and color ownership remain per character. This does not unlock one color globally across every hairstyle or every character.
- Your existing saved variants and worn appearance are retained. Upgrading does not recolor your character, consume a coupon or reroll a pending boss reward.

The source hairstyles have their original palettes, including styles available only in Black. Color matching respects actual artwork colors, including White/Silver and nonstandard Brown/Purple palettes.

### Clearer Styling previews

Browse named hairstyles with **Back/Next arrows**. Use **Hide worn equipment** to see the hairstyle on the bare-character preview. This toggle is only a preview: it does not unequip real gear. Previewing a style or color does not spend a coupon or change the save; closing without saving keeps your original appearance.

Characters still pinned to content 1.17 retain its exact-variant coupon rules and access to their previously saved hair until they accept the content upgrade.

### Classic item details and equipment actions

- Equipment, consumable and storage details use compact **Classic navy tooltips**, with item icons, requirements, stat lines and the relevant actions.
- Open an item's **Auto-sell** control directly from its tooltip to select that item's future monster drops. Claim the **level-40 milestone** to unlock it. Items already in Inventory or storage are kept, and farming targets, wishlisted items, active quest materials, NX items and equipped, locked or scrolled gear retain their protections. The control also explains locked, paused or protected rules.
- Unmet level, job, stat and availability requirements are shown clearly. Equip attempts provide rejection feedback without changing the save when an item is ineligible.
- Permanent bonuses from gear that will remain equipped now count toward equipment requirements. For example, 27 base STR plus a retained hat giving +3 STR can meet a 30 STR weapon requirement.
- An item's own bonuses, gear it replaces or displaces, temporary buffs and NX appearance items do not help qualify it. Comparisons and armor guidance use the same eligibility checks.
- Worn real equipment exposes **Unequip** and **Compare**. Unequip returns the exact item to the Equip bag, keeping its rolls, scroll results, remaining slots, history and lock. It needs a free Equip slot; if the bag is full, nothing moves and the game explains how to make room.

The Special items receive five source icons: Full AP Reset, Full SP Reset, Random NX Box, the two-hour EXP coupon and the new Hair Color Coupon.

### Shared storage presentation

Shared Storage uses square item cells, type tabs and the matching class, type, category, search and sorting controls. Open an item directly from its grid to inspect the Classic tooltip. Existing storage capacity and transfer rules are retained.

### Progress and verification

The cosmetic equipment catalog, character artwork, global cosmetic and hairstyle-coupon chances, boss rewards and NX Box pool are unchanged. The new color coupon is a shop addition; this release does not introduce a new color-coupon drop rate.

The completed release verified **1,009 unique Flutter cases** through the full sweep and affected-file reruns. Android update and full-account restoration checks preserved character progress, profile and shared storage. Native checks covered the updated UI without committing transactions; the new coupon behavior, upgrade preservation and Unequip actions were covered by engine, widget and SQLite tests. No physical-phone performance claim is made.

The game remains fully offline. Check GitHub manually for future updates.

### Game guide and release history

- [Read the main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Read the complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Both documents are also attached below as downloadable Markdown assets.

---

## RCed Idle 0.21.0 — Expanded NX catalog and shared storage

Released 27 October 2026. App version **0.21.0**, content version **1.17.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **HUD menu → Settings** before updating.
2. Download the APK attached to this release and open it on your Android phone. Allow your browser or file app to install it if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** The application ID and signing certificate are unchanged.
4. Storage improvements and the startup logo apply immediately. To enable the expanded cosmetic rewards, choose **Review content update → Back up & upgrade** independently for each existing character. Pending time settles under the old rules, and a safety backup is kept. New characters start on content 1.17.0.

### Expanded cosmetics and hairstyles

The reward catalog grows from eight cosmetics to **2,090 appearance-only equipment items and weapon covers**. It includes hats, face and eye accessories, earrings, tops, overalls, bottoms, gloves, shields, shoes, capes and **247 compatible weapon covers**.

- Universal monster drops, Random NX Boxes, guaranteed first-clear boss cosmetics and repeat-clear rare boss cosmetics all draw from the expanded eligible catalog.
- NX Boxes select uniformly from the 2,090 appearances. Duplicates remain possible; previews can be searched before opening a box.
- Hair coupons offer **190 base hairstyles across 1,496 color variants**. A coupon permanently unlocks the selected variant for that character's Styling collection.
- Cosmetic equipment changes appearance while normal gear retains its combat stats. Weapon covers use their supported weapon types and source poses; incompatible or intentionally empty source poses can hide the cover.
- Outfit artwork loads as needed, with bounded caches. Source-layer fixes include completed Red Boxing Gloves and Teddy Bear coverage.

This imports the supported physical cash equipment and hairstyles from the game's **GMS95 artwork source**. It does not include every cosmetic from every MapleStory version. **Rings, chat bubbles and partner effects are excluded.** Seven gun/knuckle-only covers remain reserved until a compatible Pirate class exists. The NX inventory pocket remains **200 slots**.

### Drop chances and boss rewards

Each defeated monster has a **1-in-60,000 cosmetic chance** and a **1-in-120,000 hair-coupon chance**. These are alternative outcomes of one global roll, not guaranteed rewards after a fixed number of kills. Enlarging the catalog does not increase the total drop chance, and Steal does not add global cosmetic rolls.

Bosses also use their separate guaranteed and rare reward rules. **Six-hour boss cooldowns, ordinary equipment drops, EXP, mesos, combat formulas and Special shop prices are unchanged.** Pending boss rewards keep their original results through the catalog upgrade. Ordinary global drops that cannot fit are skipped under the existing full-bag policy; they do not become pending boss rewards.

### Shared storage improvements

- Shared storage starts at **100 slots** and automatically gains **six slots for every ten-level milestone from 10 through 70 reached by each character**. Three level-70 characters provide **226 slots**.
- Existing levels count retroactively. Storage bonuses do not require claiming inventory milestones or upgrading a character's content pack. Mesos use no item slots.
- Send one item or selected stack directly from Inventory to storage, or transfer a multi-selection together. Selecting one stack transfers only that stack's quantity.
- A batch moves the complete selection together. If capacity or eligibility checks fail, none of its items move.
- Storage has matching search, class, type, category and sorting controls. Transfer processing preserves existing forecasts and keeps browsing available.
- Existing overflow remains stored and withdrawable. Gear keeps its rolls, scroll results, history and locks; equipped combat items and the last copy of an equipped NX appearance remain protected.

Storage responsiveness was improved and checked with batch-transfer workloads and Android interactions. These checks do not establish a specific frame rate or input latency on every phone.

### Startup and saved progress

The **Lupin logo now appears during both Android and in-game startup**. Existing characters bypass character creation and retain their progress. The save format is unchanged, and Android update, transfer, cosmetic-use and full-account restoration checks completed successfully.

The game remains fully offline. Check GitHub manually for future releases; this update does not add an automatic update checker.

### Game guide and release history

- [Read the main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Read the complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Both documents are also attached below as downloadable Markdown assets.

---

## RCed Idle 0.20.0 — Special shop and boss rewards

Released 27 October 2026. App version **0.20.0**, content version **1.16.0**. Requires **Android 8.0 or later**.

### Install or update

1. If you already play, export a complete account backup from **HUD menu → Settings** before updating.
2. Download the APK attached to this release and open it on your Android phone. Allow your browser or file app to install it if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first.** This release keeps the same app identity and signing certificate so an update preserves your local data.
4. Existing characters keep their current content rules. To enable the new Special shop and boss rewards, choose **Review content update → Back up & upgrade** for each character. The upgrade settles pending time under the old rules and creates a safety backup. New characters start on content 1.16.0.

### New Special shop

Open **Shop → Special** to buy:

| Item | Price |
| --- | ---: |
| Full AP Reset Coupon | 300,000 mesos |
| Full SP Reset Coupon | 300,000 mesos |
| Classic Hair Coupon | 1,000,000 mesos |
| Random NX Box | 500,000 mesos |
| 2× EXP Coupon, two hours | 2,000,000 mesos |

Purchases go into your inventory; activate them when ready. Hair coupons permanently unlock a chosen hairstyle for that character. NX boxes contain one of the eight current cosmetics with equal odds; duplicates are possible. Cosmetics change appearance without changing combat stats.

EXP coupons begin counting down when activated, including while paused or offline. Extra coupons extend the duration at the same 2× multiplier. They do not increase mesos or item drop chances.

### Boss rewards and cooldowns

- Each boss now has a **six-hour cooldown after a victory**, tracked independently for every boss and character. Losses and retreats remain retryable. Cooldowns pass while paused or offline.
- The first clear of each boss grants **one guaranteed random NX cosmetic**. Characters with earlier clears receive that entitlement once when upgrading their content.
- Every victory grants the EXP and mesos below, plus **one ordinary equipment item**. Equipment can belong to any of the four class families.
- Each victory also has independent chances for a functional 60% upgrade scroll (**25%**), an NX cosmetic (**1%**) and a two-hour 2× EXP coupon (**0.5%**).
- If a boss reward cannot fit in your inventory, it remains saved for later claiming. Claiming delivers the original result without rerolling it.

| Boss | Base EXP | Mesos |
| --- | ---: | ---: |
| Mano | 18,000 | 30,000 |
| Stumpy | 32,000 | 70,000 |
| Mushmom | 52,000 | 150,000 |
| Shade | 78,000 | 160,000 |
| Zombie Mushmom | 87,000 | 170,000 |
| Jr. Balrog | 110,000 | 180,000 |

An active EXP coupon doubles the listed EXP. Boss difficulty, normal-field combat and ordinary drop rates are unchanged.

### Navigation improvements

- **Armor** now sits beside Journey in the HUD menu, starts with **My class** selected, and includes class, type and search controls.
- The former armor-guide shortcut in Inventory now opens **Auto-sell** directly. Character's equipment page still provides access to the armor guide.

The game remains fully offline. This release includes eight NX cosmetics and six coupon hairstyles.

---

## RCed Idle 0.19.0 — Magicians, progression bosses and NX

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 27 October 2026 · Content 1.15.0.

Magician, F/P Wizard, I/L Wizard and Cleric completed the four launch families through second job. The game reached 15 jobs including Beginner, 94 skills and ten second-job branches, with wand/staff progression, Mage equipment and layered casting artwork. Third jobs and Pirate remained deferred.

- Added six repeatable progression bosses: Mano, Stumpy, Mushmom, Shade, Zombie Mushmom and Jr. Balrog. First clears award permanent cosmetic crests; the first five unlock further regions, while Jr. Balrog is the level-70 capstone. Previously accessible maps stay unlocked.
- Expanded exploration with seven new normal maps. The world presents 21 main routes, 11 retained earlier routes and six boss arenas.
- Added rare global appearance-only NX cosmetics and hair coupons, a separate 200-slot NX pocket, an independent wardrobe and permanent per-character hairstyle collections. The initial library held eight cosmetics and six coupon hairstyles.
- Added 145 ordinary equipment items to progression shop stock through level 70, keeping their clean stats, requirements and existing monster drops.
- Added a Lupin app icon, compact controls, consistent filters and persistent AP/SP attention dots, alongside browsing and forecast improvements.

EXP-coupon support extends a fixed 2× timer rather than multiplying it further. Boss-specific rare rewards and coupon durations were not assigned in this release; the stronger boss reward policy arrived in 0.20.0.

Existing characters required **Review content update → Back up & upgrade** to enable content 1.15. Install the latest APK over the existing app without uninstalling. Settings retains complete-account backup export.

---

## RCed Idle 0.18.0 — Thief, Assassin and Bandit

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 27 October 2026 · Content 1.14.0.

The Thief family joined the playable roster, advancing from Thief into Assassin or Bandit. All 18 first- and second-job skills were included, covering dagger attacks, claw throwing, recovery passives, Drain, Steal, Haste and their related mechanics. Both branches retain the Thief skill book; third jobs remained outside this release.

- Added dagger and claw equipment progression through level 70, 122 new item definitions, usable scroll rules for both weapon families and 11 throwing-star types.
- Added clearly documented RCed farming routes for progression items missing from the playable source drop catalog, without a global map or economy rebalance.
- Introduced rechargeable throwing stars. Attacks spend owned charges; recharging restores spent charges for the appropriate meso fee and cannot create a star type the character never owned.
- Exposed star selection and recharge through Hunt's supply setup and Restock planner. Shared storage transfers available charges without duplicating spent ones.
- First Thief advancement offers a starting dagger or claw, recovery supplies and 500 Subi charges.

Weapon, ammunition and character-art lookups were optimized to reduce repeated work. Actual costs still depend on skills and hunting routes: high-cost choices can exhaust supplies or reduce net income.

Existing characters retained their earlier content until **Review content update → Back up & upgrade**. Upgrade the relevant character to 1.14 to access Thief content. Install current APK updates over the existing app without uninstalling, and use Settings for complete-account backups.

---

## RCed Idle 0.17.0 — Live minimap, scroll shop and Journey

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 27 October 2026 · Content 1.13.0.

Inventory, shopping and exploration received clearer controls and more useful information.

- Moved inventory selection into a compact checklist control beside search. Equip, Use and Etc now share consistent grid and footer layouts while retaining their separate capacities and individual stack selection.
- Added independent class, type and sorting choices for Weapons and Equips. Shop lists reuse their catalog and build visible rows on demand.
- Expanded the shop to all 37 registered Lesser/100% scrolls. At this release, 29 had usable effects and eight were clearly marked collectibles with unsupported effects.
- Added source-based spawn and respawn markers across all 25 minimaps, plus a moving player marker that illustrates the encounter route. The display does not create extra monsters or rewards.
- Separated Journal and Journey. Journal groups discoveries by type and starts with categories collapsed. Journey records level-ups, job advancements and claimed milestones.

New Journey events record their dates and maps, including events earned during offline progress. Older events without reliable dates or locations are shown as unknown rather than reconstructed. The HUD menu consistently opens Settings.

Interface improvements applied to older saves immediately. Expanded scroll stock and dated Journey recording required the backed-up upgrade to content 1.13. Existing inventory, history and shared storage were preserved in Android update checks.

Install the latest APK over the existing app; do not uninstall first. Settings provides complete-account backup export.

---

## RCed Idle 0.16.0 — Classic navigation and per-skill attack rules

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 27 October 2026 · Content 1.12.0.

A compact Classic navigation dock brought rounded buttons, readable labels, static icons and attention dots together. Forest, rock, cave, industrial and other terrain treatments gave all 25 maps suitable foreground platforms. The scenery changes were visual; they did not change route geometry or rewards.

- Set a minimum living-monster count from 1 to 6 for each learned attack, alongside an explicit fallback. The highest eligible threshold determines the attack.
- Use the same saved attack rules across real combat, forecasts, equipment comparisons and supply planning. Existing two-skill policies remain intact until edited and saved.
- Focus the Classic quest board on 15 substantive hunts and collections. Conversation-only errands, level-only NPC stages and deliveries made entirely from NPC-provided items were retired.
- Keep completed quest history and already-owned items. Continuing quest chains bypass retired steps without handing out their unearned rewards.
- Retain daily and weekly hunting tasks, level milestones, inventory expansions, crafting unlocks and reset coupons. Time-only and meso-only recurring tasks were retired.

Navigation and terrain appeared immediately after installation. Quest changes and the expanded skill editor required an explicit backed-up upgrade to content 1.12 for each character. Old elapsed time was settled under the character's prior rules first.

Use the latest release for installation, install over the existing app, and do not uninstall first. Full-account backup export remains available in Settings.

---

## RCed Idle 0.15.0 — Keep grinding with full bags

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 27 October 2026 · Content 1.11.0.

Full bags no longer stop EXP and meso gains under the new content rules. Grinding keeps existing items, fills any usable partial stacks, and skips only newly generated item quantities that cannot fit. Eligible automatic sales still work, and away summaries distinguish skipped items from loot actually received.

- Added nine hunting routes, bringing the catalog to 25 maps. New choices include additional Ant Tunnel, Burnt Land, excavation and tomb routes for different monsters and farming goals.
- Revised Transfer Area travel timing while retaining its saved monsters and encounters. The patch did not change monster EXP rewards, meso rewards or item-drop probabilities.
- Replaced the World Map's large controls with compact cards showing scenery, monsters and rates. Tap an unlocked card to travel back to Hunt.
- Search maps by name or monster, filter by the actual monster species, and open smaller detail or layout controls as needed.
- Added a direct Restock control on Hunt with selectable session duration.

Notification checks, inactive-character saving and battle rendering were adjusted to reduce repeated work. These changes were checked in automated and Android emulator flows; no specific physical-phone frame rate was promised.

Interface improvements applied immediately. Existing characters needed **Review content update → Back up & upgrade** to enable the full-bag behavior and new routes, while earlier pinned rules remained available.

Install the latest APK over the existing app and do not uninstall first. Export a full account backup from Settings if desired.

---

## RCed Idle 0.14.0 — Faster planning, reset coupons and Victoria quests

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 26 October 2026 · Content 1.10.0.

Supply and session planning were reworked to reuse recent rates instead of repeatedly simulating long sessions. Hunt samples its current map, other forecasts run when requested, and supply lists update from current stock. Purchase reviews preserve the quantities you selected and explain when a basket cannot fit. Session estimates still assume an unchanged build and restocking; actual grinding continues to enforce supplies and capacity.

- Level 30, 50 and 70 milestones each grant one Full AP Reset Coupon and one Full SP Reset Coupon. Previously claimed eligible milestones receive their added coupons once after upgrading.
- AP resets refund invested stats; SP resets refund ranks to the appropriate job books. Resets preserve level and job, pause grinding for review, and retain equipment that becomes ineligible.
- All non-equipment items use stacks of 1,000. Existing quantities and equipment instances remain intact.
- Expanded the playable Classic quest catalog to 37 stages: 34 Victoria stages and three Maple Island stages. Quest-only items drop for accepted matching objectives and stop at the carried quota.
- Inventory excludes worn gear from its carried-equipment list. Crafting and comparison views expose useful item stats earlier.

Existing characters kept their saved rules until the backed-up content upgrade to 1.10. New reset handling preserved learned ranks and exact point totals during migration.

For a current installation, use the latest release and install over the existing app. Do not uninstall first; Settings can export a complete account backup.

---

## RCed Idle 0.13.0 — Inventory tools and stronger armor choices

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 26 October 2026 · Content 1.9.0.

Inventory management and character-building actions became easier to use, while repeated work behind stat calculations was reduced.

- Equipment inventory groups items by slot and item type.
- Batch selling lets you review selected equipment and individual stack quantities before confirming one sale. Item protections and changed selections are checked before the sale completes.
- Allocate AP or SP in a chosen quantity while retaining the familiar +1 controls. Skill books show the jobs the character has actually attained.
- Search and filter farming targets and crafting recipes by class or type. Conditional attack choices use stacked rows for easier reading.
- Battle presentation stays visible while actions are saved, and large carried-equipment collections no longer require the same repeated full-save work during stat reads.

Content 1.9 revised physical defense so armor upgrades have a stronger effect. Benefits depend on character level and equipment; undergeared characters can take more damage, and heavy armor still has diminishing returns. Map rewards, EXP, mesos ranges and drop probabilities were not changed by this patch.

Existing characters retained earlier rules until **Review content update → Back up & upgrade**. Installation and restoration checks preserved character progress and shared storage. The performance evidence measured reduced computation, not a promised frame rate on every phone.

Use the latest release for installation, install over the existing app, and do not uninstall first. Settings offers complete-account export for backups.

---

## RCed Idle 0.12.0 — Warriors, crafting and progression

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 26 October 2026 · Content 1.8.0.

This release combined the staged Warrior and interface expansion with new crafting and inventory progression.

- Added Warrior advancement into Fighter, Page or Spearman, with 30 Warrior skills and eight weapon families. Expanded the equipment and monster-drop catalog; unsupported gear and effects were clearly marked as collectibles.
- Added 54 workshop recipes, including refining all 15 registered raw ores. Claiming the level-10 milestone unlocks crafting. Four refined materials did not yet have a further equipment recipe.
- Introduced Equip, Use and Etc capacity progression. Every ten levels through 100 offers a one-time claim of six additional slots in each tab. Existing inventories are retained when upgrading.
- Added optional automatic selling at the level-40 milestone. It applies to selected future monster drops, with protected items excluded; switching it on does not sell carried inventory.
- Increased ordinary HP/MP recovery-item stacks to 1,000 and added conditional attacks based on the living monster count.

Rounded, raised Classic controls, boxed level digits and metallic HP/MP/EXP gauges refreshed Hunt. Session estimates explain supply or capacity limits, and the battle can display six actual monsters.

Existing characters kept their earlier rules until **Review content update → Back up & upgrade**. At this release, overflowing inventory still paused grinding; continued grinding with full bags arrived later. Install current updates over the existing app without uninstalling, and export a full account backup from Settings when needed.

---

## RCed Idle 0.10.0 — Classic interface and character slots

**Archival patch notes only. No APK is provided for this historical release. [Get the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

Historical build verified on 26 October 2026 · Content 1.6.0.

The interface received a Classic Maple-inspired redesign adapted for phone screens. Inventory uses a cream grid, windows have silver-blue borders, selected tabs are pink, and the bottom status strip brings HP, MP and EXP together. Skills, quests, equipment and character stats received matching layouts while retaining their existing actions.

- Tap the character name to open Stats and the avatar to open the character roster.
- Open the minimap from Hunt. In landscape, Hunt places its controls and quest helper beside the map.
- Unlock a new second character when the first character reaches level 30. Unlock a new third character when any character reaches level 70. Already-created characters remain playable, even below these requirements.
- Pending offline progress is considered before checking whether another character slot is available.

This was an interface and roster-access update: combat rules, drop rates, content assets and balance were unchanged from 0.9.0. Existing characters kept their saved content without needing a content upgrade. Android update checks preserved character progress and shared storage, including accounts with previously created low-level characters.

For current downloads, install the latest APK over the existing app; do not uninstall first. A complete account backup can be exported from Settings.

---

## RCed Idle 0.9.0 — Hunter, faster inventory and clearer quest tracking

App **0.9.0+9** · Content **1.6.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Added the Hunter second-job branch alongside Crossbowman, with all six Hunter skills and their rank requirements.
- Added ten bows, four bow scrolls, acquisition sources, worn-equipment sprites and separate bow ammunition.
- Added an explicit War Bow or Crossbow choice at first advancement and a Hunter or Crossbowman choice at second advancement. Existing Crossbowmen kept their class.
- Implemented bow timing, mastery, buffs, Final Attack and Arrow Bomb within the idle combat model.
- Rebuilt inventory as a grid that creates visible slots as needed, with cached searches and ordering for large collections.
- Organized quests into Available, In progress and Completed, with Classic, Daily and Weekly filters.
- Added a Hunt tracker for two prioritized quests and kept ready rewards marked with a red dot until claimed.
- Saved equipment attention separately for each character. Viewing the equipment pocket acknowledges the items actually observed, while later loot can trigger a new dot.

Existing characters retained earlier content until individually choosing a backed-up upgrade to 1.6.0. Bow arrows and crossbow arrows remained distinct; existing stacks were not converted. The Hunter release expanded the Bowman family only—Warrior, Thief and Magician gameplay arrived later. Inventory improvements were verified with large collections, without claiming a physical-phone frame-rate benchmark.

---

## RCed Idle 0.8.0 — Three characters, shared storage and Classic quests

App **0.8.0+8** · Content **1.5.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Added up to three characters with independent progress, supplies and grinding clocks. Switching characters does not pause the others.
- Added shared storage for mesos, stackable items and unequipped gear, preserving equipment rolls, scrolling history and locks during transfers.
- Added whole-account export and restoration for the roster and shared storage.
- Added eight Classic NPC quests with named kills or carried-material objectives, explicit acceptance, prerequisites and one-time turn-ins.
- Corrected missing and misplaced material drops, including Orange Mushroom Cap, Squishy Liquid and Slime Bubble, and expanded the catalog to 124 items.
- Increased monster mesos by 40% and selectively raised exceptionally rare equipment sources to 0.025%. Reduced arrow drops to an 8% chance for 1–5 arrows.
- Made item, skill and scroll comparisons use five controlled 20-minute paired samples, reducing changes caused by the current battle or temporary supply shortages.
- Added income estimates after matching supply drops, alongside the conservative replacement cost of all consumed shop supplies.
- Refined Classic-style windows with blue edges, cream panels, rectangular tabs and square hotbar keys.

Existing characters kept their pinned rules until individually upgraded with a safety backup. Drop, balance and Classic quest changes belonged to content 1.5.0. The quest set was still a small subset, and other class families were not yet playable.

---

## RCed Idle 0.7.0 — Classic windows, activity quests and routes

App **0.7.0+7** · Content **1.4.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Reworked the interface around five main destinations and a persistent player HUD, with compact windows adapted for touch.
- Added an equipment-slot presentation and separate Equips, Skills and Stats views for the character.
- Organized the shop into Consumables, Equips, Weapons and Scrolls, with item details and comparison controls.
- Added six daily/weekly activity quests with level-scaled goals and rewards, explicit claims and visible UTC reset times.
- Added Meat for 160 HP and Lemon for 150 MP as higher-capacity recovery choices in shops and supply setup.
- Added arrow drops to all 25 monsters under content 1.4: a 30% chance for 5–15 arrows. These are historical values from this version.
- Introduced map-specific horizontal and climbing routes, with travel costs influenced by movement speed and range.
- Prevented contact damage during modeled travel between encounter groups and improved compact map-rate and next-level panels.

Interface improvements worked with existing content packs immediately. New quests, provisions, arrow drops and route rules required an explicit backed-up upgrade to content 1.4.0. These quests were idle activity objectives; the sourced Classic NPC quest set arrived in a later update. Unclaimed repeating rewards expired at their reset.

---

## RCed Idle 0.6.0 — Character styling, farming tools and alerts

App **0.6.0+6** · Content **1.3.0**, unchanged · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Added character creation with a name, three skins, three hairstyles and three faces: 27 bundled male appearance combinations.
- Allowed repeatable appearance changes and a separate one-time rename. Existing characters kept their progress and bypassed new-character creation.
- Added layered character and equipment artwork, attack poses, normal/critical/MISS digits and platform tiles. Worn gear changes the rendered outfit.
- Added farming-target map rankings with expected drops per hour, eligible kills and a clearly labeled first-drop probability estimate.
- Highlighted actual farm-target finds and rare drops without changing their odds or adding a pity system.
- Added shop equipment previews using a hypothetical clean item, plus skill previews comparing the current and next rank without purchasing gear or spending SP.
- Added six independent optional alerts: level-ups, farm targets, rare drops, supply stops, being downed and readiness to advance.
- Kept alerts off by default. Local background checks inspect elapsed time without awarding rewards or changing the gameplay save.

The update required no rules migration. Android may delay the approximate 15-minute alert checks, and force-stopping the app prevents alerts until it is reopened. All artwork and gameplay remained bundled for offline use; this was not yet the later NX cosmetic system.

---

## RCed Idle 0.5.0 — Level estimates and equipment comparisons

App **0.5.0+5** · Content **1.3.0**, unchanged · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Added exact EXP remaining to the next level and an estimated amount of active grinding time at the current map's forecast rate.
- Handled level caps, unavailable rates, supply stops and pending job advancement in the estimate instead of presenting misleading completion times.
- Refreshed forecasts when the character's level, build, map or save changes, while keeping ordinary progress updates responsive.
- Added full current-versus-proposed equipment comparisons for damage, hit chance, estimated casts per kill, EXP, kills, supply use and gross/net mesos per hour.
- Displayed derived character stats alongside gear requirements, remaining upgrade slots, scroll successes and failures, locks and base-plus-scroll stats.
- Accounted for an overall replacing both top and bottom, and explained why an ineligible item could not be used.
- Kept comparisons read-only: viewing an item neither equips it nor spends mesos, supplies, scroll slots or live randomness.
- Improved loading, error and close controls for comparisons on narrow screens and with enlarged text.

These features required no content upgrade or save migration. The engine and content packs stayed unchanged. Time estimates assumed the same build and map, excluded paused time and could change when supplies or player choices changed.

---

## RCed Idle 0.4.0 — Focused battles and scrolling history

App **0.4.0+4** · Content **1.3.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Changed targeting to finish the current living monster before switching. After a kill, the character prefers another injured monster over a fresh spawn.
- Added battle presentation driven by actual saved attacks: damage and misses, critical hits, target HP, hit reactions, defeats and earned drop icons.
- Improved damage-number readability by replacing the previous number on rapid hits to the same target and separating simultaneous drop icons.
- Added scrolling reveals for success, intact failure and destruction, with before/after stats, consumed slots, Skip and Continue controls.
- Introduced a scrolling ledger with attempt totals, successes, consumed scrolls, successful stat gains and recent detailed records.
- Saved each scrolling result before showing its reveal, so reopening the app or retrying a completed action cannot reroll it or consume another scroll.
- Added equipment-level information to inventory and shop views, plus a character-name shortcut to Character.
- Distinguished measured monster mesos, session cash changes and forecast income after replacement supply costs.

Existing adventures retained their old rules until an explicit backup and upgrade. Earlier lifetime scrolling totals and item histories survived, while the new detailed ledger began at the upgrade; unavailable older records were not reconstructed. Reduced motion and returning from offline time suppress unnecessary battle replay.

---

## RCed Idle 0.3.0 — Armor progression and supply planning

App **0.3.0+3** · Content **1.2.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Expanded armor progression with 32 gear definitions and 14 scrolls, covering hats, tops, bottoms, overalls, gloves and shoes.
- Added armor guidance with equipment requirements, prices, hunting sources and slot filters. The sourced armor path reached level 70 and remained usable beyond it.
- Resolved top, bottom and overall conflicts while preserving displaced equipment, rolls and scrolling history.
- Added supply planning for sessions of up to 24 hours, including expected consumption, first shortages, fallback behavior and supplies unavailable in shops.
- Added reviewed supply baskets that validate the complete purchase before spending mesos. Planning itself does not consume supplies or advance the live adventure.
- Added a clean level-10 Crossbow and 15 Red plus 15 Blue Potions to future first-job advancement rewards. The weapon is not equipped automatically; already-advanced characters receive no retroactive grant.
- Improved inventory search, armor filters, hunting-map filters and enlarged-text layouts.
- Preserved existing gear statistics and both earlier content packs through explicit, backed-up upgrades.

New adventures started on content 1.2.0. Supply forecasts assumed an unchanged build and excluded replenishment from future loot, so their results were preparation estimates rather than guaranteed session lengths.

---

## RCed Idle 0.2.0 — Full Crossbowman skill book and source artwork

App **0.2.0+2** · Content **1.1.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

- Completed the supported Beginner, Bowman and Crossbowman skill book: 15 skills plus Basic Attack, with rank effects, prerequisites and resource costs.
- Added separate Beginner skill points, selectable attacks and automatic buff controls with ordering and skip-or-pause choices when resources are missing.
- Added saved, ordered AP/SP targets for future level-ups. Automatic allocation remains optional, and job advancement still requires a player choice.
- Expanded combat support for multi-target attacks, buffs, cooldowns, mastery, critical effects and Final Attack.
- Bundled 211 source artwork files covering monster animations, item and skill icons, 12 full map scenes and all 16 minimaps.
- Added read-only equipment and scroll-success forecasts that leave live inventory, progress and randomness unchanged.
- Improved narrow-screen skill dialogs and the scrollable update review. Paused scenes and reduced-motion mode keep animated sprites still.
- Introduced explicit, backed-up content upgrades while retaining the original 1.0.0 rules for existing adventures.

New adventures started on content 1.1.0. Existing adventures could choose **Review skill update → Back up & upgrade** after pending time settled under their old rules. Character artwork was still a placeholder, and four excavation maps retained fallback scenery.

---

## RCed Idle 0.1.0 — First playable adventure

App **0.1.0+1** · Content **1.0.0** · Verified **26 October 2026**.

**Archival patch notes only. No game binary is provided for this historical version. [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest).**

This first Android build established the offline grinding, equipment and scrolling adventure.

- Introduced real-time idle combat that continues while the app is closed, with no away-time cap. Kills award EXP, mesos and individually rolled loot.
- Added 16 training maps, 25 monsters, 31 item definitions and eight scrolls, with progression data through level 100.
- Opened the Beginner → Bowman → Crossbowman path, with explicit advancement at levels 10 and 30 and an initial subset of class skills.
- Added manual AP/SP allocation, equipment requirements, potions, arrows and supply exhaustion that stops grinding when required supplies run out.
- Introduced equipment rolls, item locks, protected selling and individual scrolling with visible success and destruction odds.
- Added map forecasts, inventory, character, shop, workshop, journal, wishlist filters and settings.
- Saved progress locally with autosave, rolling recovery checkpoints, resumable offline progress and export/import through Android's file picker.
- Bundled the game data, fonts and initial procedural artwork for connection-free first launch and play.

This historical build had a partial skill book and simplified armor coverage. Character customization, additional jobs and the later quest, crafting and boss systems were not yet included.
