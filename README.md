<p align="center">
  <img src="media/rced-idle-logo.png" width="180" alt="RCed Idle game logo">
</p>

# RCed Idle

An offline idle RPG for **Android 8.0+**. Build your characters, hunt for equipment, develop your skills and progress while the game is closed.

[Latest update](#latest-update) · [Screenshots](#screenshots) · [Game features](#game-features) · [Install or update](#install-or-update) · [Patch history](RCed-Idle-Patch-History.md)

## Latest update

**0.27.0 — Field rates, platform routes and boss loot** · 28 October 2026

**[Download the latest APK](https://github.com/iRCed7/rced-idle-releases/releases/latest/download/RCed-Idle.apk)** · [Open the release page](https://github.com/iRCed7/rced-idle-releases/releases/latest)

- **Revised field rates:** lower EXP multipliers on level-10+ maps and reduced field mesos bonuses; balance remains provisional.
- **Platform routing:** nearby monster groups are weighed against actual travel time, with less immediate backtracking.
- **Boss loot:** guaranteed weapons in boss-specific level bands and attack-focused scroll pools; NX/coupon bonuses remain.
- **Purple incoming-hit numbers:** original damage, MISS and GUARD artwork, with separate Magic Guard MP loss.
- **Excavation scenery:** original terrain and sky for Excavation Sites I–III and Remains Tomb I–IV.
- Install over the existing app, then choose **Back up & upgrade** per character for content 1.23.

> **Updating?** Install over your existing app; do not uninstall first. Export a complete account backup from Settings. Existing characters enable new content through **Review content update → Back up & upgrade**.

<details>
<summary>Full patch notes for 0.27.0</summary>

Released 28 October 2026. App version **0.27.0**, content version **1.23.0**. Requires **Android 8.0 or later**.

### Revised field EXP and mesos

- Ordinary maps recommended for level 10 or above retain **5/11 of their previous EXP multiplier**, except **Remains &lt;Tomb&gt; I**, which retains **65%** because its revised routing already reduces throughput. Earlier starter routes retain their EXP profiles.
- For field mesos multipliers above 1, half the bonus above 1 remains: for example, **1.6 becomes 1.3**. Multipliers at or below 1 are unchanged.
- These are fixed map reward settings. Monster base rewards, potion prices, consumption rules, ordinary drop chances, equipment stats and skill damage formulas are unchanged. Boss purses are separate from field profiles.

**Balance remains provisional.** The Tomb I calibration brings tested EXP rates closer to the reported Classic reference, but it is not an exact recreation of every build. Coin income and potion consumption still need joint tuning; some tested rotations remain loss-making. Do not treat gross mesos as net profit or expect a guaranteed hourly rate.

### Routes that consider nearby monster groups

Between targets, characters weigh nearby living monsters against reachable, denser platforms, including real walking and connection time. They finish their current target and pending Final Attack first.

Routes remain committed across intermediate platforms, with a short clearing window on arrival to reduce immediate backtracking. Attack range, same-platform restrictions, Speed and paid Teleport still apply. Spawn capacities and respawn timers are unchanged. This is a hunting heuristic, not a guaranteed maximum-EXP route.

### Boss weapons and attack scrolls

Future boss victories guarantee one uniformly selected real weapon from the following required-level bands; armor is removed from that equipment roll:

| Boss | Weapon requirement levels |
| --- | --- |
| Mano | 25–30 |
| Stumpy | 30–40 |
| Mushmom | 40–50 |
| Shade | 50–60 |
| Zombie Mushmom | 60–70 |
| Jr. Balrog | 70 |

The separate **25% scroll roll** now uses weapon-attack, glove-attack and glove-magic-attack scrolls. Defensive and stat-only scrolls are removed. Existing 60% attack scrolls are included; the catalog's glove-magic option is the 100% Lesser scroll. Weapon selection is not tailored to your job, and not every family has an item in each band.

The six-hour cooldown, fixed boss EXP/mesos, guaranteed first-clear NX and established rare NX/EXP-coupon bonuses remain. Previously earned armor, scrolls and pending rewards stay owned and claimable; the new pools apply only to future victories.

### Purple hit numbers and excavation scenery

- Incoming character damage uses the original **purple hit-number artwork**, including MISS and GUARD. Actual zero HP loss remains 0, and Magic Guard MP loss stays separately labeled.
- Outgoing hits retain their existing artwork and individual recorded rolls.
- **Excavation Sites I–III and Remains &lt;Tomb&gt; I–IV** use original terrain and sky artwork, with a matching ruins foreground platform. The scenery is bundled for offline Hunt and World Map use.

### Verification and saved progress

**1,308 Flutter tests and 69 source/data tests passed**, with clean analysis and signed APK validation. A disposable Android clone completed two normal cold launches, an in-place update and the normal backed-up 1.22 → 1.23 upgrade. Its synthetic account preserved **36/36 gameplay groups and 52/52 prior backup rows**; live Tomb I movement and incoming-damage checks passed.

The original emulator account and phone were untouched. These checks do not certify an uninspected phone's state, physical-phone performance or complete class/economy parity.

</details>

## Screenshots

Hunt is a **0.26.0** example-character preview; Opening, Inventory and Quests retain **0.24.0** labels. Other module images in [Game features](#game-features) retain their explicit **0.23.0** or **0.22.0** capture labels. Select an image for full size; forecasts are illustrative.

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-opening.png" width="240" alt="RCed Idle 0.24.0 Victoria Island opening with illustrated artwork and Enter Victoria Island button"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.26.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.26.0-hunt.png" width="240" alt="RCed Idle 0.26.0 Hunt with compact blue Start control, Home scroll, potion quickslots and Classic navigation icons"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-inventory.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-inventory.png" width="240" alt="RCed Idle 0.24.0 Use inventory with item filters, ammunition, potions and compact navigation"></a></p>

<p><a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-quests.png" width="240" alt="RCed Idle 0.24.0 Quest log with Classic, Daily, Weekly and Milestones tabs"></a></p>

## Game features

**Published game: 0.27.0 · Content: 1.23.0 · Overview dated 28 October 2026**

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
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.26.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.26.0-hunt.png" width="240" alt="RCed Idle 0.26.0 Hunt with compact blue Start control, Home scroll, potion quickslots and Classic navigation icons."></a>
</p>

[Hunt (0.26.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.26.0-hunt.png)

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

### Field rates and excavation routes on content 1.23

Ordinary maps recommended for level 10 or above retain **5/11** of their previous EXP multiplier, except **Remains &lt;Tomb&gt; I**, which retains **65%** because routing also reduces its throughput. Earlier starter maps retain their EXP profiles. Field mesos multipliers above 1 retain half the bonus above 1; for example, 1.6 becomes 1.3. Monster base rewards, potion prices, skill damage and ordinary drop chances are unchanged.

Between targets, routing weighs nearby living monsters against reachable denser platforms and their real travel cost. Characters finish the current target and pending Final Attack first. Route commitment and a short clearing window reduce immediate backtracking; spawn timers and capacities are unchanged. This is a hunting heuristic, not guaranteed optimal routing.

**Balance remains provisional:** some tested skill rotations still lose net mesos, and coin income and potion consumption need joint tuning. Gross mesos are not net profit, and the calibration does not reproduce every player's build or establish exact Classic economy parity.

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
- Buy supplies, equipment and scrolls with mesos. On content 1.19, shop weapons require **level 30 or below**; all 55 higher-level weapons retain monster-drop routes, existing crafting recipes and their owned copies, stats, upgrades and sale values. Non-weapon equipment stock is unchanged. Review and sell multiple inventory items together. Stack sales offer an **All** shortcut and explicit confirmation.
- Unlock **54 crafting recipes** through the level-10 milestone, including material refining and equipment crafting.
- Claim the level-40 milestone to unlock optional **Auto-sell**, then use an item's tooltip control to select its future-drop rule. It applies only to future monster drops, keeping existing inventory and storage intact. Farming targets, wishlisted items, active quest materials, NX items and equipped, locked or scrolled gear are protected; the control explains locked, paused and protected rules.

On content 1.20 or later, bow and crossbow arrows stack to **5,000**; throwing stars remain at 1,000. Ordinary zero-value items can be batch sold or selected for future Auto-sell for **0 mesos**. Manual sales remove the selected quantities together; equipped and locked gear is protected and scrolled gear requires confirmation. Automatic target, wishlist and quest protections do not prevent intentional manual sales.

On current content, full bags do not stop EXP and mesos from ordinary hunting, but new item drops that cannot fit are skipped.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-inventory.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-inventory.png" width="240" alt="RCed Idle 0.24.0 Use inventory tab with potions, ammunition, food, search and item filters."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png" width="240" alt="RCed Idle 0.22.0 compact classic tooltip for a Brown Pole-Feather Hat with requirements, stats and Unequip, Compare and Scroll actions."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png" width="240" alt="RCed Idle 0.22.0 Workshop crafting panel with a Bronze Ingot recipe, batch sizes, ingredient requirements and Craft button."></a>
</p>

[Inventory](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.24.0-inventory.png) · [Item details](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png) · [Crafting](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-crafting.png)

### Quests, milestones and the Special shop

Complete **16 active Classic quests**, including Hungry Ronnie at level 32, plus one daily hunt and one weekly hunt. Offline kills count toward supported objectives. Follow accepted objectives on Hunt and collect rewards from the quest log. Hide individual tracked quests without abandoning them or changing progress; visibility is saved per character.

Every ten-level milestone can be claimed for **six more slots in each ordinary inventory pocket**. Certain milestones also grant reset coupons.

The **Special shop** sells full AP/SP resets, hairstyle coupons, hair color coupons, random NX boxes and two-hour 2× EXP coupons for mesos. A Hairstyle Coupon costs **1,000,000 mesos** and unlocks a style while preserving the current color; a Hair Color Coupon costs **500,000 mesos** and changes the color of the currently worn style. These separate coupon rules require content 1.18 or later. Items are purchased first and activated separately. On content 1.20 or later, all six Special shop items share the **200-slot NX pocket**. Existing quantities are preserved on upgrade; overflow is retained, but transactions cannot increase occupied slots while over capacity. Extra EXP coupons extend the duration at the same 2× multiplier; their timers continue while paused or offline.

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
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png" width="240" alt="RCed Idle 0.22.0 character roster with two example characters, a locked third slot and Shared storage button."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png" width="240" alt="RCed Idle 0.22.0 shared storage with compact square item slots, category tabs, Deposit and Withdraw controls and search filters."></a>
</p>

[Characters](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-characters.png) · [Shared storage](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-shared-storage.png)

### Customize your appearance

Choose a name, skin, hairstyle and face, then watch equipped gear change your character's appearance. Styling remains available after creation, with a one-time character rename.

The current catalog includes **2,090 reward-eligible NX equipment items and weapon covers**, including **247 compatible weapon covers**, plus **190 source hairstyles across 1,496 exact color variants**. The two existing starter styles, Zeta and Unkempt Hair, bring Styling to **192 displayed style groups**. NX equipment changes appearance without replacing normal combat stats. The separate NX inventory pocket holds **200 slots**.

On content 1.18 or later, saved hairstyles appear once in Styling. A Hairstyle Coupon unlocks a style while preserving your current color; switching to an owned style also uses that color when available. A style without the matching color is shown as unavailable rather than silently recoloring the character. Source palettes vary, and some styles only have Black.

A Hair Color Coupon changes the currently worn style after confirmation and saves the resulting exact variant for that character. Saved colors remain free to select on their matching currently worn style, and an already-saved or current color cannot consume another coupon. Color ownership does not carry across every hairstyle or character. Existing saved variants remain intact.

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

Plan supplies for **1, 4, 8 or 24 hours**, review shortages and costs, and buy a selected supply basket manually. View estimated EXP, mesos, supply costs and time to the next level. Journal tracks discoveries, while Journey records progression milestones and advancements.

The [grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) explains combat formulas, **35 variable groups and all 94 skills**, including their conditions and how they affect training. Damage thresholds, accuracy, overkill, travel and supply costs mean an item or skill point does not have one universal EXP percentage.

Optional local notifications cover level-ups, target and rare drops, supply stops, defeat and advancement. They are off by default; delivery depends on Android's background settings. Enlarged text, reduced motion and optional workshop sound support different play preferences.

**Eighteen locally bundled music tracks include the login theme and explicit assignments for all 38 maps.** Thirty-one ordinary maps use audited source assignments; Drake's Meal Table uses the requested Sleepy Wood override. Five custom boss arenas inherit their background-map music, while Jr. Balrog retains its dedicated theme. Settings provides a toggle and volume slider, initially at 30% volume. Same-region travel does not restart the track. Playback stops when the app leaves the foreground, loses audio focus or headphones disconnect; foreground return starts the assigned track again. Music is offline, and changing its settings does not change character progress. Combat sounds have an independent Settings toggle and volume slider. The offline trial includes 45 monster hit reactions and four crossbow recordings; Double Shot and Final Attack: Crossbow reuse the basic crossbow clip. Other weapon-family attack sounds are outside the trial. Sounds follow live events without replaying an offline/resume backlog; some historical rotations remain silent.

### Keep your progress

Export and import a **complete account backup** from Settings, including every character and shared storage. Existing characters retain their current content rules until you choose **Review content update → Back up & upgrade**, which settles pending time under the old rules and creates a safety backup. Upgrade each character independently to **content 1.23** for revised field reward profiles, density-aware routing and future boss loot pools, alongside prior content changes; new characters start on 1.23. Packs through 1.22 retain their original simulation until upgraded. Earlier pinned content keeps its own rules, including the exact-variant hair behavior on 1.17. Installing the APK alone does not switch a character's content pack. The animated opening, Hunt interface and music arrive with the app update.

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
- [Download the feature guide](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.27.0/RCed-Idle-Game-Features.md) or [patch history](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.27.0/RCed-Idle-Patch-History.md) as a file.
- [Browse all releases](https://github.com/iRCed7/rced-idle-releases/releases) — earlier archive entries contain patch notes only, without old game binaries. The staged 0.11.0 changes shipped in 0.12.0.

The APK's SHA-256 checksum is attached to each game release.
