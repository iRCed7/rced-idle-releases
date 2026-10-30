<p align="center">
  <img src="media/rced-idle-logo.png" width="180" alt="RCed Idle game logo">
</p>

# RCed Idle

An offline idle RPG for **Android 8.0+**. Build your characters, hunt for equipment, develop your skills and progress while the game is closed.

[Latest update](#latest-update) · [Screenshots](#screenshots) · [Game features](#game-features) · [Install or update](#install-or-update) · [Patch history](RCed-Idle-Patch-History.md)

## Latest update

**0.35.2 - Grind boss shortcut and roster layout** · 31 October 2026

**[Download the latest APK](https://github.com/iRCed7/rced-idle-releases/releases/latest/download/RCed-Idle.apk)** · [Open the release page](https://github.com/iRCed7/rced-idle-releases/releases/latest)

- Hunt is now named Grind across headings, navigation and return controls.
- Open Bosses directly with the Jr. Balrog map shortcut.
- A red dot identifies ready bosses at your recommended level or previously defeated.
- Updated character selection uses reviewed roster art and wider Character/Quest layouts.
- 122 focused tests and emulator update/restart checks passed, preserving all 56 backups.
- Install over the existing app. No content upgrade is required.

> **Updating?** Install over your existing app; do not uninstall first. Export a complete account backup from Settings. Existing characters enable new content through **Review content update → Back up & upgrade**.

<details>
<summary>Full patch notes for 0.35.2</summary>

Released 31 October 2026. App **0.35.2**, Android build **37**, content **1.30.0**. Requires Android 8.0 or later.

### Grind and boss access

The main module is now called **Grind** in its heading, navigation and return controls. A still **Jr. Balrog shortcut** beside World map and Home opens the existing Bosses tab directly, without starting a challenge.

The selected character gets a red dot when a boss is off cooldown and either:
- The character has reached its recommended level, or
- That character has defeated it before.

Character creation must be complete, HP must be positive and no other boss fight may be active. Opening Bosses does not dismiss the dot. Readiness updates with cooldown expiry, ordinary offline catch-up and character switching.

This is an alert rule, not a challenge restriction. Higher-level bosses remain accessible. Older packs without field bosses have no shortcut; older boss packs without cooldowns retain their rules. Rewards, damage, cooldowns and save formats are unchanged.

### Roster and responsive layout

Includes three reviewed tree/platform/empty-slot images, a revised character selector and wider Character/Quest content on unfolded screens. Selection and Play retain their behavior. Crowded action strips scroll horizontally while keeping 48-pixel touch targets.

Readiness checks only six boss definitions and the current character ledger. It adds no forecast, simulation, database read or private timer.

### Verification and saved progress

**122 focused tests passed**: 70 readiness, shortcut, navigation and reward checks, plus 52 roster/responsive/quest UI tests. Full lib/test analysis is clean. This is focused validation, not a full-suite run.

Package, signer and 16 KB alignment passed; all 56,670 prior asset payloads are retained, with three reviewed roster images added. Engine, persistence, Android code and game content match the previous release.

An in-place 0.35.1 to 0.35.2 synthetic emulator update kept the database unchanged before launch. Cold launch/restart preserved the account, shared storage and all **56 prior backup records**. The installed shortcut and dot were reviewed, and tapping opened Bosses without a challenge. Physical-phone frame pacing and the player's save were not inspected.

Boss Mastery Trials, Expedition Gauntlets and Profession Work Orders remain proposals and are not included.

</details>

## Screenshots

Hunt is a **0.35.0 UI test** example-character preview; Opening, Inventory and Quests retain **0.24.0** labels. Other module images in [Game features](#game-features) retain their explicit **0.23.0** or **0.22.0** capture labels. Select an image for full size; forecasts are illustrative.

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png" width="240" alt="RCed Idle 0.24.0 Victoria Island opening with illustrated artwork and Enter Victoria Island button"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.2-grind.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.2-grind.png" width="240" alt="Grind 0.35.2 with boss shortcut, synthetic widget capture"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-inventory.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-inventory.png" width="240" alt="RCed Idle 0.24.0 Use inventory with item filters, ammunition, potions and compact navigation"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png" width="240" alt="RCed Idle 0.24.0 Quest log with Classic, Daily, Weekly and Milestones tabs"></a></p>

## Game features

**Published game: 0.35.2 | Content: 1.30.0 | Overview dated 31 October 2026**

### Painted UI and reliable startup

App 0.35.1 includes coordinated blue/gold navigation, parchment panels and aligned tabs, item rows, skill/stat readings, shops, quests and workshop controls. Settings groups backup/import actions in Save management. Narrow layouts support scrolling and large text; unfolded Hunt, inventory and shop use expanded layouts. Older screenshots below retain their historical capture labels.

The database startup-lock fix retries transient BUSY/LOCKED opens and closes notification snapshot connections before simulation. Notification jobs remain read-only for gameplay progress. No save schema, gameplay rules or automatic content upgrade is introduced. Install over your existing app; no content upgrade is required for these UI/startup changes.

### Enter Victoria Island

An animated illustrated opening welcomes you with classic login music. Select **Enter Victoria Island** to continue; music switches to the current map's regional track. All eighteen music tracks are bundled for offline play.

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png" width="240" alt="RCed Idle 0.24.0 Victoria Island opening with illustrated artwork and Enter Victoria Island button"></a></p>

Opening preview — **0.24.0**.

### Play at your own pace

- Prepare your character, choose a map, select attacks and supplies, then start grinding.
- Hunt combines a compact live minimap, Home shortcut and potion icons with owned counts. Open World Map, Adventure details and Monster drops from the minimap popup. Start/Pause uses a compact blue control; supply setup remains available through potion quickslots. A warning icon lists full inventory pockets.
- Earn EXP, mesos and actual item drops while the game is open or closed. Offline progress runs at the same ordinary pace, with **no away-time cap**.
- Supplies, defeat, pauses and job advancement still matter. Running out of resources can stop grinding or trigger your chosen fallback; the game does not automatically buy supplies or choose your next job.
- No online account, internet connection, advertisements or real-money purchases are required to play.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.2-grind.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.2-grind.png" width="240" alt="Grind 0.35.2 with the Jr. Balrog boss shortcut and ready dot, synthetic character."></a>
</p>

[Grind (0.35.2)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.2-grind.png)

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
- On content 1.19, use Warrior Potion for **+10 Attack Power** or Magic Potion for **+10 Magic Attack**, each lasting **ten minutes** and costing **500 mesos**. Attack Power is distinct from Weapon Attack. Drink owned stock manually or enable optional automatic reuse for that character; there is no automatic purchase.
- The strongest positive skill bonus and strongest potion bonus add per stat. Benefits within either pool do not sum; permanent gear and passive bonuses remain separate, and skill drawbacks still apply.
- Equipment, skill ranks, attack speed, range, defense, accuracy, critical hits, multi-target attacks and supported status effects affect your results.
- Preview the estimated impact of equipment, shop purchases, skill ranks and successful scroll upgrades before committing resources.

Attack-potion timers continue while paused and offline. Paused time does not consume replacements, and disabling renewal preserves the paid remaining duration. An active copy cannot be consumed again to stack its strength or duration; the two different potion types can coexist. Empty optional potion stock does not stop grinding. Supply plans show shortages and include the replacement cost of consumed potions.

Combat is adapted for idle play. Forecasts are estimates under stated conditions; they do not award rewards or guarantee future drops. Equipment, shop, skill, AP and scroll comparisons share controlled baselines and reuse completed results when reopened. Immediate stat changes remain visible while the first hourly estimate runs. Controlled comparisons reset temporary effects and use ample supplies; live results still depend on your actual stock and conditions.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png" width="240" alt="RCed Idle 0.22.0 beginner skill inventory with Three Snails, Nimble Feet, Recovery and Combat policy."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png" width="240" alt="RCed Idle 0.23.0 attack potion controls with Warrior Potion and Magic Potion, Use now buttons and Auto-use after expiry checkboxes."></a>
</p>

[Skills](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-skills.png) · [Attack-potion controls (0.23.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png)

### Platform movement and loot on content 1.21

Speed, world distance and platform connections determine travel time. Finish a valid focused target, then choose nearby eligible monsters on the same platform. Each attack must reach its targets; multi-target thresholds count only eligible monsters in that skill's local range. When no route can satisfy a policy, the selected basic fallback applies or grinding pauses with an explanation. Mage Teleport can shorten a same-platform walk at its normal MP cost, but cannot bypass platform connections. The minimap follows movement and freezes when paused.

Spawn cooldowns, attack timing, range and travel limit throughput once damage already kills in one hit. Platforms and connections are RCed approximations based on bundled spawn coordinates, rather than verified original collision geometry.

Ordinary equipment and HP/MP restoration drop chances are **50% lower** than in content 1.20; restoration drops contain **one item**. Boss tables and challenge rewards, global NX, scrolls, materials and arrows retain their previous chances. Plan restocking and compare net mesos: some expensive skill rotations still cost more than they earn on some routes.

### Monster encyclopedia and advanced loot rules

Browse **45 registered monsters**, search and filter the catalog, and inspect ordinary, global, accepted-quest, Steal, boss and first-clear drop sources separately. Open the current-map book from the Hunt minimap popup or Monsters from Settings. Opening the catalog does not simulate grinding.

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.25.0-monster-book.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.25.0-monster-book.png" width="240" alt="RCed Idle 0.25.0 monster encyclopedia with search, filters and monster artwork"></a></p>

Monster encyclopedia — **0.25.0**, isolated synthetic preview.

Advanced Auto-sell supports multiple equipment-level, usable-job and equipment-category rules. All conditions within a rule must match; any matching rule can select an eligible future drop. The claimed level-40 unlock and existing target, wishlist, quest, NX, equipped, locked and scrolled-item protections remain. Existing carried inventory is never emptied by these rules.

### Progression economy and excavation routes

Content 1.24 retunes fixed map reward profiles for solo progression and distinct EXP, income and item-farming choices. Field mesos no longer receive a level-gap penalty; EXP decay for substantially outleveled monsters remains. Ordinary monsters attempt attacks every **2.4 seconds**, previously 1.5, reducing sustained potion pressure without changing per-hit defense, Magic Guard, source stats, skill MP costs or potion prices. Boss behavior and ordinary drop probabilities are unchanged.

Between targets, routing weighs nearby living monsters against reachable denser platforms and their real travel cost. Characters finish the current target and pending Final Attack first. Route commitment and a short clearing window reduce immediate backtracking; spawn timers and capacities are unchanged. This is a hunting heuristic, not guaranteed optimal routing.

All 70 controlled builds had a profitable tested route and distinct EXP/income winners. Some routes remain negative, and one documented Burnt Land routing case loses throughput after a damage upgrade. The policy supports generally improving progression, not guaranteed profit from every upgrade or exact Classic parity.

Excavation Sites I–III and Remains &lt;Tomb&gt; I–IV use original terrain and sky, with a matching ruins foreground platform, bundled for offline Hunt and World Map use.

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.27.0-tomb-i.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.27.0-tomb-i.png" width="480" alt="RCed Idle 0.27.0 Remains Tomb I scenery with original terrain, sky and ruins platform"></a></p>

Remains Tomb I — **0.27.0**, isolated synthetic scenery preview.

### Explore maps and challenge bosses

Explore **38 maps**, compare training routes, view their monsters and drops, follow the live minimap, and unlock progression routes. Choose a desired farm item to help rank maps by expected yield and highlight useful finds.

Accessible primary routes prepare estimates in the background after build changes, starting with the current Hunt map. Opening and closing World Map keeps ongoing work and completed results; new boss access adds routes without discarding existing rates for that build. Earlier Routes calculates retired alternatives when requested. Failed estimates can be retried, and ordinary stock changes do not restart controlled route comparisons.

Six boss encounters are available: **Mano, Stumpy, Mushmom, Shade, Zombie Mushmom and Jr. Balrog**. Victory grants fixed EXP/mesos and, on content 1.23, one uniformly selected weapon: Mano level 25–30, Stumpy 30–40, Mushmom 40–50, Shade 50–60, Zombie Mushmom 60–70 and Jr. Balrog level 70. The separate 25% scroll roll uses weapon attack, glove attack and glove magic attack scrolls; rare NX and EXP-coupon bonuses remain. Selection is not job-weighted. Previously earned armor and other pending rewards remain claimable. Each boss's first clear guarantees one random NX cosmetic. Victories start a **six-hour cooldown for that boss and character**; failed attempts remain retryable. Rewards that cannot fit stay saved for later claiming.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-world-map.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-world-map.png" width="240" alt="RCed Idle 0.23.0 route cards for Mushroom Garden, Southern Forest and West Rocky Mountain with monster art and illustrative forecast values."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png" width="240" alt="RCed Idle 0.22.0 boss list at larger text size, showing Mano and Stumpy recommendations and rewards."></a>
</p>

[World map (0.23.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-world-map.png) · [Bosses](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-bosses.png)

### Collect, improve and manage equipment

- Find individually rolled equipment, check requirements, compare stats, equip upgrades and lock items you want to keep.
- Inspect equipment, consumables and stored items in compact Classic navy tooltips with icons, requirements, stat lines and the relevant actions.
- Meet equipment requirements using base stats plus permanent bonuses from gear that stays equipped. The candidate's own bonuses, replaced or displaced gear, temporary buffs and NX appearances do not count. Unmet requirements are explained before a valid equip can occur.
- Unequip a real item into a free Equip slot while keeping its rolls, scroll results, remaining slots, history and lock. If the bag has no room, the item stays equipped and the game explains how to make space.
- Use compatible scrolls with visible success and destruction odds. View the outcome, stat changes and scrolling history.
- Browse armor progression from Settings by class, item type and search, including ordinary gear through level 70.
- Buy supplies, equipment and scrolls with mesos. On content 1.19, shop weapons require **level 30 or below**; all 55 higher-level weapons retain monster-drop routes, existing crafting recipes and their owned copies, stats, upgrades and sale values. Content 1.25 adds a separate Crafting shop tab with 18 supply entries, including materials and base armor. Review and sell multiple inventory items together. Stack sales offer an **All** shortcut and explicit confirmation.
- Claim the level-10 milestone to unlock **279 recipes** across six professions on content 1.25; choose two permanent specializations per character. Earlier pinned packs retain their original crafting rules.
- Claim the level-40 milestone to unlock optional **Auto-sell**, then use an item's tooltip control to select its future-drop rule. It applies only to future monster drops, keeping existing inventory and storage intact. Farming targets, wishlisted items, active quest materials, NX items and equipped, locked or scrolled gear are protected; the control explains locked, paused and protected rules.

On content 1.20 or later, bow and crossbow arrows stack to **5,000**; throwing stars remain at 1,000. Ordinary zero-value items can be batch sold or selected for future Auto-sell for **0 mesos**. Manual sales remove the selected quantities together; equipped and locked gear is protected and scrolled gear requires confirmation. Automatic target, wishlist and quest protections do not prevent intentional manual sales.

On current content, full bags do not stop EXP and mesos from ordinary hunting, but new item drops that cannot fit are skipped.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-inventory.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-inventory.png" width="240" alt="Painted inventory with parchment cells, synthetic 0.35.0 UI test capture."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png" width="240" alt="RCed Idle 0.22.0 compact classic tooltip for a Brown Pole-Feather Hat with requirements, stats and Unequip, Compare and Scroll actions."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-crafting.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-crafting.png" width="240" alt="Painted crafting journal, synthetic 0.35.0 UI test capture."></a>
</p>

[Inventory](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-inventory.png) · [Item details](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png) · [Crafting journal (0.35.0 UI test capture)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.35.0-ui-test-crafting.png)

### Professions and timed crafting

Choose two permanent specializations per character from **Smithing, Weaponcrafting, Tailoring, Woodcrafting, Leatherworking and Arcforge**. Claim the level-10 milestone first. Each profession advances through ranks 1–8; character-level gates apply. Historical recorded crafts grant matching mastery when you learn the discipline, without duplicating items.

Browse **279 recipes** in a Classic journal with profession tabs, mastery, output stats and required-material grids. Click a craftable ingredient to follow its recipe and return to the parent. Phones use focused details; wide screens show two columns. Run one queue per character. Enter a quantity, use MAX or Craft All, up to 10,000 executions. New jobs on content 1.26 take 250 ms per craft; already reserved jobs retain their saved duration. Crafting continues while resting, hunting and offline. Materials and fees are reserved up front; cancelling refunds only unfinished work. Finished output waits safely if your bag is full. Equipment-input recipes require exact-item confirmation and protect equipped, locked, scrolled, wishlisted and targeted gear.

Use shared storage to exchange supplies and output between characters. Some recipes need another specialization's materials. Ranks 9–10, housing, advanced-arrow and Fame recipes, optional catalysts and kits remain deferred. Parties are not enabled.

### Quests, milestones and the Special shop

Complete **16 active Classic quests**, including Hungry Ronnie at level 32, plus one daily hunt and one weekly hunt. Offline kills count toward supported objectives. Follow accepted objectives on Hunt and collect rewards from the quest log. Hide individual tracked quests without abandoning them or changing progress; visibility is saved per character.

Every ten-level milestone can be claimed for **six more slots in each ordinary inventory pocket**. Certain milestones also grant reset coupons.

The **Special shop** sells full AP/SP resets, hairstyle coupons, hair color coupons, random NX boxes and two-hour 2× EXP coupons for mesos. A Hairstyle Coupon costs **1,000,000 mesos** and unlocks a style while preserving the current color; a Hair Color Coupon costs **500,000 mesos** and changes the color of the currently worn style. Content 1.26 uses random unowned style/color unlocks; earlier packs retain their targeted rules. Items are purchased first and activated separately. On content 1.20 or later, all six Special shop items share the **200-slot NX pocket**. Existing quantities are preserved on upgrade; overflow is retained, but transactions cannot increase occupied slots while over capacity. Extra EXP coupons extend the duration at the same 2× multiplier; their timers continue while paused or offline.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png" width="240" alt="RCed Idle 0.24.0 Quest Log with Classic, Daily, Weekly and Milestones tabs and Sam's Suggestion available."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png" width="240" alt="RCed Idle 0.22.0 Village Shop consumables list with stock search, item filters and Buy x10 controls."></a>
</p>

[Quests](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png) · [Shop](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shop.png)

### Develop a three-character account

Create up to three characters with independent jobs, equipment and grinding sessions. The second slot requires the first character to reach level 30; the third requires any character to reach level 70. Other characters can keep grinding while you play a different slot.

Shared storage starts at **100 item slots**, with **six additional slots for every ten-level milestone from 10 through 70 reached by each character**. Bonuses are automatic and retroactive, independent of inventory milestone claims and each character's content pack. Three level-70 characters provide **226 shared slots**. Mesos use no item slots, and any existing overflow remains stored and withdrawable.

Send an individual item, one selected stack or a multi-selection directly from Inventory to storage. A selected stack moves only its own quantity; a batch transfers the complete selection together or leaves it unchanged if validation fails. Storage uses square item cells and type tabs, with matching search, class, type, category and sorting controls. Open items from the grid to inspect their Classic tooltips; browsing remains available during transfers.

Shared storage transfers mesos, stackable items and unequipped gear between characters. Equipment keeps its rolls, scroll results, history and locks. Equipped combat items and the last copy of an equipped NX appearance are protected. Characters on older content may need to upgrade before receiving newer items.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.30.0-characters.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.30.0-characters.png" width="240" alt="RCed Idle 0.30.0 synthetic character selector with Classic treehouse and bridge artwork."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png" width="240" alt="RCed Idle 0.22.0 shared storage with compact square item slots, category tabs, Deposit and Withdraw controls and search filters."></a>
</p>

[Characters](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.30.0-characters.png) · [Shared storage](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png)

### Customize your appearance

Choose a name, skin, hairstyle and face, then watch equipped gear change your character's appearance. Styling remains available after creation, with a one-time character rename.

The current catalog includes **2,090 reward-eligible NX equipment items and weapon covers**, including **247 compatible weapon covers**, plus **190 source hairstyles across 1,496 exact color variants**. The two existing starter styles, Zeta and Unkempt Hair, bring Styling to **192 displayed style groups**. NX equipment changes appearance without replacing normal combat stats. The separate NX inventory pocket holds **200 slots**.

On content 1.26, hairstyle coupons randomly unlock an unowned style while any remain, retaining the current color where supported. Color coupons randomly unlock a missing color of the currently worn style while any remain. When all eligible options are owned, the dialog explains that another owned look may be selected. Acquired styles and exact colors remain free to reapply. Hair randomness has its own saved stream and does not advance combat or loot randomness. Earlier pinned packs keep targeted coupon behavior. Owned appearances and coupons are preserved.

Use Back/Next arrows to browse named hairstyles and **Hide worn equipment** to see hair on the bare-character preview. The toggle does not unequip real items. Previews do not change saves or consume coupons; closing without saving preserves the original appearance.

The same eligible cosmetic catalog appears in rare universal drops, Random NX Boxes and boss rewards. Boxes select equally among the 2,090 appearances, and duplicates are possible. On content 1.22, each defeated monster has a **1-in-4,000 cosmetic chance** and a **1-in-120,000 hairstyle-coupon chance** as alternative global outcomes. The same 2,090 appearances are equally likely, so a particular cosmetic has a 1-in-8,360,000 chance per kill. Earlier pinned packs retain their old rate. These are probabilities, not guaranteed rewards after that many kills; there is no pity timer. The Hair Color Coupon is sold in the shop; it has no added global drop chance. Boss-specific cosmetic rewards are separate. Ordinary drops that cannot fit are skipped; pending boss rewards retain their existing protection.

The catalog covers the supported physical cash equipment and hairstyles from the **GMS95 artwork source**, rather than every cosmetic from every region or era. **Rings, chat bubbles and partner effects are excluded**, and seven Pirate-only covers remain reserved. Weapon covers follow their supported weapon types and original pose availability; incompatible or deliberately hidden poses can leave a cover invisible. Artwork loads for requested outfits instead of loading the entire wardrobe on each screen change.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png" width="240" alt="RCed Idle 0.22.0 Classic Hair Coupon preview with hairstyle carousel, search and Hide worn equipment option."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png" width="240" alt="RCed Idle 0.22.0 Hair Color Coupon dialog with an Acorn hairstyle preview and color swatches."></a>
</p>

[Hair styles](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png) · [Hair colors](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png)

### Follow combat and review rewards

Each recorded hit displays its own damage, critical or miss appearance in order. If an early hit kills a target, no unrolled number is invented. On content 1.22 or later, incoming strikes show actual HP loss after mitigation using original purple hit artwork and separate **MP −N** losses for Magic Guard. Misses and guarded attacks are distinguished. Reduced motion and offline/resume handling suppress transient effects; combat formulas and rewards are unchanged.

Offline reports show only retained item quantities and count auto-sale mesos once. Opening a report grants nothing again. Boss-report dismissal persists per character without deleting the encounter details, clear records, first-clear rewards or pending loot from the Bosses page. A later encounter creates a fresh report.

### Plan, track and stay informed

Hunt displays **NET MESO /h**, matching World Map's supply-adjusted estimate: coins plus configured auto-sales, minus the cost of consumed supplies still missing after matching retained drops. Negative values use a warning color. It does not assume all equipment or other loot is sold; Adventure details retain gross income and supply breakdowns. Stocked estimates are not wallet-change measurements or a guarantee that carried supplies last an hour.

Plan supplies for **1, 4, 8 or 24 hours**, review shortages and costs, and buy a selected supply basket manually. View estimated EXP, mesos, supply costs and time to the next level. Journal tracks discoveries, while Journey records progression milestones and advancements.

The [grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) explains combat formulas, **35 variable groups and all 94 skills**, including their conditions and how they affect training. Damage thresholds, accuracy, overkill, travel and supply costs mean an item or skill point does not have one universal EXP percentage.

Optional local notifications cover level-ups, target and rare drops, supply stops, defeat and advancement. They are off by default; delivery depends on Android's background settings. Enlarged text, reduced motion and optional workshop sound support different play preferences.

**Eighteen locally bundled music tracks include the login theme and explicit assignments for all 38 maps.** Thirty-one ordinary maps use audited source assignments; Drake's Meal Table uses the requested Sleepy Wood override. Five custom boss arenas inherit their background-map music, while Jr. Balrog retains its dedicated theme. Settings provides a toggle and volume slider, initially at 30% volume. Same-region travel does not restart the track. Playback stops when the app leaves the foreground, loses audio focus or headphones disconnect; foreground return starts the assigned track again. Music is offline, and changing its settings does not change character progress. Combat sounds have an independent Settings toggle and volume slider. The offline trial includes 45 monster hit reactions and four crossbow recordings; Double Shot and Final Attack: Crossbow reuse the basic crossbow clip. Other weapon-family attack sounds are outside the trial. Sounds follow live events without replaying an offline/resume backlog; some historical rotations remain silent.

### Classic touch controls and safer movement

Touch keycaps below Hunt configure attacks, buffs and supplies; HP/MP shortcuts open the matching recovery selection. Per-skill monster thresholds appear on the attack strip. Grind/Rest shares a compact row with EXP, net mesos and next-level timing. AP/SP allocation has one-point arrows and a larger plan. Shops default to the active character's class; inventory displays unlocked cells and hides the worn NX copy while keeping extras.

The Classic character selector previews outfits on a treehouse and bridge, with a parchment stat card; preview selection does not switch the active character until confirmed. Content 1.26 fixes a paused-climb upgrade/resume exception, commits platform trips and clears the monsters present on arrival before choosing another detour. Spawn limits and monster rewards are unchanged. Solo balance remains under review; parties remain disabled.

### Archer balance and shared skill behavior

On content 1.27, Hunter and Crossbowman Final Attack adds bonus hits without extra time or supplies, using a 25% trigger chance and 55% of the captured rank damage multiplier. It only hits surviving reachable enemies and cannot chain itself. On content 1.29, Warrior Final Attack also becomes a free bonus hit, with its own policy described below. Allocated SP and the player toggle remain.

Power Knockback pushes eligible nearby enemies within their platform, suppressing contact attacks only while they are beyond contact reach; spells remain possible. Attack rules skip cooling-down choices. Debuffs consider range, immunity and existing coverage, independent slow effects retain their expiry, and automatic recovery avoids spending a cooldown at full resources. Focus and Nimble Feet check whether they help the current situation.

Routing considers productive clusters reachable on the current platform before detouring elsewhere. Rewards, drop tables, spawns and shop prices are unchanged. Controlled tests do not establish universal profitability: some mage rotations and heavily invested archer builds remain costly. The Thief pass adds the optional tactics described below; the Warrior pass follows below; The Mage pass follows below; parties remain deferred.

### Thief tactics and defensive choices

Content 1.28 adds optional learned Drain, Disorder and Steal tactics in Attack rules. New tactics start off; existing rotations remain. Drain activates below a chosen HP threshold and heals from actual damage, with a six-second cooldown. Set its threshold above the potion threshold if you want a chance to heal before potions. Disorder and Steal make one opening attempt per monster life, remembered through save/reload. Steal grants at most one eligible ordinary item, no EXP/mesos or global NX, and cannot steal boss loot.

Dark Sight ends when an attack is paid for and grants a three-second guard for the next landed contact hit; enemy magic remains unprotected. Automatic use checks nearby durable threats and has a cast-time cost. Haste shortens existing jump links by up to 10% without changing climbs, falls or attack speed. Claw Mastery improves Lucky Seven's minimum-roll floor toward 65% without increasing its maximum.

Utilities may trade EXP for survival, income or loot. Controlled builds do not prove every setup profitable or all classes balanced. The Mage pass follows below; parties remain deferred.

### Warrior damage, defense and positioning

On content 1.29, six Warrior Final Attacks add a free follow-up after a landed Power Strike or Slash Blast, with a 25% chance and 40% of the captured multiplier. Fighter hits up to three surviving targets; Page and Spearman focus one. Spearman retains bounded actual-damage lifesteal. These follow-ups cost no extra action or supplies and cannot chain themselves.

Threaten uses a six-second recast cooldown, reduced cost/time and percentage-or-flat weapon-defense reduction. Automatic casting checks eligible durable threats instead of wasting a cast on short or empty fights. Rush physically dashes on the current foothold and pushes eligible survivors within bounded distances. It retains HP/MP costs, cooldown and incoming-damage exposure.

Other defense and recovery values remain; usefulness depends on threats, supplies and build. Controlled results do not prove universal map profitability. The Mage pass follows below; parties remain deferred.

Startup loads only current content and historical versions needed by saved characters, with large JSON decoding away from the UI thread and temporary validation packs released afterward. All historical packs remain bundled for old saves and backups. The corrected startup avoids the memory exhaustion found in the withheld initial candidate.

### Mage recovery, control and supply choices

Content 1.30 makes Improved MP Recovery scale from 1% to 2% of maximum MP per ten seconds, gives Magic Claw up to 18% direct damage by rank, and halves Teleport's source MP cost before solo tuning. Teleport requires at least 150 ms saved over same-platform walking.

Slow uses a six-second recast cooldown and half source MP/time, skipping unsuitable automatic targets. Burn and poison retain independent bounded schedules and previously paid effects survive migration.

Cleric can enable **Heal below HP %** in Attack rules; it defaults off and keeps the normal damage rotation. Bless discounts Heal MP by its source healing bonus. Holy Arrow deals 70% of its earlier direct damage on ordinary fields; boss damage and Heal's undead damage remain unchanged. This is not a fixed percentage EXP change.

Earlier class policies, maps, rewards and drops are retained. Controlled comparisons do not establish universal class parity. Parties remain deferred.

### Grind boss shortcut and roster

The main module is named **Grind**. Its Jr. Balrog shortcut opens Bosses directly; the red dot shows an off-cooldown boss at the character's recommended level or already defeated by that character. Creation must be complete, HP positive and no boss encounter active. Opening the page does not clear the dot. Higher-level bosses remain accessible; rewards and challenge rules are unchanged.

The 0.35.2 roster uses revised tree/platform/empty-slot artwork and a responsive selector. Character and Quest content expands on unfolded displays. Existing selection and Play actions remain. This app/UI update needs no content upgrade.

### Keep your progress

Export and import a **complete account backup** from Settings, including every character and shared storage. Existing characters retain their current content rules until you choose **Review content update → Back up & upgrade**, which settles pending time under the old rules and creates a safety backup. Upgrade each character independently to **content 1.30** for Mage recovery, damage, control and supply changes alongside the earlier Warrior, Thief and Archer changes; new characters start on 1.30. Packs through 1.29 retain their original simulation until upgraded. Earlier pinned content keeps its own rules, including the exact-variant hair behavior on 1.17. Installing the APK alone does not switch a character's content pack. The animated opening, Hunt interface and music arrive with the app update.

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
- [Grinding reference](RCed-Idle-Grinding-Reference.md) — how stats, skills, supplies and hourly estimates work.
- [Download the feature guide](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.35.2/RCed-Idle-Game-Features.md) or [patch history](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.35.2/RCed-Idle-Patch-History.md) as a file.
- [Browse all releases](https://github.com/iRCed7/rced-idle-releases/releases) — earlier archive entries contain patch notes only, without old game binaries. The staged 0.11.0 changes shipped in 0.12.0.

The APK's SHA-256 checksum is attached to each game release.
