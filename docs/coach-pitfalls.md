# Common coaching mistakes

**Match fetch:** Never hand-roll long `curl` chains. Run `scripts/fetch_lol_match.py` once with `RIOT_API_KEY` (routing, ranked SR defaults, 429 retries).

**Item names:** Resolve IDs only via `items.json` from the export (or Data Dragon). If missing: `Unknown item (ID: XXXX)` – never guess from memory.

**Smite:** Only the jungler has Smite. If `ELITE_MONSTER_KILL` killer is not jungle, say they **secured** or **last-hit** the objective – not “landed Smite.”

**Counterplay:** Before “dodge this ability,” check whether the analyzed champion’s kit answers it (e.g. Braum **E** vs MF **R** – stand in channel with **E**, don’t only “dodge”).

**Deaths in lane phase (0–14 min) vs. lane matchup:** If the player dies repeatedly (3+ times) before 14 minutes to their direct lane opponents, do not reduce it to a generic “positioning” note. Contextualize it: identify the lane matchup, explain *why* that matchup is inherently dangerous (e.g. long-range poke champions like Caitlyn/Lux have strong kill threat in lane and punish champions with shorter range or less mobility like Zyra/Smolder), and frame the coaching around *lane-phase fundamentals* – wave management, trading windows, when to play safe vs. aggressive, how to minimise kill threat in that specific matchup. A finding like “died 4 times to Caitlyn/Lux” should explain the kill range and poke threat of that duo and what lane-phase adjustments address it.

**Itemization critique:** Before calling an item wrong: (1) Skill Capped guide for champ/role (see `docs/lol-reference.md`), (2) enemy comp (heal → GW, CC → Mikael’s, AoE → Locket). **Grievous Wounds** applies on any damaging hit – do not dismiss anti-heal because the buyer is “low damage”; critique timing/sequencing instead. For timing critiques (e.g. “buy this earlier”), avoid prescribing exact backs – item timing is highly contextual (gold on hand, recall timing, death timing, power-spike urgency). Prefer: “could have prioritized this earlier given the comp” over “should have bought this on first or second back.”

**Support quest item evolutions (Celestial Opposition / Zaz’Zak’s Realmspike / Vigilant Wardstone / Dreamcatcher / etc.):** These items are obtained by completing the support quest, not by purchasing outright. Do NOT critique the player for “choosing” a quest evolution item as their first purchase – they didn’t choose to spend gold on it. The only valid critique here is which evolution they picked, if it mismatches their kit (e.g., picking Dreamcatcher on a champion with no heals/shields to proc its passive).

**Champion stats:** For ranges/CDs/damage numbers, use wiki or Data Dragon – not training-data recall.

**Objective steal attempts (Baron, Dragon, Rift Herald, Void Grubs):** When a player dies in a neutral objective pit shortly before or as the objective is secured, assume it was a deliberate steal attempt – not random aggression – and evaluate it as such. Do not label it as incompetence without checking the steal conditions.

Steal attempt viability framework:
- **Favorable conditions (closer to 50/50):** team is losing badly and needs a miracle, both junglers are similar level (equal smite damage), enemy team has low burst at the objective so they can't rush it faster than smite timing
- **Unfavorable conditions (bad attempt):** stealer's smite deals less damage (outleveled), stealer has no smite (non-jungler last-hitting), winning team's burst damage (e.g. a fed mage/ADC in the pit) can finish the objective before smite window opens
- If the stealing team is losing hard AND junglers are similar level AND enemy has no extreme burst in pit → correct instinct, coin-flip execution
- If any unfavorable condition applies → poor risk/reward; coaching should identify which condition broke the steal math
