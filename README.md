<p align="center">
  <img src="media/rced-idle-logo.png" width="180" alt="RCed Idle game logo">
</p>

# RCed Idle

An offline idle RPG for **Android 8.0+**. Build your characters, hunt for equipment, develop your skills and progress while the game is closed.

[Latest update](#latest-update) · [Screenshots](#screenshots) · [Game features](#game-features) · [Install or update](#install-or-update) · [Patch history](RCed-Idle-Patch-History.md)

## Latest update

**0.23.0 — Attack potions, regional music and faster forecasts** · 28 October 2026

**[Download the latest APK](https://github.com/iRCed7/rced-idle-releases/releases/latest/download/RCed-Idle.apk)** · [Open the release page](https://github.com/iRCed7/rced-idle-releases/releases/latest)

- **Timed attack potions:** Warrior Potion adds +10 Attack Power and Magic Potion adds +10 Magic Attack for ten minutes. Each costs 500 mesos; use owned stock manually or enable optional renewal. Requires content 1.19.
- **Skills and potions combine:** the strongest skill bonus and strongest potion bonus add per stat, with gear and passive bonuses separate and skill drawbacks preserved.
- **Hunt for higher-level weapons:** content 1.19 limits weapon-shop stock to required level 30 or below. Higher-level weapons keep their monster drops, existing crafting recipes and owned copies.
- **Reuse completed comparisons:** equipment, shop, skill, AP and scroll previews share controlled baselines, keep immediate stat details visible and reuse finished hourly estimates when reopened.
- **Maps prepare in the background:** accessible primary routes warm after build changes, starting with the current Hunt map. Reopening keeps completed rates and pending work.
- **Clearer Hunt actions:** compact rounded Start grinding, Home and Restock controls retain complete labels and accessible touch targets; opening attack-potion controls does not consume stock.
- **Regional music, fully offline:** ten bundled tracks cover all 38 maps, with a Settings toggle and volume slider. Music stops when the app leaves the foreground and restarts when you return.

> **Updating?** Install over your existing app; do not uninstall first. Export a complete account backup from Settings. Existing characters enable new content through **Review content update → Back up & upgrade**.

<details>
<summary>Full patch notes for 0.23.0</summary>

Released 28 October 2026. App version **0.23.0**, content version **1.19.0**. Requires **Android 8.0 or later**.

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

</details>

## Screenshots

Example-character previews: **Hunt, attack-potion controls and map cards are from 0.23.0**; other module images retain their **0.22.0** capture labels. Select an image to view it at full size. Explore more modules beside their descriptions in [Game features](#game-features). Some panels are isolated previews; forecast values are illustrative.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png" width="220" alt="RCed Idle 0.23.0 Hunt screen with a green Start grinding button and labeled Home and Restock controls beneath Snail Hunting Ground II."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png" width="220" alt="RCed Idle 0.23.0 attack potion controls with Warrior Potion and Magic Potion, Use now buttons and Auto-use after expiry checkboxes."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png" width="220" alt="RCed Idle 0.22.0 compact classic tooltip for a Brown Pole-Feather Hat with requirements, stats and Unequip, Compare and Scroll actions."></a>
</p>

[Hunt (0.23.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png) · [Attack potions (0.23.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-attack-potions.png) · [Item details (0.22.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-item-tooltip.png)

## Game features

**Published game: 0.23.0 · Content: 1.19.0 · Overview dated 28 October 2026**

### Play at your own pace

- Prepare your character, choose a map, select attacks and supplies, then start grinding.
- Use the compact rounded Start grinding, Home and Restock controls beneath Hunt's map; their labels and touch targets support narrow screens and larger text.
- Earn EXP, mesos and actual item drops while the game is open or closed. Offline progress runs at the same ordinary pace, with **no away-time cap**.
- Supplies, defeat, pauses and job advancement still matter. Running out of resources can stop grinding or trigger your chosen fallback; the game does not automatically buy supplies or choose your next job.
- No online account, internet connection, advertisements or real-money purchases are required to play.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png" width="240" alt="RCed Idle 0.23.0 Hunt screen with a green Start grinding button and labeled Home and Restock controls beneath Snail Hunting Ground II."></a>
</p>

[Hunt (0.23.0)](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.23.0-hunt.png)

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

### Explore maps and challenge bosses

Explore **38 maps**, compare training routes, view their monsters and drops, follow the live minimap, and unlock progression routes. Choose a desired farm item to help rank maps by expected yield and highlight useful finds.

Accessible primary routes prepare estimates in the background after build changes, starting with the current Hunt map. Opening and closing World Map keeps ongoing work and completed results; new boss access adds routes without discarding existing rates for that build. Earlier Routes calculates retired alternatives when requested. Failed estimates can be retried, and ordinary stock changes do not restart controlled route comparisons.

Six boss encounters are available: **Mano, Stumpy, Mushmom, Shade, Zombie Mushmom and Jr. Balrog**. Victory grants EXP, mesos and equipment, with additional chances for scrolls, NX cosmetics and EXP coupons. Each boss's first clear guarantees one random NX cosmetic. Victories start a **six-hour cooldown for that boss and character**; failed attempts remain retryable. Rewards that cannot fit stay saved for later claiming.

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
- Browse armor progression by class, item type and search, including ordinary gear through level 70.
- Buy supplies, equipment and scrolls with mesos. On content 1.19, shop weapons require **level 30 or below**; all 55 higher-level weapons retain monster-drop routes, existing crafting recipes and their owned copies, stats, upgrades and sale values. Non-weapon equipment stock is unchanged. Review and sell multiple inventory items together.
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

The **Special shop** sells full AP/SP resets, hairstyle coupons, hair color coupons, random NX boxes and two-hour 2× EXP coupons for mesos. A Hairstyle Coupon costs **1,000,000 mesos** and unlocks a style while preserving the current color; a Hair Color Coupon costs **500,000 mesos** and changes the color of the currently worn style. These separate coupon rules require content 1.18 or later. Items are purchased first and activated separately. Extra EXP coupons extend the duration at the same 2× multiplier; their timers continue while paused or offline.

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

On content 1.18 or later, saved hairstyles appear once in Styling. A Hairstyle Coupon unlocks a style while preserving your current color; switching to an owned style also uses that color when available. A style without the matching color is shown as unavailable rather than silently recoloring the character. Source palettes vary, and some styles only have Black.

A Hair Color Coupon changes the currently worn style after confirmation and saves the resulting exact variant for that character. Saved colors remain free to select on their matching currently worn style, and an already-saved or current color cannot consume another coupon. Color ownership does not carry across every hairstyle or character. Existing saved variants remain intact.

Use Back/Next arrows to browse named hairstyles and **Hide worn equipment** to see hair on the bare-character preview. The toggle does not unequip real items. Previews do not change saves or consume coupons; closing without saving preserves the original appearance.

The same eligible cosmetic catalog appears in rare universal drops, Random NX Boxes and boss rewards. Boxes select equally among the 2,090 appearances, and duplicates are possible. Each defeated monster has a **1-in-60,000 cosmetic chance** and a **1-in-120,000 hairstyle-coupon chance** as alternative global outcomes. Those are probabilities, not guaranteed rewards after that many kills. The Hair Color Coupon is sold in the shop; it has no added global drop chance. Boss-specific cosmetic rewards are separate. Ordinary drops that cannot fit are skipped; pending boss rewards retain their existing protection.

The catalog covers the supported physical cash equipment and hairstyles from the **GMS95 artwork source**, rather than every cosmetic from every region or era. **Rings, chat bubbles and partner effects are excluded**, and seven Pirate-only covers remain reserved. Weapon covers follow their supported weapon types and original pose availability; incompatible or deliberately hidden poses can leave a cover invisible. Artwork loads for requested outfits instead of loading the entire wardrobe on each screen change.

<p>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png" width="240" alt="RCed Idle 0.22.0 Classic Hair Coupon preview with hairstyle carousel, search and Hide worn equipment option."></a>
  <a href="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png"><img src="https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png" width="240" alt="RCed Idle 0.22.0 Hair Color Coupon dialog with an Acorn hairstyle preview and color swatches."></a>
</p>

[Hair styles](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-style.png) · [Hair colors](https://raw.githubusercontent.com/iRCed7/rced-idle-releases/main/media/screenshots/v0.22.0-hair-color.png)

### Plan, track and stay informed

Plan supplies for **1, 4, 8 or 24 hours**, review shortages and costs, and buy a selected supply basket manually. View estimated EXP, mesos, supply costs and time to the next level. Journal tracks discoveries, while Journey records progression milestones and advancements.

The [grinding reference](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md) explains combat formulas, **35 variable groups and all 94 skills**, including their conditions and how they affect training. Damage thresholds, accuracy, overkill, travel and supply costs mean an item or skill point does not have one universal EXP percentage.

Optional local notifications cover level-ups, target and rare drops, supply stops, defeat and advancement. They are off by default; delivery depends on Android's background settings. Enlarged text, reduced motion and optional workshop sound support different play preferences.

**Ten locally bundled background-music tracks cover all 38 maps**, using regional and biome assignments chosen for RCed. Settings provides a toggle and volume slider, initially at 30% volume. Same-region travel does not restart the track. Playback stops when the app leaves the foreground, loses audio focus or headphones disconnect; foreground return starts the assigned track again. Music is offline, and changing its settings does not change character progress. Attack and monster sound effects are not included.

### Keep your progress

Export and import a **complete account backup** from Settings, including every character and shared storage. Existing characters retain their current content rules until you choose **Review content update → Back up & upgrade**, which settles pending time under the old rules and creates a safety backup. Upgrade each character independently to **content 1.19** for timed attack potions, the skill/potion stacking rules and the weapon-shop level limit; new characters start on 1.19. Earlier pinned content keeps its own rules, including the exact-variant hair behavior on 1.17. Installing the APK alone does not switch a character's content pack. Forecast caching, the Hunt interface and music arrive with the app update.

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
- [Download the feature guide](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.23.0/RCed-Idle-Game-Features.md) or [patch history](https://github.com/iRCed7/rced-idle-releases/releases/download/v0.23.0/RCed-Idle-Patch-History.md) as a file.
- [Browse all releases](https://github.com/iRCed7/rced-idle-releases/releases) — earlier archive entries contain patch notes only, without old game binaries. The staged 0.11.0 changes shipped in 0.12.0.

The APK's SHA-256 checksum is attached to each game release.
