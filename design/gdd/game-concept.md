# Game Concept: Smile & Devour

*Created: 2026-04-28*
*Status: Draft*

---

## Elevator Pitch

> It's a roguelite auto-battler where you play as a tiny slime, absorbing every
> enemy you touch to evolve your color, powers, and form — growing from the
> weakest creature in the world to its unstoppable apex predator, one run at a time.

---

## Core Identity

| Aspect | Detail |
| ---- | ---- |
| **Genre** | Roguelite auto-battler / survivor |
| **Platform** | Web / Browser (WebGL) |
| **Target Audience** | Mid-core roguelite fans + anime aesthetic players |
| **Player Count** | Single-player |
| **Session Length** | 10–20 minutes per run |
| **Monetization** | None planned for MVP |
| **Estimated Scope** | Small (2–6 weeks, solo) |
| **Comparable Titles** | Vampire Survivors, Brotato, 20 Minutes Till Dawn |

---

## Core Fantasy

You start as the smallest, weakest thing on the screen — a tiny white blob.
Everything wants to kill you. But every enemy you absorb makes you slightly
more dangerous, slightly more colorful, slightly more *yours*. By the end of
a run, the screen is filled with cascading color, your slime is glowing with
the DNA of dozens of defeated enemies, and you are the thing everything else
should be afraid of. The fantasy is the arc itself: zero to apex, earned
through absorption, expressed through color.

---

## Unique Hook

It's like Vampire Survivors, AND ALSO every enemy type you absorb shifts your
slime's color aura and unlocks a new passive ability variant — so no two runs
ever look or play the same, and your slime's appearance is a live readout of
every choice you made.

---

## Visual Identity Anchor

**Selected Direction: Pop Anime Burst**

*One-line visual rule:* Every element is drawn, animated, and colored as if it
belongs in a high-energy anime opening — exaggerated, expressive, and immediately readable.

**Supporting visual principles:**

1. **Silhouette first** — Every enemy and the slime itself must be instantly
   readable as a silhouette at any size. If the shape isn't clear, redesign it.
   *Design test:* Convert any sprite to black — can you still tell what it is?

2. **Color = identity** — Enemy types each own a distinct hue. The slime's aura
   is always the blended result of what it has absorbed. Color is the UI.
   *Design test:* Cover all text and icons — can a player still understand what's
   happening from color alone?

3. **Everything bounces** — Idle animations, hit reactions, absorption VFX, UI
   elements — all use squash-and-stretch. Nothing is static.
   *Design test:* Play a 10-second clip with the sound off — does it still feel alive?

**Color philosophy:** The world palette is desaturated and cool (greens, greys,
dark purples) so the slime's ever-brightening aura pops against it. The slime
is always the most colorful thing on screen.

---

## Player Experience Analysis (MDA Framework)

### Target Aesthetics (What the player FEELS)

| Aesthetic | Priority | How We Deliver It |
| ---- | ---- | ---- |
| **Fantasy** (power escalation, identity) | 1 | Zero-to-apex arc; visual evolution of the slime |
| **Challenge** (mastery, skill expression) | 2 | Enemy type prioritization; absorption synergy decisions |
| **Expression** (self-expression) | 3 | Every run produces a unique color combination and build |
| **Sensation** (sensory pleasure) | 4 | Magnetic pop VFX, color shift, squash-and-stretch animations |
| **Discovery** (emergent systems) | 5 | Finding color synergy combos through experimentation |
| **Narrative** | N/A | Not a narrative game |
| **Fellowship** | N/A | Single-player only |
| **Submission** | N/A | Not a relaxation game |

### Key Dynamics (Emergent player behaviors)

- Players will start prioritizing specific enemy types over others to build toward
  a color/ability combination they want
