# RCed Idle Grinding Reference

**App 0.23.0 · Content 1.19.0 — with newer-content compatibility notes**

> **Content 1.22 (app 0.26.0):** Universal NX cosmetic probability is now 1 in 4,000 kills across the same 2,090 appearances; hair coupons remain 1 in 120,000. Earlier pinned content retains its former rate. Boss and ordinary drops are unchanged from 1.21. Incoming HP/MP events and individual outgoing numbers present resolved combat values without changing damage formulas. Older NX probabilities below describe their labeled historical pack.

> **Content 1.21 compatibility (app 0.25.0):** The original tables below describe 1.19. Platform travel now uses Speed, actual distance and paid platform connections; attacks and multi-target thresholds use eligible targets within range on the same platform. Teleport only shortens same-platform walking, and cannot bypass connections. Comparisons start at the selected map entrance. Ordinary equipment and HP/MP restoration drop chances are halved, with one restoration item per drop. Boss rewards, global NX, scrolls, materials and arrows are unchanged. Content 1.20 also raised arrow stacks to 5,000, moved Special shop items into NX and allowed zero-value sales. Older movement, supply and loot descriptions below should not be used as 1.21 rules. See the [0.25.0 notes](https://github.com/iRCed7/rced-idle-releases/releases/tag/v0.25.0) and in-game monster encyclopedia for current rules. Characters pinned to earlier content retain their original simulation.


[Main game page](https://github.com/iRCed7/rced-idle-releases) · [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest)

This guide explains what changes EXP, mesos, item farming and supply use in RCed Idle. It covers all **35 variable groups** and all **94 skill entries**: Basic Attack plus 93 trainable skills. Exact rank values appear in the in-game skill book; the overview here explains what each skill does and when its benefit changes or disappears.

The guide describes RCed's implemented idle simulation. Confirmed source values, RCed solo balance adjustments and estimated mechanics are different kinds of information. Adaptations and unresolved source details are called out below. No stat, item or skill grants a universal fixed percentage of EXP or mesos across every build and map.

Existing characters can remain on older pinned content. Their formulas, rewards and skill behavior may differ. Installing a new APK does not automatically adopt content 1.19: each existing character chooses **Review content update → Back up & upgrade**. Export a complete account backup from Settings before updating, and install over the existing app without uninstalling or clearing data.

Use the guide alongside the game's **Compare**, **Maps**, **Plan supplies** and skill-impact views. Those views account for the build, map, attack policy and supplies you are considering.

- [What hourly rates mean](#what-hourly-rates-mean)
- [All 35 factors and damage formulas](#all-35-factors-and-damage-formulas)
- [Encounters, movement, rewards and resources](#encounters-movement-rewards-and-resources)
- [How estimates and comparisons work](#how-estimates-and-comparisons-work)
- [All 94 skills by job](#all-94-skills-by-job)
- [Practical limits](#practical-limits)

## What hourly rates mean

The engine schedules attacks, buff casts, incoming attacks, travel, spawns and periodic recovery. It resolves misses, damage lines, criticals, procs, target health, drops and resource consumption at those event times. It prioritizes the current target and wounded monsters while clearing an encounter. The visible sprite count is not the simulation's target count.

For the actually simulated grinding interval `T` in milliseconds:

- `EXP/h = gained EXP × 3,600,000 / T`.
- `Gross mesos/h = monster-dropped mesos × 3,600,000 / T`.
- `Net buying every supply/h = (monster mesos + automatic-sale proceeds − replacement cost of consumed supplies) × 3,600,000 / T`.
- `Net after supply drops/h` charges only consumed quantities not replaced by matching retained drops. A supply automatically sold is not also counted as a free replacement. Surplus unsold items and quest turn-in rewards have no assigned income value in this rate.
- Throwing-star cost uses the per-charge recharge price, not the cost to buy a new stack. Non-shop reagents can have zero priced cost; their acquisition time is explicitly outside net mesos and must be considered separately.
- Item farming uses the encounter-specific kill/Steal frequencies and actual target drop probabilities. A shared global cosmetic roll is kill-only; Steal never rolls that pool. Equipment, material and scroll map modifiers do not multiply global NX or quest drop odds.

`T` is active grinding time, not necessarily the requested wall-clock session. A stopped sample includes a stop reason; its rate does not promise that an injured or undersupplied live character will sustain an uninterrupted hour. Boss combat potential is not a promise of repeat boss reward income every minute: live challenge cooldowns, first-clear rewards and saved pending loot are separate progression rules.

## All 35 factors and damage formulas

Permanent stats start with base AP allocations and add the actual rolled stats and scroll bonuses of worn real gear. NX cosmetics, hair, skin and face never add combat stats. Requirements use retained permanent real-gear bonuses, excluding the candidate and displaced pieces; being eligible to wear a candidate is checked afresh, each time you consider equipping it.

| # | Factor | Effect and important conditions |
| --- | --- | --- |
| 1 | STR | Main physical stat for ordinary melee, secondary for bows/crossbows, and part of thief secondary damage with DEX. Adds `floor(STR/4)` physical defense in complete skill books. Weapon factors, defense and casts per kill determine the gain. |
| 2 | DEX | Main bow/crossbow damage stat, secondary ordinary-melee stat, and part of thief secondary damage with STR. Contributes to physical accuracy and `floor(DEX/6)` evasion. Accuracy stops improving hit chance at 100%. |
| 3 | INT | Main spell stat; adds `floor(INT/2)` MATK and `floor(INT/4)` magic defense, and affects magic accuracy. Element, monster defense, mastery, MP cost and target density all matter. |
| 4 | LUK | Main claw/dagger damage stat; contributes to accuracy, `floor(LUK/3)` evasion and Heal's damage expression. Weapon skill, criticals, hit caps and target type affect its value. |
| 5 | Weapon attack | Multiplies physical damage. Compatible real gear and a selected, available throwing star can contribute attack. It is different from Attack Power; unarmed recovery-field practice uses a separate fallback. |
| 6 | Attack Power | Adds a term inside the physical damage bracket, commonly `AttackPower/50`; close bow knockback uses `/150`. It is not the same as adding that many points of weapon attack. |
| 7 | MATK | Comes from INT, real equipment and applicable skill/potion bonuses. Improves spells, magic damage over time and magical retaliation, but not an ordinary physical wand swing. |
| 8 | Mastery | Raises the low end of damage rolls when the weapon matches. Lucky Seven uses its own 0.5 mastery override; other mastery bonuses can still apply. |
| 9 | Critical chance and damage | Change the chance and extra damage of critical hits; critical chance is capped at 95%. Overkill and recovery, bleed or retaliation interactions prevent a fixed gain in kills. |
| 10 | Physical accuracy | Used by physical attacks against monster avoidance and the level deficit. Its value changes with enemy debuffs and disappears once hit chance reaches its cap. |
| 11 | Magic accuracy | A separate, INT-based score for magical attacks. Monster avoidance, level difference and applicable debuffs still matter. |
| 12 | Evasion | Reduces incoming hit probability using monster accuracy and both levels. It is not flat damage reduction. Successful evasion can trigger Nimble Recovery. |
| 13 | Physical defense | Reduces physical/contact damage through the armor formula below, including its minimum-damage floor. Incoming frequency, evasion and rounding govern potion savings. |
| 14 | Magic defense | Uses the corresponding armor path against magical incoming moves. More physical defense cannot substitute for it against those moves. |
| 15 | Maximum HP and MP | Affect survival, refill thresholds, percentage recovery, absorption caps and Magic Guard reserves. They do not directly multiply EXP; larger refills can waste more potion healing. |
| 16 | Restoration and recovery | Potion, Heal and passive-recovery bonuses restore resources up to the maximum. Overhealing is wasted. Heal's damage is undead-only; MP Eater is limited by enemy MP and its lockout. |
| 17 | Shield guard | A worn shield gives `max(0.05, shieldDefense/(shieldDefense+500))` guard probability on the supported contact-hit path. A successful guard prevents that hit, separately from evasion. |
| 18 | Knockback resistance | Avoids the modeled attack delay from supported incoming hits, on applicable warrior/dagger paths. It does not directly increase attack speed when no such hit occurs. |
| 19 | Stun, slow and contact blocking | Prevent or delay eligible enemy actions. Duration, immunity, target state and incoming attack type can make their benefit smaller or zero. |
| 20 | Speed | Changes horizontal route travel, clamped to 50–140. It does not shorten climbing or remove waits for monsters to spawn. |
| 21 | Jump | Remains on source gear and buffs, but the current idle simulation has no manual jumping or grinding-rate calculation using it. No EXP bonus is attributed to Jump. |
| 22 | Attack timing | Weapon, skill and Booster timing determine milliseconds per action, generally in 30 ms steps. Buff casts, travel, incoming knockback, cooldowns and follow-ups also consume time. |
| 23 | Range | Affects reach, route coverage and target eligibility. Range alone neither adds targets nor increases raw damage; direct Disorder and Steal do not gain claw ranged-travel coverage. |
| 24 | Targets and damage lines | Determine eligible monsters hit per cast and separately resolved damage lines. Extra targets help only when living, eligible targets exist; kill thresholds and overkill matter. |
| 25 | Element | Weakness uses 1.25×, neutral 1×, resistance 0.75× and immunity 0×. Numeric relations are bounded to 0–1.25; status immunity is checked separately. Heal requires undead targets. |
| 26 | Monster properties | HP, level, defenses, avoidance, accuracy, attack power, MP, moves, undead status and immunities affect kills, damage taken and supply needs. |
| 27 | Spawns and routes | Map capacity, spawn ticks, individual respawn cooldowns, encounter groups and horizontal/climbing edges set a throughput ceiling. An empty map waits for spawns rather than inventing monsters. |
| 28 | Potions and supplies | Chosen HP/MP potions, refill thresholds, restoration bonuses and overheal change costs. Timed attack potions and optional automatic renewal also consume stock and affect net income. |
| 29 | Buff policy | Automatic priority, resource rules, duration, cooldown and casting time control uptime. In 1.19, the strongest same-stat skill bonus adds to the strongest potion bonus; same-pool bonuses do not all stack. |
| 30 | Attack policy | Selected skill, monster-count rules, fallback, Final Attack, ammunition and throwing-star choice change damage, targets, timing and resource demand. |
| 31 | RCed solo balance | Versioned job/level damage, MP, boss, multi-target and skill-specific factors adapt source mechanics to solo idle play. These adjustments are distinct from confirmed source values. |
| 32 | Rewards | Monster rewards, map profiles, overlevel reductions, item probabilities, quest conditions and the active interval of an EXP coupon all affect actual gains. |
| 33 | Net supply costs | Monster mesos and future automatic-sale proceeds are reduced by consumed-supply replacement costs. Matching retained drops can offset use; surplus unsold loot has no assigned cash value. |
| 34 | Inventory | Actual stock and bag room affect session duration and retained drops. Controlled comparisons use plentiful supplies and unlimited item room, so they do not predict a full bag's retained loot. |
| 35 | Cosmetics | NX equipment, hairstyle, face and skin change appearance only. They add no combat stats or grinding-rate bonus. |

### Physical damage

The ordinary weapon range uses approximately these **pre-monster** expressions, retaining rounding and the applicable weapon/skill branches. Here `W` is effective weapon attack, `floor` rounds downward and `clamp` bounds a value between the stated minimum and maximum:

`low = floor(W × [0.8 + (P × mastery × lowWeaponFactor + S)/100 + AttackPower/50])`

`high = floor(W × [1 + (P × highWeaponFactor + S)/100 + AttackPower/50])`

`P/S` are STR/DEX for ordinary melee, DEX/STR for bow/crossbow, and LUK/(STR+DEX) for claw/dagger. Weapon factors and special skill rules determine the actual calculation; this shorthand is not a substitute for close-bow, fixed-damage, Lucky Seven, swing/stab or critical branches. Ordinary melee swing/stab is modeled with its source 60%/40% distribution. Skills can replace factors, add damage lines, force criticals, ignore defense or apply target attenuation.

Physical monster scaling is `100/(effective monster defense+100) × levelScale`. Threaten/Disorder can reduce effective defense. With positive level deficit `g`, `levelScale` is 1 for `g=0`, `1/(1+0.005g²)` below 10, and `1/(1+0.05g)` from 10 onward. The pinned solo damage policy applies job/level, boss, multi-target and skill-specific factors. Fixed Three Snails damage takes its own branch.

### Spell damage

For ordinary spells, the raw line is shown below; `roll` is the sampled position between the low and high ends of the damage range:

`magicPower/100 × MATK × (1 + INT × [mastery + (1−mastery)×roll]/125)`

Spell mastery is `(masteryLevel/10+0.1)×0.7`. Monster scaling is `100/(magicDefense+100) × elementFactor × levelScale`; solo policy and critical/event branches apply afterward. Element factors are neutral 1, weak 1.25, resistant 0.75, immune 0. Numeric source relations are clamped to 0–1.25. Status effects separately require a nonimmune target and an allowed element relation.

Heal uses its own source expression, damages undead only and shares its target pool with the caster. Its published damage model is marked unconfirmed and solo HP recovery is an explicit adaptation. Magic DoTs use their separate MATK/INT/power expression; recasting refreshes duration without multiplying simultaneous DoT damage and retains a stronger existing application. Axe bleed also has a separate, defense-ignoring STR/DEX/Attack Power expression. These branches are recorded in the corresponding skill rows.

### Hit, incoming damage and defense savings

For an outgoing attack, let `g=max(0, monsterLevel−playerLevel)`, `a=chosenAccuracy×100/(10g+255)`, and `e=effective monster avoidance`. A sufficiently large `a−e` saturates to 100%; otherwise the game uses a logistic-width hit calculation and bounds the final probability to 0–1. Magic attacks use `magicAccuracy`, and Slow can reduce enemy evasion. The chosen score and level deficit must therefore be evaluated together.

For current physical mitigation, with raw hit `R`, defense `D`, player level `L`, monster level `M`:

`legacy = R×(1−D/(D+300+2R)) − (D/25+L/10)`

`armorBand = clamp(exp((5M−D)/125), 0.35, 1.25)`

`damage = max(1, floor(max(0.15R, legacy×armorBand)))`

Magical moves substitute magic defense. Contact-specific and general mitigation apply after this step; evasion and shield guard can prevent a hit, and Magic Guard transfers a share of remaining damage to available MP. Raw monster damage uses its physical/magic attack and source move power, with the scheduler's random 1.2–1.4 factor. Incoming frequency, stun/slow/contact block, monster MP, route travel and attack moves all matter. Consequently “+4 defense” has no fixed universal mesos saving; it must be evaluated against the chosen map and supply policy. Old pinned packs retain their original defense arithmetic.

## Encounters, movement, rewards and resources

The route follows the forward circuit and clears a sector before moving. Each crossed edge costs:

`round(horizontalMs × 100/clamp(speed,50,140) × 300/(300+effectiveRangeBonus)) + climbMs`

Teleport can shorten a beneficial edge at a per-use MP cost and modeled action floor. Direct Disorder/Steal strikes do not gain ranged travel coverage from claw range. An empty map waits for its next spawn rather than inventing extra mobs. Capacity, spawn ticks, per-point respawn cooldowns, route groups, target type and total monster HP create the throughput ceiling. Increasing targets, attack speed or damage past that ceiling can leave EXP unchanged.

Monster EXP and mesos are source rewards modified by the map's reward profile and overlevel policy, with integer rounding. Profiles independently alter EXP, mesos and selected equipment/material/scroll probabilities; maps are not forced to sum to a universal “one point of value.” Fixed boss purses have their explicitly scoped exemption. Double-EXP coupons multiply eligible EXP only while active; additional coupons extend duration rather than create 4× or 8×.

HP/MP potion selection, threshold, restoration bonuses, overheal, automatic buff order, resource fallback and star choice change supply demand. Running out of a required reagent can change the chosen attack or stop a live session. Forecast benchmarks deliberately use plentiful resources; the supply planner overlays actual carried quantities afterward, includes a 25% reserve, respects whole-basket capacity and distinguishes non-shop shortages. Full inventory in current packs preserves EXP/mesos while skipping item drops that cannot fit; benchmark inventory room is unlimited and does not predict actual retained loot in a full bag.

Warrior Potion and Magic Potion add a separate potion buff pool. In 1.19, the strongest positive same-stat **skill** bonus and strongest same-stat **potion** bonus are added together; multiple skill buffs of that stat or multiple potions of that stat do not multiply the pool. Permanent equipment/passive bonuses remain separate, and the strongest skill penalties are retained. Automatic attack potions are a saved combat policy, not an assumption that a manually activated live potion lasts forever. Timed potion use/cost appears in supply and net metrics.

## How estimates and comparisons work

The result depends on the combination of build, map and policy. The game can reuse unchanged equipment stats, skill ranks, timing, spawn information and prices, but it cannot attach a reliable universal “adds 8% EXP” label to an item. Accuracy caps, kill thresholds, travel, density and costs make the combined result nonlinear.

### What refreshes an estimate

Estimates respond to the character's content version, level, job, allocated stats, maximum resources, learned ranks, real worn equipment and its rolls/scroll bonuses. The selected attack or star, recovery potions and thresholds, fallback, automatic-buff order and resource rules, Final Attack, monster-count rules, automatic attack potions and applicable auto-sell/protection rules also matter. Each map has its own result. Changing characters or importing a save prevents an old calculation from appearing for the wrong adventure.

Ordinary EXP progress, current HP/MP, the current monster's remaining HP, random outcomes, remaining stock and a live buff's age do not continually restart the controlled benchmark. The benchmark deliberately starts from the same conditions. Actual stock, affordability, bag space, active EXP-coupon time, item ownership, equipment eligibility and available SP are checked separately when relevant. Appearance, music and reduced motion do not change combat estimates.

### Map forecasts

Hunt's current map is prepared first, followed by accessible primary routes in the background, even while World Map is closed. Results appear as they finish. Ordinary alternatives exclude boss arenas; older routes are included when **Earlier Routes** is shown. Newly unlocked routes can be prepared without discarding ready estimates for the same build.

Reopening Maps uses ready results or continues the calculation already underway. Closing the overview does not cancel the remaining work. If a map estimate fails, it offers an explicit retry instead of displaying a fabricated zero or restarting endlessly. A changed build refreshes the relevant results.

### Comparing gear, skills, AP and scrolls

Equipment facts, skill ranks and immediate stat changes can appear while the first hourly calculation is still pending. Compatible comparisons share an unchanged baseline, and reopening a comparison can reuse its ready rates. Eligibility, price, ownership and available SP are always checked again; an old rate never authorizes an unavailable action.

Controlled comparisons use **five fixed 20-minute samples** with fresh encounters, full HP/MP, ready cooldowns, plentiful supplies, no live EXP boost and frozen level/equipment. The two sides use paired conditions so normal sample variation is visible. These are benchmarks, not a promise of uninterrupted play or a naturally funded progression route.

Map planning normally uses a five-minute sample. With automatic ten-minute attack potions, it uses ten minutes to cover a full buff cycle. Resource exhaustion, spawn saturation, travel and later player choices can still change actual results.

A skill already used by the saved monster-count rotation is compared within that rotation. An attack outside it uses an explicitly labeled single-attack setup on both sides so the proposed skill is actually cast. Buffs are maintained in each learned setup, and relevant triggered follow-ups are enabled for their previews. These hypothetical policy changes never alter the live character.

EXP-coupon displays apply the remaining boosted interval to the unboosted estimate. Time to next level immediately subtracts EXP already earned and accounts for coupon expiry. Current supplies, affordability and capacity are applied to live planning without pretending that the character has the benchmark's unlimited stock.

## All 94 skills by job

Each entry retains the skill's maximum rank, mechanism and major conditions. A passive works without repeated casting; a buff has the stated activation or maintenance rules; a triggered follow-up needs an eligible event. Basic Attack is a baseline action, not a trainable skill. Repeated names under different jobs are separate branch skills.

Damage over time is abbreviated **DoT**. All references to source facts, unknown source values and RCed adaptations remain explicit. Consult the in-game skill book for exact values at each rank.

### All jobs

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Basic Attack | 1 | Attack | Weapon-dependent ordinary attack. Baseline has no trainable ranks or MP cost; ranged weapons consume their configured ammunition. |

### Beginner

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Nimble Feet | 3 | Buff | Temporary movement speed reduces the horizontal portion of route travel, subject to speed bounds; duration, cooldown and casting overhead limit uptime. Cast time is modeled at 600 ms; the source does not publish its timing. |
| Recovery | 3 | Buff | Gradual HP recovery in six five-second ticks, with cooldown and casting time. Changes HP supply demand rather than raw attack damage. HP arrives in six equal five-second ticks; tick cadence and 600 ms cast time are modeled. |
| Three Snails | 3 | Attack | Fixed damage bypasses ordinary weapon/stat damage scaling. Ranks change fixed damage, MP and the required shell item; shell farming is a real resource constraint. |

### Bowman

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Arrow Blow | 20 | Attack | Single-target bow/crossbow damage multiplier changes landed damage and casts needed per monster; rank MP costs change profit. |
| Critical Shot | 15 | Passive | Bow/crossbow critical probability and critical bonus improve expected landed damage, subject to the critical cap and kill thresholds. |
| Double Shot | 20 | Attack | Two independently resolved lines on one target; rank damage and MP cost affect kill thresholds and supply use. |
| The Eye of Amazon | 15 | Passive | Bow/crossbow range bonus reduces effective horizontal route travel. It is not a direct damage or EXP multiplier. Range reduces route travel by 300 / (300 + bonus range); encounter geometry is modeled. |
| Focus | 20 | Buff | Temporary accuracy and evasion affect misses and incoming hit frequency. MP, HP, cast time and refresh duration enter costs. Evasion lowers modeled contact-hit probability; platform collision is not simulated. |
| Power Knockback | 15 | Attack | Weapon-specific close attack with rank-dependent target count, range and knockback. Bow close damage uses different stat/Attack Power divisors; contact interruption can reduce incoming damage. Uses the upper published swing timing. Knockback blocks contact for 5 ms per pixel; collision is modeled. |

### Hunter

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Amazon's Judgement | 20 | Passive | Passive landed-attack proc slows targets for a duration. Fewer incoming attacks can save HP supplies without increasing raw damage. Slow extends the affected enemy’s modeled contact interval by 100 / (100 − slow). |
| Arrow Bomb | 30 | Attack | Bow area damage with chance/duration stun. Stunned targets cannot make ordinary scheduled incoming attacks; boss/status immunity applies. The source confirms one initial projectile and a linked six-target explosion. RCed reuses the first explosion hit roll as the projectile gate: an initial miss cancels the explosion. Other targets roll independently; surviving landed targets can be stunned. The hit-roll coupling, encounter grouping and prevention of contact while stunned are explicit idle approximations; there is no separate initial-projectile damage. |
| Bow Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Bow Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Final Attack: Bow | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. RCed’s saved toggle maintains Final Attack automatically instead of manual 60-second activation. Three arrows split 3, 2+1, or 1+1+1 across available enemies. An empty encounter cancels the follow-up without spending supplies. |
| Soul Arrow: Bow | 20 | Buff | Temporary matching-weapon arrow exemption trades buff MP/casting time for ammunition savings. It does not grant permanent arrows. |

### Crossbowman

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Amazon's Judgement | 20 | Passive | Passive landed-attack proc slows targets for a duration. Fewer incoming attacks can save HP supplies without increasing raw damage. Slow extends the slowed enemy’s modeled contact interval by 100 / (100 − slow). |
| Crossbow Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Crossbow Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Final Attack: Crossbow | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. A saved toggle controls procs. If the original group is empty at execution, the follow-up is discarded without cost. |
| Iron Arrow | 30 | Attack | Up to six crossbow targets; each successive target takes the configured 0.8 attenuation. Extra targets only help when living targets exist in the encounter. |
| Soul Arrow: Crossbow | 20 | Buff | Temporary matching-weapon arrow exemption trades buff MP/casting time for ammunition savings. It does not grant permanent arrows. |

### Warrior

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Improved HP Recovery | 15 | Passive | Periodic max-HP-based passive regeneration plus improved HP potion restoration reduces supply demand; no direct damage multiplier. Source confirms continuous 10-second HP regeneration but does not publish the amount. RCed regenerates 1% of effective maximum HP per tick. Potion healing bonus uses the exact published rank. |
| Iron Body | 20 | Buff | Temporary defense improves physical mitigation; casting cost and uptime determine net HP savings. |
| Max HP Increase | 15 | Passive | Raises derived maximum HP, affecting survivability, threshold refills and percentage-based recovery; no direct attack damage bonus. |
| Power Strike | 20 | Attack | Weapon-based direct attack with rank damage and target-count changes. Weapon swing/stab rules, MP cost and action timing apply. |
| Precise Strikes | 15 | Passive | Passive accuracy and critical chance improve hit and critical outcomes, subject to caps. |
| Slash Blast | 20 | Attack | Area weapon attack with HP/MP costs and rank-dependent damage/range; nearby target availability limits benefit. |

### Fighter

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Axe Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Axe Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Final Attack: Axe | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Final Attack: Sword | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Rage | 30 | Buff | Temporary Attack Power raises the additive term inside weapon damage; defense penalty can increase HP spending. Skill and potion bonus pools stack in 1.19. |
| Rush | 20 | Attack | Cooldown-limited multi-target attack with range and knockback. Basic attack can fill its cooldown; travel and encounter count govern usefulness. Encounter displacement and grouping model the source rush/knockback; no physical platform collision is simulated. |
| Sword Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Sword Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |

### Page

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Blunt Weapon Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Blunt Weapon Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Final Attack: Blunt Weapon | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Final Attack: Sword | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Rush | 20 | Attack | Cooldown-limited multi-target attack with range and knockback. Basic attack can fill its cooldown; travel and encounter count govern usefulness. Encounter displacement and grouping model the source rush/knockback; no physical platform collision is simulated. |
| Sword Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Sword Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Threaten | 30 | Buff | Recast defense-reduction/slow debuff on up to the configured encounter targets. Raises outgoing physical damage and reduces incoming cadence when not immune; costs cast time and MP. Applies the source defense reduction and slow to up to four living encounter targets; recast automation is an idle adaptation. |

### Spearman

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Final Attack: Polearm | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Final Attack: Spear | 30 | Triggered follow-up | An enabled matching-weapon proc after an eligible trigger schedules one extra action with its own timing and resources. It cannot trigger itself; an empty encounter cancels it. Spear/polearm versions can heal; source triggers and targets vary by weapon. Saved automatic Final Attack toggle models the source 25% activation and uses one follow-up with its own resources and animation. It cannot trigger itself; an emptied encounter cancels the follow-up. |
| Iron Will | 30 | Buff | Temporary flat defense and knockback resistance improve physical mitigation and reduce incoming-hit attack delays. No direct EXP multiplier. |
| Polearm Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Polearm Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Rush | 20 | Attack | Cooldown-limited multi-target attack with range and knockback. Basic attack can fill its cooldown; travel and encounter count govern usefulness. Encounter displacement and grouping model the source rush/knockback; no physical platform collision is simulated. |
| Spear Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Spear Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |

### Thief

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Dark Sight | 20 | Buff | Travel concealment ends before attacking. Current routes already suppress incoming contact while traveling, so automatic use can add MP/cast cost with zero defensive benefit; it stays off by default. Automatic Dark Sight is used only while moving between encounters and is cancelled before attacking. Current idle routes already suppress incoming damage during movement, so enabling it can add MP and cast-time costs without improving rates. It stays off by default. The source is an indefinite toggle; the stored one-day duration is an internal cap, not a source rank duration. It never permits attacking while invulnerable. |
| Disorder | 20 | Attack | Direct weapon strike applies temporary enemy attack and defense reduction. Claw users pay no stars for this close strike; proc/status rules remain conditional. Source weapon-dependent reach is 60–133px. RCed uses a fixed 86px encounter reach and applies its attack/defense debuff only on a successful hit. |
| Double Stab | 20 | Attack | Two-line dagger attack; rank damage and MP alter per-monster kill thresholds and profit. |
| Keen Eyes | 15 | Passive | Claw range bonus reduces route movement; direct Disorder/Steal strikes do not inherit that ranged movement bonus. |
| Lucky Seven | 20 | Attack | Two-star, two-line claw attack with its own weapon multiplier and fixed 0.5 mastery override. Claw mastery still contributes its other bonuses. |
| Nimble Body | 15 | Passive | Passive accuracy and evasion alter hit/miss outcomes, with no resource cost. |

### Assassin

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Claw Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Claw Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Critical Recovery | 20 | Passive | Chance-based HP/MP recovery on critical attack events, with a 30-second internal lockout and max-resource percentages. |
| Critical Throw | 30 | Passive | Claw critical probability/bonus improves landed damage; critical recovery can interact with successful criticals. |
| Drain | 30 | Attack | Claw attack with chance-based life steal, limited by dealt damage, target maximum HP and the character HP cap. Can reduce HP potion cost at the expense of MP/stars. |
| Haste | 20 | Buff | Temporary speed reduces horizontal travel; source timing/cost and refresh uptime apply. Jump is retained as a source stat but has no current grinding calculation. Speed affects encounter travel time. Jump is retained as a source bonus; this idle simulation has no manual platform-jump controls. |

### Bandit

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Dagger Booster | 20 | Buff | Matching-weapon attack speed changes to the source boosted timing table. Refresh casts and HP/MP cost consume time/resources; it does not multiply damage. |
| Dagger Mastery | 20 | Passive | Matching-weapon mastery raises the lower damage bound. Other rank bonuses depend on the weapon and can include accuracy, criticals, speed, bleed, defense bypass, star retrieval or knockback resistance; not every mastery grants every bonus. |
| Haste | 20 | Buff | Temporary speed reduces horizontal travel; source timing/cost and refresh uptime apply. Jump is retained as a source stat but has no current grinding calculation. Speed affects encounter travel time. Jump is retained as a source bonus; this idle simulation has no manual platform-jump controls. |
| Nimble Recovery | 20 | Passive | Chance-based HP/MP recovery on evasions, with a 30-second internal lockout. More evasion can make it trigger more often. |
| Savage Blow | 30 | Attack | Dagger attack whose line count changes with rank; each line and action cost participates in kill thresholds and proc interactions. |
| Steal | 30 | Attack | Up to two direct strikes; one successful theft per spawn makes at most one additional ordinary item-table attempt, with stun and temporary Attack Power. Grants no theft EXP/mesos and never rolls the global NX pool. A successful theft makes one additional attempt at the monster item-drop table, takes at most one item, grants no EXP or mesos, and can succeed once per spawn. Source does not publish item-selection odds; using RCed drop probabilities is an explicit idle adaptation. Quest conditions and full-bag skipping still apply. Source permits any weapon: claws can use this direct physical strike without consuming stars; RCed keeps their equipped star attack bonus and fixed swing multiplier 1. |

### Magician

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Energy Bolt | 20 | Attack | Neutral single-target magic power/mastery attack using MATK and INT, magic accuracy and enemy magic defense. |
| Improved MP Recovery | 15 | Passive | Periodic maximum-MP recovery and improved MP potion restoration reduce MP demand; no raw spell damage bonus. |
| Magic Armor | 20 | Buff | Temporary physical and magic defense bonuses reduce incoming damage through the corresponding defense calculation. |
| Magic Claw | 20 | Attack | Neutral two-line magic attack using MATK and INT, magic accuracy and enemy magic defense. |
| Magic Guard | 15 | Buff | Transfers a rank percentage of incoming damage from HP to available MP; it is resource conversion, not free damage immunity. Source toggle is stored with a one-day internal duration for idle automation; this is not a source duration. Damage transfer is limited by available MP, with the remainder paid as HP. |
| Max MP Increase | 15 | Passive | Increases derived maximum MP; changes reserve, threshold refills, percent recovery and Magic Guard capacity, not raw spell power. |

### Fire/Poison Wizard

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Fire Arrow | 30 | Attack | Fire direct magic damage plus conditional magic DoT; enemy element/status relations and DoT refresh rules apply. Source burn is a three-second effect at one-second intervals. The data lists 100% application; live status resistance is unresolved. RCed applies it after a successful hit unless the target is resistant, immune or status-immune. Reapplication refreshes rather than stacks. |
| Meditation | 20 | Buff | Temporary MATK bonus improves spells and magic DoTs. Strongest same-stat skill bonus stacks with the strongest potion bonus in 1.19. Party effects apply to the active solo character; independent characters are not a combat party. |
| MP Eater | 20 | Passive | Chance to absorb a fraction of enemy MP on eligible magic hit, limited by enemy remaining MP and a five-second lockout; saved MP changes net profit. |
| Poison Breath | 30 | Attack | Poison direct damage plus conditional magic DoT; a stronger active DoT is retained rather than multiplied by rapid recasts. Source explosion hits at most six targets, including the acquired target. Poison lasts five seconds at one-second intervals. Live status resistance is unresolved; RCed honors elemental/status immunity. Reapplication refreshes rather than stacks. |
| Slow | 20 | Buff | Recast enemy speed/evasion debuff reduces incoming frequency and may improve hit chance. Target, duration and immunity conditions apply. Movement speed and evasion reductions affect living encounter targets. They do not refresh an existing Slow. Route and enemy-action timing are idle abstractions. |
| Teleport | 20 | Buff | Optional travel automation spends MP per beneficial route hop to shorten travel, with a modeled 150ms floor. Technical toggle duration is not an ordinary repeated casting cost. Source distance and MP cost are verified; source cast timing is unavailable. RCed treats Teleport as optional travel automation with a 150 ms action floor, paying MP per use only when it shortens the route. Enabling the one-day technical toggle itself has no MP cost. |

### Ice/Lightning Wizard

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Cold Beam | 30 | Attack | Ice direct damage and action slow, subject to elemental and status immunity; reduced incoming pressure can lower HP consumption. Source gives a three-second slow without a quantified action-speed penalty. RCed uses a 30% action slow for non-resistant, non-immune targets; this value is a disclosed idle balance parameter. |
| Meditation | 20 | Buff | Temporary MATK bonus improves spells and magic DoTs. Strongest same-stat skill bonus stacks with the strongest potion bonus in 1.19. Party effects apply to the active solo character; independent characters are not a combat party. |
| MP Eater | 20 | Passive | Chance to absorb a fraction of enemy MP on eligible magic hit, limited by enemy remaining MP and a five-second lockout; saved MP changes net profit. |
| Slow | 20 | Buff | Recast enemy speed/evasion debuff reduces incoming frequency and may improve hit chance. Target, duration and immunity conditions apply. Movement speed and evasion reductions affect living encounter targets. They do not refresh an existing Slow. Route and enemy-action timing are idle abstractions. |
| Teleport | 20 | Buff | Optional travel automation spends MP per beneficial route hop to shorten travel, with a modeled 150ms floor. Technical toggle duration is not an ordinary repeated casting cost. Source distance and MP cost are verified; source cast timing is unavailable. RCed treats Teleport as optional travel automation with a 150 ms action floor, paying MP per use only when it shortens the route. Enabling the one-day technical toggle itself has no MP cost. |
| Thunder Bolt | 30 | Attack | Lightning area magic damage and conditional stun. Target density/route geometry and immunity strongly affect throughput. Source data lists a two-second stun and six-target cap. Live final status resistance is unresolved. RCed honors elemental resistance and boss/status immunity. |

### Cleric

| Skill | Maximum rank | Type | Effect and conditions |
| --- | ---: | --- | --- |
| Bless | 20 | Buff | Temporary general damage reduction and enhanced Heal recovery improve survival and supply efficiency; no physical/magic accuracy or evasion bonus is granted by these current rank rows. Party effects apply to the active solo character; damage reduction is distinct from Invincible contact protection and Magic Guard resource transfer. |
| Heal | 30 | Attack | Restores caster HP and damages undead only, sharing its source target pool. Mixed maps need a non-Heal fallback. Published damage and modeled solo healing assumptions are retained in definition provenance. Solo Heal reserves one of six shared slots for the caster, leaving five undead targets. Undead damage is non-elemental and uses the separately labeled source-model formula. Source HP recovery amount is unresolved: RCed restores maximum HP times the sourced recovery rate, multiplied by active Bless. This explicit adaptation is tested separately from damage. |
| Holy Arrow | 30 | Attack | Holy single-target magic attack; enemy holy weakness, resistance or immunity modifies damage. |
| Invincible | 20 | Buff | Temporary contact mitigation plus configured contact retaliation. Physical/magic moves and reflect immunity are distinct; no blanket invulnerability. Reduction applies to monster contact only, not physical attack moves or magic attacks. Contact retaliation uses INT and magic attack, not the amount of damage received. |
| MP Eater | 20 | Passive | Chance to absorb a fraction of enemy MP on eligible magic hit, limited by enemy remaining MP and a five-second lockout; saved MP changes net profit. |
| Teleport | 20 | Buff | Optional travel automation spends MP per beneficial route hop to shorten travel, with a modeled 150ms floor. Technical toggle duration is not an ordinary repeated casting cost. Source distance and MP cost are verified; source cast timing is unavailable. RCed treats Teleport as optional travel automation with a 150 ms action floor, paying MP per use only when it shortens the route. Enabling the one-day technical toggle itself has no MP cost. |

## Practical limits

- This guide applies to **content 1.19.0 in app 0.23.0**. Older pinned packs keep their own arithmetic and progression rules. The app's visual and performance updates do not automatically opt a character into new gameplay content.
- Confirmed source rank values and item statistics are used where available. Unpublished timings, solo healing, encounter grouping, selected status behavior and other idle adaptations are identified in the relevant explanations. An unresolved source value is not presented as confirmed.
- RCed models routes, timing and encounters; it does not simulate a full platform game's collision geometry, projectile paths, manual jumping or every original multiplayer interaction. Party effects here apply to the active solo character; separate character slots are not a combat party.
- Hourly results are finite simulations under stated conditions. They are neither guaranteed drop deadlines nor fixed bonuses for every point or item. Stock, bag space, enemy composition, spawn limits, changing builds and manual actions can change real outcomes.
- Boss cooldowns, first-clear entitlements, pending rewards and quest turn-ins remain separate from ordinary continuous-grinding rates. A boss's combat potential does not imply that its purse can be collected repeatedly without waiting.
- Performance improvements do not establish a guaranteed phone frame rate, battery life or touch latency. A completed synthetic estimate is not evidence of a natural level-one progression playthrough.

[Return to the main game page](https://github.com/iRCed7/rced-idle-releases) · [Download the latest release](https://github.com/iRCed7/rced-idle-releases/releases/latest)
