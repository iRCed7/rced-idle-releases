# RCed Idle — Patch History

Complete recorded release history through **0.20.0**, assembled on **27 October 2026**. Earlier entries describe the features and balance at that time; later updates may replace those rules. Historical verification dates are retained, while these GitHub archive entries were added on 27 October 2026.

[Download the latest game](https://github.com/iRCed7/rced-idle-releases/releases/latest) · [Main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)

**About 0.11.0:** no separately verified release artifact is recorded. Its staged Warrior, drop and interface work was combined into 0.12.0, which was verified as an update from 0.10.0. That work is covered in the 0.12.0 notes below.

## Release index

| Version | Main update |
| --- | --- |
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