- Players will experiment with absorption order to discover synergy combos
- Players will replay runs specifically to try a different color/type path
- Players will share screenshots of their final run state (the slime's unique color)

### Core Mechanics (Systems we build)

1. **Magnetic absorption** — proximity to enemies triggers a pull force; contact
   triggers absorption with a satisfying pop VFX and color shift
2. **Color-aura evolution** — each enemy type maps to a hue; absorbing enemies
   blends the slime's aura toward that hue and unlocks ability variants
3. **Wave escalation** — enemy density and type complexity increases over time,
   forcing the player to make faster absorption-priority decisions
4. **Level-up upgrade selection** — wave clears award a choice of 1 from 3 random
   upgrades drawn from the 5-upgrade pool
5. **Boss encounter** — end-of-run elite enemy requiring the player's accumulated
   abilities to survive

---

## Player Motivation Profile

### Primary Psychological Needs Served

| Need | How This Game Satisfies It | Strength |
| ---- | ---- | ---- |
| **Autonomy** | Which enemy types to prioritize is the core tactical decision every run | Core |
| **Competence** | Learning type synergies and color combos rewards knowledge and improves outcomes | Core |
| **Relatedness** | The slime is expressive and cute; emotional attachment despite being a blob | Supporting |

### Player Type Appeal (Bartle Taxonomy)

- [x] **Achievers** — Power escalation arc, run completion, milestone unlocks (V1.0)
- [x] **Explorers** — Synergy discovery; "what if I absorb all fire types first?"
- [ ] **Socializers** — Not a social game (screenshot sharing is passive)
- [ ] **Killers/Competitors** — No PvP or leaderboard in MVP

### Flow State Design

- **Onboarding curve:** First 60 seconds — slime is small, enemies are slow, absorption
  is hard to miss. The mechanic teaches itself before the player reads anything.
- **Difficulty scaling:** Enemy density and move speed increase per wave. Elite enemies
  appear at wave 4+ to force ability decisions under pressure.
- **Feedback clarity:** Color shift is immediate visual confirmation of absorption.
  Ability unlock text appears on upgrade screen. Run score at end shows absorption count by type.
- **Recovery from failure:** Instant restart. Run is 10–20 min — short enough that death
  feels like "one more try" not "lost progress."

---

## Core Loop

### Moment-to-Moment (30 seconds)
Move the slime around the arena. Enemies swarm. Proximity triggers the magnetic pull —
enemies are drawn slightly toward you. Contact = absorption pop + color shift. Passive
abilities fire automatically. Survive the wave.

### Short-Term (5-15 minutes)
Wave clears → level-up pause → choose 1 of 3 upgrades drawn from the 5-card pool.
Every 3–4 waves, an Elite enemy appears. Absorbing it grants a rare aura bonus and a
powered-up ability variant. Each wave cleared is a small victory; each Elite absorbed
is a dopamine spike.

### Session-Level (10-20 minutes)
Run opens with a tiny white slime. It escalates through color evolutions and ability
stacks. Final wave is the boss. Run ends in victory or death. Natural stopping point.
The slime's final color palette is the run's "story" — shareable, unique.

### Long-Term Progression
**MVP:** No meta-progression — pure run-based loop. Run quality is its own reward.
**V1.0+:** Unlock new starting slime archetypes (pre-seeded color/ability combos) via
run milestones. Unlock new biomes with new enemy color pools.

### Retention Hooks

- **Curiosity:** "What happens if I only absorb blue enemies all run?"
- **Investment:** Mid-run color builds feel personal — players want to finish the run
  they're on.
- **Mastery:** Type synergy knowledge compounds across runs; skilled players clearly
  perform better.
- **Social (passive):** End-of-run slime color is screenshot-worthy — organic sharing.

---

## Game Pillars

### Pillar 1: Absorb Everything
Every interaction is an absorption opportunity — nothing is neutral contact.

*Design test:* If we're debating whether X should trigger the absorption mechanic — it
does. If it doesn't, cut it or remove it from the game.

### Pillar 2: Readable Chaos
The screen can be filled with effects and enemies, but the player always knows what
they are and what they're doing.

*Design test:* If a new player can't identify an enemy type within 1 second, redesign
the visual. If the slime's current state isn't readable at a glance, simplify the VFX.

### Pillar 3: Every Run Tells a Story
The color evolution of your slime is a visual diary of the choices you made this run.

*Design test:* If two runs can end with identical-looking slimes via different paths,
we've failed this pillar. Color must be uniquely determined by absorption history.

### Pillar 4: Pop Anime Energy
Everything is expressive, bouncy, and exaggerated. Physics, UI, sound, art — all pushed
to anime extremes.

*Design test:* If it could ship in a Western-art-style game unchanged, it's not pop
anime enough. Add bounce, add saturation, add personality.

### Pillar 5: Tight & Shippable
Every feature must justify its presence in the MVP. If it can't be built in weeks, it's
a post-launch idea.

*Design test:* Does the core loop work without this feature? If yes — it's not MVP scope.

### Anti-Pillars (What This Game Is NOT)

- **NOT a builder/crafter:** Real-time crafting or base-building would dilute the
  "move and absorb" core verb. Every second spent in a menu is a second not absorbing.
- **NOT a narrative game:** No dialogue, cutscenes, or story beats. The slime's
  visual evolution IS the story.
- **NOT multiplayer:** Scope-killer for a weeks timeline. Co-op and PvP are V2+ ideas.
- **NOT manually aimed:** No active attack buttons. Passive auto-attack is the genre
  contract. Breaking it breaks the loop.

---

## Inspiration and References

| Reference | What We Take From It | What We Do Differently | Why It Matters |
| ---- | ---- | ---- | ---- |
| Vampire Survivors | Passive auto-attack survivor loop; wave escalation; level-up upgrade picks | Absorption as the core verb; visual evolution; anime aesthetic | Proves the market and loop. Our hook differentiates. |
| Genshin Impact | Pop anime art direction; expressive character personality; color as identity | No gacha; slime is a blank canvas not a named character | Validates the aesthetic appeal to our target audience |
| Nikke | High-quality anime presentation on a simple gameplay loop | 2D arena (not side-scroll); no story/dialogue | Proves players will engage with strong anime style even in simple games |
| That Time I Got Reincarnated as a Slime (anime) | Slime-as-protagonist power fantasy; absorption as ability acquisition | No RPG story; mechanics-first not narrative-first | Direct cultural reference for the "slime who becomes powerful" fantasy |

**Non-game inspirations:**
- Anime opening sequences (Chainsaw Man, Jujutsu Kaisen) — kinetic energy, color
  saturation, expressive motion as a visual standard
- Lava lamps and fluid dynamics — the way color bleeds and blends as an aesthetic
  reference for how absorption should feel visually

---

## Target Player Profile

| Attribute | Detail |
| ---- | ---- |
| **Age range** | 16–30 |
| **Gaming experience** | Mid-core |
| **Time availability** | Short sessions (10–30 min); browser-accessible anywhere |
| **Platform preference** | Web / browser; later mobile |
| **Current games they play** | Vampire Survivors, Genshin Impact, Brotato |
| **What they're looking for** | A quick, satisfying run with strong visual style — feels like an anime power-up |
| **What would turn them away** | Slow start; ugly art; complex UI; long tutorial; no visual feedback |

---

## Technical Considerations

| Consideration | Assessment |
| ---- | ---- |
| **Recommended Engine** | Unity (developer's existing expertise; solid WebGL export) |
| **Key Technical Challenges** | WebGL build size optimization; hue-shift shader for color evolution; enemy density performance in browser |
| **Art Style** | 2D anime sprite; squash-and-stretch animation; particle-heavy VFX |
| **Art Pipeline Complexity** | Medium (custom 2D sprites + shader-driven color system) |
| **Audio Needs** | Moderate (satisfying absorption SFX; energetic BGM; enemy-type audio cues) |
| **Networking** | None |
| **Content Volume** | MVP: 1 biome, 6 enemy types, 5 upgrades, 1 boss, ~15 min runs |
| **Procedural Systems** | Enemy spawning is wave-scripted, not fully procedural. Upgrade pool is randomized draw. |

**Color evolution technical note:** Hue rotation shader on the slime sprite is the
recommended implementation — cheap, visually impactful, and avoids needing separate
sprites per color state. Enemy absorption blends the slime's target hue value toward
the enemy's hue by a fixed amount per absorption event.

---

## Risks and Open Questions

### Design Risks
- The absorption mechanic could feel too passive — player moves, enemies come to them.
  Risk: no agency. Mitigation: the *prioritization* of which enemies to absorb first is
  the active decision layer.
- 5 upgrades is a small pool — players may see the same options repeatedly. Mitigation:
  V1.0 expands the pool; MVP tests whether the loop is fun before adding variety.

### Technical Risks
- WebGL Unity build size may be too large to share easily. Mitigation: profile early,
  strip unused packages, use addressables if needed.
- Hue-shift shader + many simultaneous particle systems may exceed browser GPU budgets.
  Mitigation: profile on low-end device early; cap active particle count.

### Market Risks
- Vampire Survivors clones are common. Mitigation: the slime + absorption + anime aesthetic
  is genuinely novel visually — the hook must be visible in the first 5 seconds of a GIF.
- Browser games face discoverability problems. Mitigation: design for screenshots and
  short clips from day one; the slime's color evolution is inherently shareable.

### Scope Risks
- Art production (6 enemy types + animations + VFX) may dominate the timeline.
  Mitigation: use placeholder geometry first; validate loop before investing in art.
- "Just one more feature" creep. Mitigation: Pillar 5 (Tight & Shippable) is the veto.

### Open Questions
- Does the absorption prioritization decision feel meaningful? → Prototype with 3 enemy
  types and 2 upgrades to test.
- What's the right magnetic pull radius? Too small = frustrating; too large = no skill
  expression. → Test with 3 radius values in prototype.
- Does the color shift read clearly when multiple hues are blended? → Shader prototype
  needed early.

---

## MVP Definition

**Core hypothesis:** Players find the "absorb → evolve color → absorb more" loop engaging
for a full 10–15 minute run without meta-progression or story.

**Required for MVP:**
1. Slime movement (8-directional or analog stick)
2. Magnetic absorption mechanic with pop VFX and color shift
3. 6 enemy types (each a distinct hue, simple behavior)
4. Wave escalation (density + speed increase per wave)
5. 5-upgrade level-up pool with 3-choice selection screen
6. 1 boss encounter at run end
7. Run end screen (score + final slime color display)

**Explicitly NOT in MVP:**
- Meta-progression / unlockables
- Multiple biomes
- Sound design (placeholder only)
- Mobile input / touch controls
- Leaderboards
- Menu polish / tutorial
- Narrative of any kind

### Scope Tiers

| Tier | Content | Features | Timeline |
| ---- | ---- | ---- | ---- |
| **MVP** | 1 biome, 6 enemies, 5 upgrades, 1 boss | Core absorption loop, color evolution, wave escalation | 2–3 weeks |
| **V1.0** | 3 biomes, 12 enemies, 15 upgrades | Meta unlocks (slime archetypes), SFX, run history | 2–4 months |
| **Full Vision** | 5 biomes, 20+ enemies, 30 upgrades | Color synergy system, online leaderboard, daily runs, mobile port | 6–12 months |

---

## Next Steps

- [ ] Run `/setup-engine` to configure Unity + WebGL and populate version-aware reference docs
- [ ] Run `/art-bible` to create the visual identity specification before writing GDDs
- [ ] Run `/design-review design/gdd/game-concept.md` to validate concept completeness
- [ ] Run `/map-systems` to decompose concept into individual systems with dependencies
- [ ] Author per-system GDDs with `/design-system` for each system identified above
- [ ] Plan technical architecture with `/create-architecture`
- [ ] Record key decisions with `/architecture-decision (×N)`
- [ ] Validate readiness with `/gate-check`
- [ ] Prototype the absorption mechanic with `/prototype absorption-loop`
- [ ] Document playtest results with `/playtest-report`
- [ ] Plan first sprint with `/sprint-plan new`
