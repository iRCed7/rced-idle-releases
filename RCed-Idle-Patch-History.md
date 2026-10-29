# RCed Idle — Patch History

Complete recorded release history through **0.34.0**, updated on **30 October 2026**. Earlier entries describe the features and balance at that time; later updates may replace those rules. Historical verification dates are retained, while these GitHub archive entries were added on 27 October 2026.

[Download the latest game](https://github.com/iRCed7/rced-idle-releases/releases/latest) · [Main game features](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)

**About 0.11.0:** no separately verified release artifact is recorded. Its staged Warrior, drop and interface work was combined into 0.12.0, which was verified as an update from 0.10.0. That work is covered in the 0.12.0 notes below.

## Release index

| Version | Main update |
| --- | --- |
| [0.34.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.34.0) | Mage balance |
| [0.33.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.33.0) | Warrior balance and startup memory fix |
| [0.32.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.32.0) | Thief, Assassin and Bandit |
| [0.31.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.31.0) | Shared skill logic and archer balance |
| [0.30.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.30.0) | Classic controls and crafting journal |
| [0.29.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.29.0) | Professions and offline crafting |
| [0.28.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.28.0) | Progression economy and net income |
| [0.27.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.27.0) | Field rates, platform routes and boss loot |
| [0.26.0](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.26.0) | Damage numbers, NX drops, reports and audio |
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

## RCed Idle 0.34.0 - Mage balance

Released 30 October 2026. App version **0.34.0**, content version **1.30.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup, then **install over the existing app without uninstalling or clearing data**. Enable the new rules per character through **Settings > Review content update > Back up & upgrade**. Existing characters retain their saved rules until that action. Content 1.29 remains bundled unchanged; pending time settles under the old rules and a safety backup is created. AP/SP, progress, equipment, inventories, other characters, shared storage, appearances, professions and crafting are retained.

### Recovery, damage and travel

- **Improved MP Recovery** scales from **1% to 2% of maximum MP every ten seconds** by rank.
- **Magic Claw** gains a rank-scaled direct bonus up to **18%**. Energy Bolt retains its cheaper cost and longer range.
- **Teleport** uses half its source per-use MP before solo tuning, and only activates when a same-platform walk saves at least **150 ms**.

### Slow, burn and poison

Slow has a **six-second recast cooldown** and half its source MP and animation time. Effects apply to monster lives, so a replacement pack can be slowed without waiting for a dead pack's old duration. Automatic use skips short fights and immune targets.

Fire Arrow burn and Poison Breath poison keep separate bounded schedules. Previously paid effects survive the content upgrade.

### Cleric choices

**Heal below HP %** is an optional Attack rules tactic, **off by default**. It preserves the damage rotation, requires meaningful missing HP and pays normal cast time and MP. Active **Bless** discounts Heal MP by its source healing bonus, including when max-rank Heal already fills HP.

**Holy Arrow deals 70% of its previous direct damage on ordinary fields**, reducing its earlier advantage against living monsters. **Boss damage and Heal's undead damage remain unchanged.** A 30% direct-damage adjustment does not imply a flat 30% EXP loss: overkill, travel and spawn saturation affect actual rates. Boss status immunity and undead flags remain.

### Scope and balance limits

This pass covers Magician, Fire/Poison Wizard, Ice/Lightning Wizard and Cleric. Maps, rewards, drops and earlier class policies are unchanged. It does not claim every skill improves every rate or universal class parity. **Simulated parties remain deferred.**

Combat decisions use bounded current-state calculations. Existing background forecasting, caching and on-demand content loading remain; no new synchronous forecast or route search is added.

### Verification and saved progress

The release passed **1,601 Flutter tests**, **89 Node checks**, clean analysis, **858 controlled Mage trials** and ten exact historical replays. Package identity, release signature, 16 KB alignment, prior assets and frozen content were verified.

A synthetic Android **0.33 to 0.34 in-place update** preserved the database before launch. Cold launch, restart, Hunt rendering and save-oracle checks passed, retaining all **56 prior backup records**. These checks used the test emulator; the player's phone was untouched.

Controlled builds use fixed legal levels and labelled equipment, not a natural gear-acquisition campaign. Desktop engine timings do not establish Android frame rate, latency or battery use.

### Game guides and release history

- [Full features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached. Check GitHub manually for updates.

---

## RCed Idle 0.33.0 - Warrior balance and startup memory fix

Released 30 October 2026. App version **0.33.0**, content version **1.29.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup, then **install over the existing app without uninstalling or clearing storage**. Enable the new rules for each character through **Settings > Review content update > Back up & upgrade**. Existing characters keep their pinned version until that action. The unchanged 1.28 pack remains bundled; AP/SP, progress, equipment, inventory, shared storage, appearances, professions and other characters are retained.

### Free Warrior Final Attack

All six Warrior Final Attacks become bonus follow-ups after a landed **Power Strike or Slash Blast**, without an extra action, HP, MP or ammunition. The source **25% trigger chance** remains, with at most one follow-up per eligible cast. Only living enemies in the same platform group and source reach are eligible; it cannot trigger itself or create a replacement target.

Free hits use **40% of the captured damage multiplier**, before existing class/level policy:
- Fighter Sword/Axe: up to three survivors, effective multiplier **0.56-0.80** per target.
- Page Sword/Blunt: one survivor, **1.08-1.44**.
- Spearman Spear/Polearm: one survivor, **1.04-1.40**, retaining **5-10% actual-damage lifesteal**. Healing is bounded by missing HP, 25% of player maximum HP and monster maximum HP; overkill does not create healing.

Weapon stats, mastery, accuracy, critical rolls and defense still apply. Axe bleed and spear defense bypass retain their rules. Skill descriptions and comparisons show the free behavior. An obsolete paid Warrior Final Attack queue is cleared only at the explicit upgrade boundary; the first bonus requires a new eligible hit.

### Threaten

Threaten applies to monster lives and has a **six-second recast cooldown**, allowing a new pack to be weakened after earlier targets die. Source range, four-target limit, slow, duration and immunities remain.

Weapon-defense reduction uses the greater of the flat source amount **2-10** and **5-15%** of monster defense. MP is halved after the existing solo calculation, rounded up; cast timing is halved and rounded to a 30 ms animation step.

Automatic use requires two nearby eligible monsters expected to survive at least two primary casts, or one physical threat expected to survive at least four. Short fights, empty encounters and immune targets are skipped without spending resources. Manual use remains available. Previously paid legacy effects retain their original expiry after upgrading.

### Physical Rush

Rush now dashes up to **100 map pixels** on the current foothold during its existing paid animation. Landed hits push eligible survivors ahead by up to **60 pixels**, bounded by the platform and spawn position; enemies return at 60 pixels per second. Repeated casts cannot push indefinitely.

Six-target damage, two-second cooldown and original HP/MP costs remain. A missed cast still pays for and performs the dash. Nonimmune survivors retain 750 ms contact suppression. The character resists stagger during the dash but can still take damage; no vertical links or blanket immunity are added.

Use Rush in attack rules with a suitable monster threshold; cooldowns fall through to the next ready attack. Directly selecting Rush uses Basic Attack during cooldown. It is a situational positioning option, not a mandatory replacement for Power Strike or Slash Blast.

### Defense and balance limits

Iron Body, Iron Will, Improved HP Recovery, Max HP Increase, Rage, mastery and boosters retain published values. Rage keeps its defense penalty. Recovery ranks improve potion efficiency, while passive regeneration stays at 1% of derived maximum HP per ten seconds at every learned rank. Iron Will avoids the 120 ms next-action interruption floor when a hit would delay the character; it does not subtract that time from every hit.

Testing completed **1,668 controlled trials: 1,452 field trials and 216 boss attempts** across six Warrior weapon paths. All field trials completed their horizons and all sampled boss attempts won. These are comparable legal checkpoint builds, not a natural acquisition playthrough or universal profitability guarantee.

Maps, monster EXP/mesos, drops and earlier Archer/Thief policies are unchanged. Magician balancing and simulated parties remain deferred.

### Startup memory fix

The initial candidate was withheld after native testing found Dart heap exhaustion. The rebuilt release loads current content and only historical versions referenced by saves, decodes large packs away from the UI thread and releases temporary validation packs. Background notifications use the same on-demand approach.

All historical packs remain bundled, preserving old saves, backups and explicit upgrades. This changes loading and memory use, not saved rules or rewards. Corrected startup memory snapshots were much lower, but they are not peak-memory or physical-phone performance guarantees.

### Verification and saved progress

The final complete Flutter suite passed **1,565 tests with no failures or skips**; **89 Node checks** and analysis passed. The signed rebuilt APK passed package, alignment and offline-permission checks.

Synthetic Android testing followed the existing 0.32 installation through the withheld candidate and corrected APK, without uninstalling or clearing data. Two cold launches and a separate resting Hunt-screen entry passed. All **56 prior backup records** and saved ownership were preserved; the character remained pinned to content 1.26. Repository tests cover the explicit 1.29 upgrade.

This was not a direct 0.32-to-final native test, sustained grinding test or inspection of the player's phone. The failed candidate is not distributed.

### Game guides and release history

- [Full features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached. Check GitHub manually for updates.

---

## RCed Idle 0.32.0 - Thief, Assassin and Bandit

Released 29 October 2026. App version **0.32.0**, content version **1.28.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup, then **install over your existing app without uninstalling or clearing storage**. To enable the new rules for each character, use **Settings > Review content update > Back up & upgrade**. Existing characters keep their pinned rules until that action. The unchanged 1.27 pack remains bundled; points, items, appearances, professions, other characters and shared storage are preserved.

### Optional attack tactics

Open **Attack rules**, enable rules and choose learned tactics. Existing rotations are retained and **new tactics start off**.

- **Drain:** use below a chosen HP percentage, then return to the normal attack. Healing comes from HP actually removed by landed hits, excluding overkill and misses. Rank scales damage conversion from 10% to 20% and the per-cast cap from 2% to 8% of maximum HP. Original MP/star costs apply, with a six-second cooldown. Set Drain above the potion threshold; 75% Drain and 65% potions is a starting point. Potions retain priority below their threshold. Directly selecting Drain uses basic attacks during cooldown.
- **Disorder:** one automatic opening attempt per monster, including misses, against a reachable non-immune target expected to take at least four normal casts. MP and action time are halved with rounding. Physical attack reduction uses the greater of the source flat amount and 5-20% of monster attack. Source defense reduction and duration remain.
- **Steal:** one automatic attempt per monster life, then return to the main attack. Successful theft retains source stun and the temporary attack buff. Eligible loot is selected independently of table order: the chance of any item combines eligible row probabilities, then at most one row is selected proportionally. No EXP or mesos is granted. Quest rules and bag capacity apply; global NX is excluded and boss loot cannot be stolen. Boss Steal may still grant its combat buff.

Tactics use the focused target within normal platform/range rules, without unrelated detours. Disorder and Steal remember attempts through save/reload until that monster respawns. Comparisons preserve the ordinary rotation and describe tactic assumptions.

### Dark Sight, Haste and Claw Mastery

**Dark Sight** keeps concealment until a real attack is paid for. That attack arms a three-second guard against the next landed contact hit, reducing it by 25-50% by rank. Evasion does not consume it; magic is neither blocked nor consumes the guard. Base MP cost scales from 10 to 6 before the existing solo cost multiplier, with a 20-second cooldown. Automatic use requires a durable threat within 80 map pixels whose typical contact hit reaches at least 5% of maximum HP. It has a cast-time cost and is not permanent invulnerability.

**Haste** retains capped movement speed. Jump additionally shortens existing jump links by 1% per jump point, capped at 10%. It creates no paths and does not accelerate climbing, falling or attacks. Route selection and travel use the same cost.

**Claw Mastery** raises Lucky Seven's minimum-roll mastery floor from 50% toward 65%. Maximum damage, two-hit structure and star retrieval remain unchanged.

Critical Recovery, Nimble Recovery, boosters, accuracy/evasion, Keen Eyes, Double Stab and Savage Blow retain their existing mechanics.

### Balance results and limits

Controlled testing completed **756 trials**: 636 screening field trials, 48 extended Drain trials and 72 boss attempts. All field trials completed their horizons, and all sampled boss attempts won. Utilities can trade EXP for survival, income or loot; three candidate map/build means still had negative net mesos.

Monster EXP, mesos, raw drops, map layouts and the earlier Archer policy are unchanged. These are legal controlled checkpoint builds, not a natural level-1-to-70 playthrough or proof of universal class parity. Warrior and Magician passes and simulated parties remain deferred. Desktop simulation timings do not establish phone performance.

### Verification and saved progress

The final complete Flutter suite passed **1,502 tests with no failures or skips**; **89 Node checks** and analysis also passed. Earlier attempts were superseded by a final build including the corrected utility-aware supply estimate.

The signed APK passed identity, alignment and offline-permission checks. After resolving a software-rendering emulator failure using the host-GPU configuration and reinstalling the same APK without clearing data, two cold-launch checks passed. All **56 prior backup records**, account identity, roster and shared storage were preserved.

Native checks verified startup and checkpoint loading with content 1.26 still pinned, not an interactive Hunt playthrough or native 1.28 upgrade. Automated repository tests cover the backed-up content migration. The player's phone and personal save were untouched.

### Game guides and release history

- [Full features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached. Check GitHub manually for updates.

---

## RCed Idle 0.31.0 - Shared skill logic and archer balance

Released 29 October 2026. App version **0.31.0**, content version **1.27.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup, then **install over the existing app without uninstalling or clearing data**. Existing characters remain on their saved rules until **Settings > Review content update > Back up & upgrade** is selected for each character. Content 1.26 remains bundled unchanged. Owned items, SP/AP, progress, appearances, professions, other characters and shared storage are preserved; only an obsolete queued archer Final Attack is cleared on upgrade.

### Archer Final Attack

Hunter and Crossbowman Final Attack now adds bonus hits to a landed eligible attack without an extra action, MP, HP or arrows, and without delaying the next attack. It cannot trigger itself. Only surviving enemies on the current platform and within range are eligible; clearing the group does not create another target or extra loot.

The idle policy uses a **25% trigger chance and 55% of the captured rank's damage multiplier**, accounting for the removed animation and supply costs. Bow distributed hits and crossbow single-hit structure remain. Skill descriptions show the effective behavior. Your allocated SP and toggle are retained. **Warrior Final Attack keeps its earlier behavior** pending its own balance pass.

### Power Knockback and better routing

Power Knockback physically pushes surviving, non-immune monsters on the current platform. Rank determines distance up to 100 source-map pixels; monsters return at 60 pixels per second. The push stays within the platform and is bounded relative to spawn position. Contact damage is suppressed only outside the 80-pixel contact reach; enemy spells remain possible. A short animation shows the push.

Automatic knockback rules count close enemies. Cooling-down skills now fall through to the next eligible attack. Automated attacks avoid Heal when no undead target is available; manually selected Heal still heals against living monsters.

Routing considers productive groups reachable by walking on the current platform before taking a platform detour. Existing travel commitments and arrival-group clearing remain. This corrects unnecessary detours observed in Tomb I without a map-specific reward bonus.

### Shared utility corrections

- Slow effects retain their own strength and expiry; the strongest active slow applies without multiplying overlapping effects.
- Debuffs filter range, immunity and existing effects before filling target limits, avoiding empty or already-covered automatic casts.
- Incoming attack cadence reflects the living group's actual statuses, rather than treating the first monster as representative.
- Automatic recovery keeps its cooldown when both resources are full. MP Eater at full player MP drains only when it can prevent an affordable enemy spell.
- Automatic Focus and Nimble Feet check whether they can help current combat or travel; manual activation remains available.
- Boss reports retain unique attempt IDs, including same-time retreats. Background notifications resolve characters still pinned to content 1.26.

### Balance results and limits

Controlled testing covered **900 field trials and 132 boss attempts**, plus **240 cross-class ten-minute sessions**. Longer paired level-52 Tomb I tests gained roughly 12% EXP with learned Final Attack enabled. A level-60 rank-1 Crossbowman Drake case was effectively neutral for EXP, with more kills and better net mesos. These are controlled builds, not promises for every equipment set or rotation.

Monster EXP, mesos, drops, spawns and shop prices are unchanged. Some mage rotations and SP-heavy archer builds still have poor net mesos. **Warrior, Thief and Mage tuning and simulated parties remain deferred.** This is not a complete balance certification or an overall performance improvement.

### Verification and saved progress

The initial full Flutter suite passed 1,443 cases with four failures; all four were resolved by successful affected-suite reruns. Rerun counts overlap, so this is not a single clean full-suite result. All **89 Node checks** and final analysis passed.

The signed APK passed identity, alignment and offline-permission checks. Synthetic Android in-place installation and two cold launches preserved the pinned 1.26 checkpoint and all **56 prior backup records**. Native checks verified startup and checkpoint loading, not an interactive Hunt playthrough or native 1.27 upgrade. Repository tests separately verified the backed-up migration with three characters, shared storage and an active craft.

The player's phone and personal save were untouched. Physical-phone frame rate and battery use were not measured. Existing artwork, music, sounds and opening assets are unchanged.

### Game guides and release history

- [Full features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached. Check GitHub manually for updates.

---

## RCed Idle 0.30.0 - Classic controls and crafting journal

Released 29 October 2026. App version **0.30.0**, content version **1.26.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup, then **install over your existing app without uninstalling or clearing data**. For each existing character, use **Settings > Review content update > Back up & upgrade** to enable the new content rules. Content 1.25 remains bundled unchanged; learned professions, reserved jobs, equipment, cosmetics, other characters and shared storage are preserved.

### Crafting journal and faster batches

- Browse six profession tabs, mastery, recipe lists, output stats and a required-materials grid. Phones have a focused detail view; wider screens show list and detail columns.
- Select a craftable ingredient to open its recipe, including across professions, then return to the original recipe.
- Enter a quantity, use **MAX** for the affordable amount, or **Craft All**, with a 10,000-craft safety limit. Equipment-consuming recipes still require exact-item confirmation and run one at a time.
- New jobs take **250 ms per craft** on content 1.26. Already reserved jobs keep their saved duration after upgrading.
- Batches continue offline. Full-bag output remains held safely, and cancellation refunds only unfinished materials and fees.

### Classic controls and character selection

- New touch keycaps for attacks, buffs and supplies, with per-skill monster thresholds and matching shortcuts below Hunt. These are touch controls, not keyboard automation.
- HP/MP shortcuts open the matching recovery selection. Throwing-star controls appear only for Thief characters.
- Compact blue/orange Grind/Rest controls share a row with EXP, net mesos and next-level timing.
- AP/SP allocation has adjacent arrows for individual points and a larger allocation plan.
- Inventory displays all unlocked cells, loads large grids efficiently, hides the worn NX copy while retaining extra copies, and fixes the toolbar edge.
- Equipment shops default to the active character's class, resetting on character changes; whole-number prices omit unnecessary decimals.
- The character selector uses Classic treehouse and bridge artwork, outfits, a parchment stat card and wooden actions. Previewing a character does not activate it until confirmed.
- The old standalone Android icon splash is removed. A brief matching background handoff leads into the existing animated opening and music.

### Random hair and color unlocks

On content 1.26, hairstyle coupons randomly unlock an unowned style while any remain, retaining the current color where supported. Color coupons randomly unlock a missing color of the current style while any remain. Once all eligible choices are owned, the dialog explains that another owned look may be selected. Acquired styles and colors remain free to reapply.

Hair randomness is saved separately from combat and loot randomness. Existing looks, unlocks and coupons are retained. Earlier pinned packs keep their targeted coupon behavior until upgraded.

### Movement recovery and platform routes

Fixed a reproduced upgrade/resume error that could leave a paused climb with an expired movement segment. New upgrades preserve the pause cursor; already affected paused saves recover the short travel segment without resetting character progress, inventory or loot randomness.

Routing commits the full trip to another platform and clears the monsters present on arrival before reconsidering a density detour. Respawns behind the character no longer cause an immediate ordinary-climb reversal, and fresh spawns do not extend the arrival commitment forever.

### Balance limits and Final Attack

Final Attack remains a paid single-target follow-up with its own animation, which can delay crowd attacks. Controlled same-build samples averaged about 6% less EXP with it enabled at level 52 and about 1.7% more at level 70. These are sampled results, not universal build advice; no arbitrary damage or cost adjustment was made.

The solo audit still finds clustered map winners and some negative high-level mage/bow net-meso profiles. Balance work remains ongoing and **parties remain disabled**. Monster rewards, spawn limits and drop tables are unchanged.

### Verification and saved progress

Verification covered **1,409 distinct Flutter cases** across the initial regression run and successful reruns resolving all 18 initial failures, plus **89 Node checks** and clean analysis. This was not a single clean full-suite run.

The signed APK passed identity, alignment and offline-permission checks. Synthetic Android tests passed in-place installation, content upgrade, crafting and restart checks. All **55 prior backup records** were preserved and a safety backup added. The user's phone and personal save were not modified or tested; physical-phone performance was not measured.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached. Check GitHub manually for future updates.

---

## RCed Idle 0.29.0 — Professions and offline crafting

Released 29 October 2026. App version **0.29.0**, content version **1.25.0**. Requires **Android 8.0 or later**.

### Install or update

Export a complete account backup from Settings, then install this APK over your existing app. **Do not uninstall or clear app data.** Existing characters retain their pinned rules until you choose **Settings → Review content update → Back up & upgrade** for each character. Claim the **level-10 milestone** to unlock Crafting.

### Six professions, two specializations

Choose from **Smithing, Weaponcrafting, Tailoring, Woodcrafting, Leatherworking and Arcforge**. Each character can learn two professions, with confirmation. **Choices cannot be reset in this update.** Share materials and finished items between characters using shared storage.

Each discipline has ranks **1–8**, gated by character levels 10, 10, 15, 20, 25, 30, 35 and 40. A full mastery bar waits at its level gate; overflow is discarded, and another completed craft advances the rank after the level requirement is met. Earlier recorded crafts credit mastery when the matching profession is learned, without granting duplicate items or selecting a specialization for you.

### Timed batches and safe collection

- **279 usable recipes**, retaining the IDs, ingredients, quantities and fees of all 54 earlier recipes.
- Start batches of **1, 10 or 100** crafts. One queue runs per character while resting, hunting or offline; each execution takes three, five or seven seconds.
- Materials and mesos are reserved at the start. Cancellation refunds only unfinished work; completed output and mastery are retained.
- Output that cannot fit in inventory waits in the workshop for collection. Depositing items into shared storage can free room.
- Equipment-input recipes run one at a time, with exact-item selection and a consumption confirmation. Equipped, locked, scrolled, wishlisted and targeted gear is protected. Cancelling before completion restores the reserved item's identity and rolls.

### Workshop and supplies

The workshop adds profession selection, mastery, recipe search and filters, output stats and efficient scrolling lists. A Crafting shop tab adds **18 supply entries**, and the catalog includes **118 new item definitions**. No weapon above level 30 returns to NPC stock. Some recipes require another specialization's materials; every two-profession pairing is not self-sufficient.

### Scope and limits

Ranks 9–10, housing, unsupported advanced-arrow and Fame recipes, optional catalysts and profession kits are deferred. Added shop supply routes and estimated prices are RCed adaptations. **Simulated parties are not enabled.** Field EXP, mesos, monster drops, class formulas and boss balance retain content 1.24 rules. All 18 music tracks and 49 combat sounds remain unchanged.

### Verification and saved progress

Verification covered **1,369 distinct Flutter cases** across the full regression run and successful corrected reruns, plus **89 Node checks** and clean analysis. The signed APK passed package, alignment and offline-permission checks.

A synthetic diagnostic Android account passed in-place installation, two cold launches, the normal backed-up content upgrade and workshop restart/cancellation checks. All **54 prior backup records** and nine immutable backup exports were preserved. The original emulator and phone were untouched; physical-phone performance was not measured.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)

Feature and history snapshots are attached as Markdown files. Check GitHub manually for future updates.

---

## RCed Idle 0.28.0 — Progression economy and net income

Released 28 October 2026. App version **0.28.0**, content version **1.24.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from Settings.
2. Download the attached APK and open it on your Android phone.
3. **Install over the existing app. Do not uninstall first or clear its data.** Package and signing identity are unchanged.
4. Select **Settings → Review content update → Back up & upgrade** for each existing character to activate content 1.24. Pending time settles under the old rules, a safety backup is created and the character pauses for review.

Existing characters remain on their pinned content until upgraded. New characters use 1.24. The Hunt label improvement arrives with the app update.

### Progression and farming choices

- Field mesos no longer receive a penalty for outleveling monsters. Familiar maps can remain useful money-farming routes; existing EXP decay for substantially outleveled monsters remains.
- Fixed map reward profiles are retuned to offer distinct EXP, income and item-farming choices. They do not dynamically adjust to your character's forecast.
- Ordinary field monsters attempt incoming attacks every **2.4 seconds**, previously 1.5 seconds, reducing sustained potion pressure.
- Per-hit defense, Magic Guard, monster stats, skill MP costs and potion prices remain intact. Total potion spending does not fall by one fixed percentage: movement, kills, buffs, recovery and attack costs still matter.
- Boss attack behavior, cooldowns and rewards are unchanged. Ordinary item-drop probabilities are not globally increased.

The balance goal is satisfying solo progression rather than matching exact Classic hourly rates. Movement, attack speed, spawn capacity and respawn delays still limit throughput.

### Net mesos on Hunt

Hunt now shows **NET MESO /h**, matching World Map's supply-adjusted estimate. Negative values use the warning color. Adventure details retain the gross coins, auto-sale proceeds and supply-cost breakdown.

Net means monster coins plus configured auto-sales, minus the purchase value of consumed supplies still missing after matching retained drops. It does not assume that every equipment, ETC, scroll or cosmetic drop is sold. Wallet changes also include purchases, manual sales and rewards, so they are a different measure.

Estimates reuse the existing controlled-build forecast cache. They describe stocked potential, not a guarantee that your currently carried supplies last an hour.

### Balance evidence and limits

The paired audit covered **70 builds across ten branches**, at levels 10, 20, 30, 40, 52, 60 and 70. Every tested build had a profitable route even before supply-drop credit, and each had different EXP and net-income winners. All new twenty-minute samples completed.

This does not mean every route or rotation is profitable. Some costly setups remain negative, and a documented Burnt Land routing case earns less after a damage upgrade because it spends more time traveling. The checks support generally improving progression and useful alternatives, not guaranteed profit increases from every individual upgrade or universal class parity.

### Verification and saved progress

**1,346 Flutter tests and 83 source/data checks passed**, with clean analysis and signed APK validation. A disposable synthetic Android account passed in-place installation, two complete cold launches and the normal backed-up 1.23 → 1.24 upgrade.

All **38 checked gameplay groups** matched expected behavior: 35 were unchanged and three matched normal paused-time buff expiry under frozen rules. Owned player fields, equipment, inventory, shared storage, profile and all **53 prior backup rows** were preserved. The original emulator account and phone were untouched. These checks do not certify physical-phone performance.

Existing artwork, excavation scenery, all 18 music tracks and 49 combat clips are unchanged.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)
- [Grinding reference with newer-content notes](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md)

Feature and history snapshots are attached as Markdown files. Check GitHub manually for future updates.

---

## RCed Idle 0.27.0 — Field rates, platform routes and boss loot

Released 28 October 2026. App version **0.27.0**, content version **1.23.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from Settings before updating.
2. Download the attached APK and open it on your Android phone. Allow installation from your browser or file app if Android asks.
3. **Install over the existing app. Do not uninstall first or clear its data.** Package and signing identity are unchanged.
4. Select **Settings → Review content update → Back up & upgrade** separately for each existing character to activate content 1.23. Pending time settles under the old rules, a safety backup is created and the character pauses for review.

Existing characters retain their pinned rules until upgraded. New characters start on 1.23. Art changes arrive with the app; incoming damage events require content 1.22 or later.

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

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)
- [Grinding reference with newer-content notes](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md)

Feature and history snapshots are attached as Markdown files. Check GitHub manually for future updates.

---

## RCed Idle 0.26.0 — Damage numbers, NX drops, reports and audio

Released 28 October 2026. App version **0.26.0**, content version **1.22.0**. Requires **Android 8.0 or later**.

### Install or update

1. Export a complete account backup from **Settings** before updating.
2. Download the attached APK and open it on your Android phone. Allow installation from your browser or file app if Android asks.
3. **Install over the existing RCed Idle app. Do not uninstall first or clear its data.** Package and signing identity are unchanged.
4. Choose **Review content update → Back up & upgrade** separately for each existing character to enable content 1.22, including the increased NX rate and incoming-damage display. Pending progress settles under the old rules, a safety backup is created and grinding pauses for review. New characters start on 1.22.

Navigation, outgoing-hit display, reports and sound controls arrive with the app update. Earlier characters retain their pinned rules until upgraded.

### Damage you can follow

- Multi-hit attacks show each recorded damage roll separately, in order, with its own critical or miss appearance.
- If an early hit kills the monster, no extra unrolled damage number is invented. Older aggregate-only records retain one number.
- On content 1.22, incoming attacks show actual HP lost after mitigation. Magic Guard displays redirected loss separately as **MP −N**; misses and guarded attacks are distinguished.
- Reduced motion and offline/resume handling suppress transient effects. These displays do not change combat formulas, timing, rewards or random rolls.

### More frequent NX finds

Content 1.22 raises the total chance of any eligible universal NX cosmetic from **1 in 60,000** to **1 in 4,000 kills**. The same **2,090 cosmetics** remain equally likely; a particular cosmetic has a 1-in-8,360,000 chance per kill.

Hair coupons remain **1 in 120,000**. Boss rewards, first-clear guarantees, cooldowns, NX boxes and ordinary item drops are unchanged. Drops remain random with no pity timer, and new cosmetics need available NX space. Older pinned content retains its former rate.

### Cleaner Hunt and clearer reports

- World Map, Adventure details and Monster drops are grouped in the **minimap popup**. Hunt keeps Home and potion quickslots, with a compact blue Start/Pause control and no duplicate estimated-level line.
- New Classic artwork identifies Home, Monster drops, Shop and Quests.
- A small full-inventory warning opens a list of full pockets. EXP and mesos continue; only new drops that cannot fit are skipped.
- Offline reports show **retained quantities**. Auto-sold copies are excluded from carried finds, and their sale value appears exactly once in **Mesos gained**. Viewing a report grants nothing again.
- Dismissing a boss report is saved per character. Boss details, permanent clears, first-clear rewards and pending loot remain available on the Bosses page; a later encounter creates a new report.

### Combat sounds and map music

- A **Combat sounds** toggle and volume slider in Settings operate independently of background music.
- The offline sound trial includes hit reactions for all **45 monsters** and four crossbow recordings: Basic Attack, Arrow Blow, Power Knockback and Iron Arrow. Double Shot and Final Attack: Crossbow use the basic crossbow clip; other weapon-family attack sounds are outside this trial.
- Sound follows live combat without replaying an offline or resume backlog. Older packs support recognized basic/crossbow attack events; other historical rotations can remain silent.
- Seven music recordings bring the catalog to **18 tracks**, including the login theme. All prior recordings are preserved.
- Music assignments now cover all 32 ordinary maps and six custom boss arenas. **Drake's Meal Table uses Sleepy Wood**; returning Home selects the destination map's music.

### Verification and saved progress

The final full suite passed **1,260 tests**, with **47 source/content checks**, clean analysis and one separately recorded upgrade regression. APK signing, offline permissions and in-place installation passed.

Two original-account cold launches and exact preservation checks passed: all **27 gameplay groups**, profile, shared storage and all **51 prior backup rows** were retained. A separate synthetic character exercised Double Shot damage numbers, incoming HP display and music/sound controls. Native checks verified audio decoding and playback state, not subjective speaker quality or physical-phone performance.

### Game guides and release history

- [Full game features and screenshots](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Game-Features.md)
- [Complete patch history](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Patch-History.md)
- [Grinding reference with newer-content notes](https://github.com/iRCed7/rced-idle-releases/blob/main/RCed-Idle-Grinding-Reference.md)

Feature and history snapshots are also attached as Markdown files. Check GitHub manually for future updates.

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
