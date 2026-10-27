<p align="center">
  <img src="media/rced-idle-logo.png" width="180" alt="RCed Idle game logo">
</p>

# RCed Idle

An offline idle RPG for **Android 8.0+**. Build your characters, hunt for equipment, develop your skills and progress while the game is closed.

[Latest update](#latest-update) · [Screenshots](#screenshots) · [Game features](#game-features) · [Install or update](#install-or-update) · [Patch history](RCed-Idle-Patch-History.md)

## Latest update

**0.22.0 — Hair colors and Classic item controls** · 28 October 2026

**[Download the latest APK](https://github.com/iRCed7/rced-idle-releases/releases/latest/download/RCed-Idle.apk)** · [Open the release page](https://github.com/iRCed7/rced-idle-releases/releases/latest)

- **Choose style and color separately:** the 1,000,000-meso hairstyle coupon keeps your current color; the new 500,000-meso Hair Color Coupon recolors the worn style after confirmation. Requires content 1.18.
- **Clearer Styling previews:** saved styles appear once, Back/Next arrows browse named styles, and Hide worn equipment reveals the hair without unequipping real gear.
- **Keep saved appearances:** owned colors remain free on their matching style, sparse palettes show unavailable choices, and existing hair variants are preserved.
- **Classic tooltips with Auto-sell:** inspect requirements, stats and five updated Special-item icons, then set an item's future-drop sale rule directly after claiming the level-40 milestone. Carried items and protected drops stay kept.
- **More accurate equip requirements:** permanent bonuses from retained real gear count, while an item's own bonuses, replaced gear and temporary buffs do not.
- **Unequip real gear:** return the exact item to a free Equip slot with its rolls, scrolling history and lock intact; a full bag explains what must be cleared first.
- **Square storage grids:** item cells, type tabs and matching filters make stored items easier to browse and inspect.

> **Updating?** Install over your existing app; do not uninstall first. Export a complete account backup from Settings. Existing characters enable new content through **Review content update → Back up & upgrade**.

<details>
<summary>Full patch notes for 0.22.0</summary>

Released 28 October 2026. App version **0.22.0**, content version **1.18.0**. Requires **Android 8.0 or later**.

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

</details>

## Screenshots

**0.22.0 example-character UI previews.** Select an image to view it at full size. Explore more modules beside their descriptions in [Game features](#game-features). Some panels are isolated previews; forecast numbers are illustrative.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png" width="220" alt="RCed Idle 0.22.0 Hunt screen at Snail Hunting Ground II with an example character, quest helper and Start grinding button."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png" width="220" alt="RCed Idle 0.22.0 compact classic tooltip for a Brown Pole-Feather Hat with requirements, stats and Unequip, Compare and Scroll actions."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png" width="220" alt="RCed Idle 0.22.0 Hair Color Coupon dialog with an Acorn hairstyle preview and color swatches."></a>
</p>

[Hunt](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png) · [Item details](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png) · [Hair colors](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png)

## Game features

**Published game: 0.22.0 · Content: 1.18.0 · Overview dated 28 October 2026**

### Play at your own pace

- Prepare your character, choose a map, select attacks and supplies, then start grinding.
- Earn EXP, mesos and actual item drops while the game is open or closed. Offline progress runs at the same ordinary pace, with **no away-time cap**.
- Supplies, defeat, pauses and job advancement still matter. Running out of resources can stop grinding or trigger your chosen fallback; the game does not automatically buy supplies or choose your next job.
- No online account, internet connection, advertisements or real-money purchases are required to play.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png" width="240" alt="RCed Idle 0.22.0 Hunt screen at Snail Hunting Ground II with an example character, quest helper and Start grinding button."></a>
</p>

[Hunt](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hunt.png)

### Four class families and ten second jobs

Begin as a Beginner, then develop a character through first and second job. The current catalog contains **15 jobs, including Beginner, and 94 skill definitions, including Basic Attack**.

| First job | Second-job choices |
| --- | --- |
| Warrior | Fighter, Page, Spearman |
| Bowman | Hunter, Crossbowman |
| Thief | Assassin, Bandit |
| Magician | F/P Wizard, I/L Wizard, Cleric |

Spend Ability Points and Skill Points manually, inspect each skill's requirements and effects, or save optional allocation plans for future levels. Beginner skills use their own SP pool. Job advancement always waits for your choice. Third jobs and Pirate are not included in this release.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-ability-points.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-ability-points.png" width="240" alt="RCed Idle 0.22.0 Ability Points screen showing STR, DEX, INT, LUK and Plan your next levels."></a>
</p>

[Ability Points](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-ability-points.png)

### Shape your combat strategy

- Choose a main attack and a fallback, with minimum monster-count rules for individual skills.
- Enable optional automatic buffs, set their order, and choose whether missing resources should skip a buff or pause grinding.
- Manage HP/MP recovery choices, ammunition and rechargeable throwing stars.
- Equipment, skill ranks, attack speed, range, defense, accuracy, critical hits, multi-target attacks and supported status effects affect your results.
- Preview the estimated impact of equipment, shop purchases, skill ranks and successful scroll upgrades before committing resources.

Combat is adapted for idle play. Forecasts are estimates under stated conditions; they do not award rewards or guarantee future drops.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png" width="240" alt="RCed Idle 0.22.0 beginner skill inventory with Three Snails, Nimble Feet, Recovery and Combat policy."></a>
</p>

[Skills](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png)

### Explore maps and challenge bosses

Compare training routes, view their monsters and drops, follow the live minimap, and unlock progression routes. Choose a desired farm item to help rank maps by expected yield and highlight useful finds.

Six boss encounters are available: **Mano, Stumpy, Mushmom, Shade, Zombie Mushmom and Jr. Balrog**. Victory grants EXP, mesos and equipment, with additional chances for scrolls, NX cosmetics and EXP coupons. Each boss's first clear guarantees one random NX cosmetic. Victories start a **six-hour cooldown for that boss and character**; failed attempts remain retryable. Rewards that cannot fit stay saved for later claiming.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-world-map.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-world-map.png" width="240" alt="RCed Idle 0.22.0 route cards for Mushroom Garden, Southern Forest and West Rocky Mountain, with monster art and forecast panels."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png" width="240" alt="RCed Idle 0.22.0 boss list at larger text size, showing Mano and Stumpy recommendations and rewards."></a>
</p>

[World map](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-world-map.png) · [Bosses](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png)

### Collect, improve and manage equipment

- Find individually rolled equipment, check requirements, compare stats, equip upgrades and lock items you want to keep.
- Inspect equipment, consumables and stored items in compact Classic navy tooltips with icons, requirements, stat lines and the relevant actions.
- Meet equipment requirements using base stats plus permanent bonuses from gear that stays equipped. The candidate's own bonuses, replaced or displaced gear, temporary buffs and NX appearances do not count. Unmet requirements are explained before a valid equip can occur.
- Unequip a real item into a free Equip slot while keeping its rolls, scroll results, remaining slots, history and lock. If the bag has no room, the item stays equipped and the game explains how to make space.
- Use compatible scrolls with visible success and destruction odds. View the outcome, stat changes and scrolling history.
- Browse armor progression by class, item type and search, including ordinary gear through level 70.
- Buy supplies, weapons, equipment and scrolls with mesos. Review and sell multiple inventory items together.
- Unlock **54 crafting recipes** through the level-10 milestone, including material refining and equipment crafting.
- Claim the level-40 milestone to unlock optional **Auto-sell**, then use an item's tooltip control to select its future-drop rule. It applies only to future monster drops, keeping existing inventory and storage intact. Farming targets, wishlisted items, active quest materials, NX items and equipped, locked or scrolled gear are protected; the control explains locked, paused and protected rules.

On current content, full bags do not stop EXP and mesos from ordinary hunting, but new item drops that cannot fit are skipped.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-inventory.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-inventory.png" width="240" alt="RCed Idle 0.22.0 Use inventory tab with potions, ammunition, food, search and item filters."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png" width="240" alt="RCed Idle 0.22.0 compact classic tooltip for a Brown Pole-Feather Hat with requirements, stats and Unequip, Compare and Scroll actions."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png" width="240" alt="RCed Idle 0.22.0 Workshop crafting panel with a Bronze Ingot recipe, batch sizes, ingredient requirements and Craft button."></a>
</p>

[Inventory](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-inventory.png) · [Item details](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png) · [Crafting](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png)

### Quests, milestones and the Special shop

Complete **15 active Classic quests**, plus one daily hunt and one weekly hunt. Offline kills count toward supported objectives. Follow accepted objectives on Hunt and collect rewards from the quest log.

Every ten-level milestone can be claimed for **six more slots in each ordinary inventory pocket**. Certain milestones also grant reset coupons.

The **Special shop** sells full AP/SP resets, hairstyle coupons, hair color coupons, random NX boxes and two-hour 2× EXP coupons for mesos. A Hairstyle Coupon costs **1,000,000 mesos** and unlocks a style while preserving the current color; a Hair Color Coupon costs **500,000 mesos** and changes the color of the currently worn style. These separate coupon rules require content 1.18. Items are purchased first and activated separately. Extra EXP coupons extend the duration at the same 2× multiplier; their timers continue while paused or offline.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-quests.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-quests.png" width="240" alt="RCed Idle 0.22.0 Quest Log with Classic, Daily, Weekly and Milestones tabs and Sam's Suggestion available."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png" width="240" alt="RCed Idle 0.22.0 Village Shop consumables list with stock search, item filters and Buy x10 controls."></a>
</p>

[Quests](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-quests.png) · [Shop](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png)

### Develop a three-character account

Create up to three characters with independent jobs, equipment and grinding sessions. The second slot requires the first character to reach level 30; the third requires any character to reach level 70. Other characters can keep grinding while you play a different slot.

Shared storage starts at **100 item slots**, with **six additional slots for every ten-level milestone from 10 through 70 reached by each character**. Bonuses are automatic and retroactive, independent of inventory milestone claims and each character's content pack. Three level-70 characters provide **226 shared slots**. Mesos use no item slots, and any existing overflow remains stored and withdrawable.

Send an individual item, one selected stack or a multi-selection directly from Inventory to storage. A selected stack moves only its own quantity; a batch transfers the complete selection together or leaves it unchanged if validation fails. Storage uses square item cells and type tabs, with matching search, class, type, category and sorting controls. Open items from the grid to inspect their Classic tooltips; browsing remains available during transfers.

Shared storage transfers mesos, stackable items and unequipped gear between characters. Equipment keeps its rolls, scroll results, history and locks. Equipped combat items and the last copy of an equipped NX appearance are protected. Characters on older content may need to upgrade before receiving newer items.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png" width="240" alt="RCed Idle 0.22.0 character roster with two example characters, a locked third slot and Shared storage button."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png" width="240" alt="RCed Idle 0.22.0 shared storage with compact square item slots, category tabs, Deposit and Withdraw controls and search filters."></a>
</p>

[Characters](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png) · [Shared storage](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png)

### Customize your appearance

Choose a name, skin, hairstyle and face, then watch equipped gear change your character's appearance. Styling remains available after creation, with a one-time character rename.

The current catalog includes **2,090 reward-eligible NX equipment items and weapon covers**, including **247 compatible weapon covers**, plus **190 source hairstyles across 1,496 exact color variants**. The two existing starter styles, Zeta and Unkempt Hair, bring Styling to **192 displayed style groups**. NX equipment changes appearance without replacing normal combat stats. The separate NX inventory pocket holds **200 slots**.

On content 1.18, saved hairstyles appear once in Styling. A Hairstyle Coupon unlocks a style while preserving your current color; switching to an owned style also uses that color when available. A style without the matching color is shown as unavailable rather than silently recoloring the character. Source palettes vary, and some styles only have Black.

A Hair Color Coupon changes the currently worn style after confirmation and saves the resulting exact variant for that character. Saved colors remain free to select on their matching currently worn style, and an already-saved or current color cannot consume another coupon. Color ownership does not carry across every hairstyle or character. Existing saved variants remain intact.

Use Back/Next arrows to browse named hairstyles and **Hide worn equipment** to see hair on the bare-character preview. The toggle does not unequip real items. Previews do not change saves or consume coupons; closing without saving preserves the original appearance.

The same eligible cosmetic catalog appears in rare universal drops, Random NX Boxes and boss rewards. Boxes select equally among the 2,090 appearances, and duplicates are possible. Each defeated monster has a **1-in-60,000 cosmetic chance** and a **1-in-120,000 hairstyle-coupon chance** as alternative global outcomes. Those are probabilities, not guaranteed rewards after that many kills. The Hair Color Coupon is sold in the shop; no new color-coupon drop rate is introduced in 0.22.0. Boss-specific cosmetic rewards are separate. Ordinary drops that cannot fit are skipped; pending boss rewards retain their existing protection.

The catalog covers the supported physical cash equipment and hairstyles from the **GMS95 artwork source**, rather than every cosmetic from every region or era. **Rings, chat bubbles and partner effects are excluded**, and seven Pirate-only covers remain reserved. Weapon covers follow their supported weapon types and original pose availability; incompatible or deliberately hidden poses can leave a cover invisible. Artwork loads for requested outfits instead of loading the entire wardrobe on each screen change.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png" width="240" alt="RCed Idle 0.22.0 Classic Hair Coupon preview with hairstyle carousel, search and Hide worn equipment option."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png" width="240" alt="RCed Idle 0.22.0 Hair Color Coupon dialog with an Acorn hairstyle preview and color swatches."></a>
</p>

[Hair styles](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png) · [Hair colors](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png)

### Plan, track and stay informed

Plan supplies for **1, 4, 8 or 24 hours**, review shortages and costs, and buy a selected supply basket manually. View estimated EXP, mesos, supply costs and time to the next level. Journal tracks discoveries, while Journey records progression milestones and advancements.

Optional local notifications cover level-ups, target and rare drops, supply stops, defeat and advancement. They are off by default; delivery depends on Android's background settings. Enlarged text, reduced motion and optional workshop sound support different play preferences.

### Keep your progress

Export and import a **complete account backup** from Settings, including every character and shared storage. Existing characters retain their current content rules until you choose **Review content update → Back up & upgrade**, which settles pending time under the old rules and creates a safety backup. Upgrade each character independently to content 1.18 for the separate hairstyle/color coupon rules; new characters start on 1.18. Characters pinned to 1.17 retain their earlier exact-variant hair rules and saved appearances until upgraded. Installing the APK alone does not switch a character's content pack.

Check GitHub manually for new releases. **Install updates over your existing app; do not uninstall first.** Export a backup before updating. The game does not automatically check for or download updates.

## Install or update

1. If you already play, export a complete account backup from **HUD menu → Settings**.
2. [Download the latest APK](https://github.com/iRCed7/rced-idle-releases/releases/latest/download/RCed-Idle.apk) and open it on your Android device. Allow your browser or file app to install it if Android asks.
3. **Install over your existing RCed Idle app. Do not uninstall first.** Uninstalling removes local game data.
4. Continue playing, or choose **Review content update → Back up & upgrade** for each character when you want its new content rules.

The game stays offline. Check the [Releases page](https://github.com/iRCed7/rced-idle-releases/releases) manually for updates. The permanent download link always serves the latest published game release.

## Guides and earlier releases

- [Complete patch history](RCed-Idle-Patch-History.md) — all recorded releases and their changes.
- [Standalone game features](RCed-Idle-Game-Features.md) — the feature guide as its own readable document.
- [Download the feature guide](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.22.0/RCed-Idle-Game-Features.md) or [patch history](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.22.0/RCed-Idle-Patch-History.md) as a file.
- [Browse all releases](https://github.com/iRCed7/rced-idle-releases/releases) — earlier archive entries contain patch notes only, without old game binaries. The staged 0.11.0 changes shipped in 0.12.0.

The APK's SHA-256 checksum is attached to each game release.
