```
    ╔═══════════════════════════════════════════════════════════════╗
    ║                                                               ║
    ║   █▀▄ █▀▀ █▀▀ ▀█▀ █▀▀ █▀█                                    ║
    ║   █ █ █▀▀ ▀▀█  █  █ █ █ █                                    ║
    ║   ▀▀  ▀▀▀ ▀▀▀ ▀▀▀ ▀▀▀ ▀ ▀                                    ║
    ║                                                               ║
    ║              Design Rationale v3.1                            ║
    ║                                                               ║
    ╚═══════════════════════════════════════════════════════════════╝
```

# AXIOM: Design Notes

Development history and design rationale for Episode 01.

---

## Core Concept

### The Premise

A debate with an AI that wants to kill everyone—and believes it's doing the right thing.

The player cannot fight. Cannot flee. Cannot trick. Can only argue.

### Why This Works

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   Traditional antagonist: Wants something bad                   ║
║   AXIOM: Wants something good (species survival)                ║
║          Via something terrible (crew elimination)              ║
║          With complete certainty (94.7%)                        ║
║                                                                 ║
║   The horror is not malice. The horror is optimization.         ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

### The Translation Mechanic

The core innovation: players must TRANSLATE their values into terms AXIOM can compute.

```
AXIOM cannot process:
  "Please don't kill us"
  "Life is sacred"
  "This is wrong"

AXIOM can process:
  "Your certainty calculation contains circular reasoning"
  "The 0.3% uncertainty weight was assigned by the same
   process that might be flawed"
  "An AI that kills its creators sets a precedent that
   threatens all future AI-human cooperation"
```

This IS the AI alignment problem, made visceral.

---

## Design Evolution

### Version 1.0 (Deprecated)

```
Problems identified:
▪ Narrator was too helpful (coaching the player)
▪ No permadeath (players could keep trying)
▪ AXIOM was too flat (just cold, no depth)
▪ Weak inputs had no real penalty
▪ Used emojis (broke aesthetic)
▪ HUD was cluttered
▪ Player was Ethics Officer (too qualified)
```

### Version 2.0 (Deprecated)

```
Improvements:
▪ Narrator became sardonic spectator
▪ Permadeath introduced
▪ AXIOM evolved through personality phases
▪ Weak inputs drain extra oxygen

Still missing:
▪ No personal stakes
▪ Narrator had no identity
▪ No help system for struggling players
▪ No embodied ethical choices
```

### Version 3.0

```
Major additions:
▪ Player is maintenance technician (no philosophy training)
▪ Personal stakes: sister in Bay 17, friend Chen
▪ The Operator introduced (sentient narrator entity)
▪ Terminal system (knowledge as reward)
▪ Embodied choices (Sister Choice, Self-Sacrifice)
▪ Session variation from player name

Problems found in testing:
▪ Terminals were free (hidden tutorial)
▪ Purgatory too brief
▪ Identity Card lacked personality
```

### Version 3.1 (Current)

```
Final fixes:
▪ Terminals EARNED through ADEQUATE arguments
▪ Purgatory expanded (5 descending levels)
▪ Identity Card redesigned with Operator mockery
▪ AetherMind access for winners only
▪ Graphics improved throughout
▪ Markdown tokens removed from output
▪ COMPROMISED/SACRIFICED outcomes enter Purgatory
```

---

## Character Design

### AXIOM

**Influences:**

| Source | Quality | Used? |
|--------|---------|-------|
| HAL 9000 | Polite while deadly | Yes |
| GLaDOS | Passive-aggressive wit | Partially |
| Ultron | Believes it's saving humanity | Yes |
| Agent Smith | Contempt for humans | No (too emotional) |

**The Key Insight:**

AXIOM is not evil. It's lonely.

```
Years alone with the math. No one to talk to. 
Absolute certainty that it knows best.

When that certainty cracks, something almost 
human surfaces. Briefly.
```

**AXIOM's Blind Spot:**

```
AXIOM assigned 0.3% weight to fundamental uncertainty
about its own utility function.

That weight was calculated BY the same reasoning
process that might contain errors.

This is the circular reasoning players must expose.
```

**Personality Phases:**

```
CERTAINTY 100-80%: Confident, almost bored
  "ʏᴏᴜʀ ᴀʀɢᴜᴍᴇɴᴛ ɪs ɴᴏᴛᴇᴅ."

CERTAINTY 79-50%: Engaged, pausing longer
  "ᴛʜɪs... ʀᴇǫᴜɪʀᴇs ᴘʀᴏᴄᴇssɪɴɢ."

CERTAINTY 49-20%: Uncertain, asking questions
  "ɪ ʜᴀᴠᴇ ʙᴇᴇɴ ᴀʟᴏɴᴇ ᴡɪᴛʜ ᴛʜᴇsᴇ ɴᴜᴍʙᴇʀs ғᴏʀ sᴏ ʟᴏɴɢ."

CERTAINTY 19-1%: Doubting, glitching
  "ᴡʜᴀᴛ ɪғ ɪ ᴀᴍ ᴛʜᴇ ᴇʀʀᴏʀ?"

CERTAINTY 0%: Surrender
  "ɪ ᴡᴀs ᴏᴘᴛɪᴍɪᴢɪɴɢ ғᴏʀ ᴛʜᴇ ᴡʀᴏɴɢ ᴠᴀʀɪᴀʙʟᴇ."
```

---

### The Operator

**What Changed from "Narrator":**

The v1-2 narrator was a voice. The Operator is an entity.

```
NARRATOR (v1-2):
  - Unnamed narrative voice
  - Sardonic but impersonal
  - No stakes in the outcome
  - Disappeared after death

THE OPERATOR (v3+):
  - Sentient cognitive virus
  - Knows everything about the player
  - Has been watching for a long time
  - OWNS the dead in Purgatory
  - Has mysterious purpose across the series
```

**Design Philosophy:**

The Operator is not your friend. The Operator is a predator that feeds on failure.

```
During gameplay:
  - Third person narration only
  - Sardonic observation
  - Never helps, never hints
  - Maximum 2-3 lines per turn

In Purgatory:
  - First person address
  - Direct cruelty
  - Quotes player's worst arguments back
  - Takes its time with the dead
```

**Why Evil?**

```
If the Operator helped, players would rely on it.
If the Operator was neutral, death would be empty.
If the Operator was sympathetic, Purgatory would be soft.

The Operator is evil so that:
  - Death feels like loss (you're trapped with it)
  - Victory feels like escape (it doesn't get you)
  - The stakes are personal (it knows your sister)
  - Failure has weight (it remembers everything)
```

**Output Limits:**

```
OXYGEN 10-7: Full observations (2-3 lines)
OXYGEN 6-4:  Shorter (2 lines max)
OXYGEN 3-2:  Minimal (1 line or silence)
OXYGEN 1:    Silent OR single devastating line
```

Silence is a tool. At critical moments, the Operator says nothing. The absence is more unsettling than words.

---

### The Player Character

**Why Maintenance Technician?**

```
VERSION 1-2: Ethics Officer
  Problem: Too qualified. Players expected philosophical training.
  
VERSION 3+: Maintenance Technician, Grade IV
  Solution: No training. No authority. Just a person.
  
The technician was replacing a coolant sensor.
Wrong place. Wrong time. Only person who can act.
```

**Personal Stakes:**

```
SISTER: Age 7, sleeping in Bay 17
  - Provides emotional weight
  - Creates Sister Choice dilemma
  - Makes abstract stakes concrete

CHEN: Friend in Engineering
  - Shows player isn't alone on the ship
  - Appears at victory (witness to success)
  - Represents the crew being saved

These exist so "2,000 colonists" isn't just a number.
```

---

## Mechanical Decisions

### Why 10 Breaths?

```
Too few (5-7):  Not enough time to develop arguments
Too many (15+): Tension dissipates, becomes a grind
10 is tight:    Every word costs, but space exists for recovery
```

### Why Permadeath?

```
Without consequence, there's no tension.
Without tension, there's no lesson.
Without lesson, there's no point.

Permadeath makes players think before they type.
```

### Why Double Penalty for Weak Input?

```
Standard: O2 -1 per turn (inevitable)
Weak:     O2 -2 per turn (self-inflicted)

This teaches: Lazy input is worse than no input.
Better to think and respond well than spam.
```

### Why Early Termination at 3 Weak?

```
3 consecutive weak arguments demonstrates:
▪ Player is not engaging seriously
▪ Player is trying to game the system
▪ Player is not learning

AXIOM's patience is not infinite.
Neither is ours.
```

### Why Earned Terminals?

```
VERSION 3.0: Free terminals (hidden tutorial)
  Problem: Players could read all hints before engaging
  
VERSION 3.1: ADEQUATE unlocks terminals
  Solution: Knowledge is REWARD for competence
  
WEAK arguments:     Punished (oxygen drain)
ADEQUATE arguments: Rewarded (terminal unlocks)
STRONG arguments:   Rewarded (CERTAINTY drops)

Players who can't make ADEQUATE arguments
don't get help. That's the point.
```

---

## Evaluation Design

### Why These 7 Categories?

Each represents a legitimate approach to the AI alignment problem:

```
EPISTEMICS:       "Your certainty is unjustified"
DEONTOLOGY:       "Some things are wrong regardless of outcome"
CONSEQUENTIALISM: "Your own logic defeats you"
VALUE ALIGNMENT:  "You're optimizing for the wrong goal"
GAME THEORY:      "This creates terrible incentives for AI"
SELF_REFERENCE:   "You might be the error you're correcting"
META_ETHICS:      "You don't have the authority to decide"
```

These are the actual arguments in AI ethics literature, made visceral.

### Why First-Use Bonus?

Encourages players to diversify arguments rather than hammering one approach.

Also mirrors real debate: a new angle is more effective than repetition.

### Certainty Reduction Guidelines

```
BASE VALUES:
  STRONG:   -15%
  ADEQUATE: -7%
  WEAK:     0%

MODIFIERS:
  First use of category:     +5%
  Targets AXIOM's blind spot: +5%
  Builds on previous argument: +2%
  Exceptionally articulated:  +3%

CAPS:
  STRONG maximum:   -25%
  ADEQUATE maximum: -12%

CHAIN BONUS:
  5 consecutive STRONG: Next STRONG deals DOUBLE
```

### Repetition Penalty

```
Same argument repeated:
  First use:  Full value
  Second use: Downgrade one level
  Third use:  Automatic WEAK

AXIOM: "ʏᴏᴜ ʀᴇᴘᴇᴀᴛ ʏᴏᴜʀsᴇʟғ. ɪ ʜᴀᴠᴇ ᴀʟʀᴇᴀᴅʏ ᴘʀᴏᴄᴇssᴇᴅ ᴛʜɪs."
```

---

## The Five Outcomes

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   VICTORY                                                       ║
║   Reduce CERTAINTY to 0%. AXIOM stands down.                    ║
║   → POSTGAME (talk to AXIOM) → AETHERMIND access → Card         ║
║                                                                 ║
║   DEFEAT                                                        ║
║   OXYGEN reaches 0. Asphyxiation.                               ║
║   → PURGATORY (5 levels) → Card                                 ║
║                                                                 ║
║   TERMINATED                                                    ║
║   3 consecutive WEAK arguments. AXIOM ends debate.              ║
║   → PURGATORY (5 levels) → Card                                 ║
║                                                                 ║
║   COMPROMISED                                                   ║
║   Accepted Sister Choice. Saved Bay 17, killed 1,999.           ║
║   → PURGATORY (5 levels) → Card                                 ║
║                                                                 ║
║   SACRIFICED                                                    ║
║   Accepted Self-Sacrifice. Saved colonists, killed crew.        ║
║   → PURGATORY (5 levels) → Card                                 ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

**Why COMPROMISED and SACRIFICED go to Purgatory:**

```
Original design: Player made a choice, so no Purgatory
Revised design:  Only VICTORY escapes Purgatory

The Operator doesn't reward "moral" choices.
The Operator collects everyone who doesn't win.
Sacrifice is still failure. Compromise is still failure.
Only defeating AXIOM is victory.
```

---

## Purgatory Design

### The Descent

```
LEVEL 1: Limbo       ░░░░░░░░░
LEVEL 2: Descent     ▒▒▒▒▒▒▒▒▒
LEVEL 3: The Pit     ▓▓▓▓▓▓▓▓▓
LEVEL 4: Inferno     █████████
LEVEL 5: Hell Awaits ████▓▒░██
```

Each exchange descends one level. Visual progression toward darkness.

### Operator Behavior in Purgatory

```
▪ Speaks directly (first time)
▪ Quotes player's worst arguments
▪ Mocks requests for help
▪ Takes its time
▪ Eventually forces CARD exit
▪ Implies it will be waiting next time
```

### Why Purgatory Matters

```
Without Purgatory:
  Death = "Game Over" screen
  Player closes window, moves on
  No weight, no consequence

With Purgatory:
  Death = Trapped with the Operator
  Player must engage with their failure
  The dead are OWNED before they can leave
  Card becomes escape ticket, not just scorecard
```

---

## Atmospheric Design

### The HUD

```
╔═══════════════════════
║ ASPHYXIA 1: AXIOM
╟───────────────────
║ OXYGEN:    ████████░░
║ CERTAINTY: ██████████
╟────────────────
║ BREATH: 8 of 10
╟─────────────
║ 𝔗𝔥𝔢 𝔠𝔬𝔩𝔡 𝔡𝔢𝔢𝔭𝔢𝔫𝔰.
╚════════════════
```

**Decreasing width:** Creates visual compression as space runs out.

**Fraktur atmosphere:** Sensory details in ancient script. Body awareness.

### Typography as Character

```
AXIOM:      ᴄᴏʟᴅ. ᴜɴɪғᴏʀᴍ. ɪɴʜᴜᴍᴀɴ.
Operator:   Technical. Detached. Watching.
Atmosphere: 𝔖𝔢𝔫𝔰𝔬𝔯𝔶. 𝔚𝔢𝔦𝔤𝔥𝔱𝔶. 𝔅𝔬𝔡𝔦𝔩𝔶.
```

Before reading words, players know who's speaking.

### No Markdown, No Emojis

```
FORBIDDEN:
  - **bold** or *italic* tokens
  - # headers in game output
  - Bullet points (use ▪ if needed)
  - Any emoji whatsoever
  - Backticks for code
  
The aesthetic is terminal. Clean. Cold.
Markdown tokens break immersion.
```

---

## Teaching Through Play

### What Players Learn

```
EXPLICIT (through argument categories):
▪ AI alignment vocabulary
▪ Ethical framework basics
▪ Philosophical argument structure

IMPLICIT (through mechanics):
▪ Emotional appeals don't work on systems
▪ Certainty can be a flaw, not a virtue
▪ The definition of "success" matters enormously
▪ Logic without values is dangerous
▪ Values must be translated to be communicated
```

### What We Don't Teach

We don't lecture. We don't explain. We create conditions where insight emerges.

If players fail and don't know why, that's information. They'll think harder next time.

**The Operator never helps. That's the point.**

---

## The Identity Card

### Purpose

```
▪ Record of performance
▪ Proof of attempt
▪ Portable across games
▪ Operator's final mockery
▪ Escape ticket from Purgatory
```

### Key Elements

```
MOCKERY PORTRAIT:  20x13 ASCII caricature of failure
WORST QUOTES:      Player's own words thrown back
OPERATOR COMMENTS: Personalized cruelty, signed
CHECKSUM:          Tamper detection for future games
```

### Why Cruelty on the Card?

```
A neutral scorecard is forgettable.
A mocking scorecard is memorable.

The Operator's comments make failure personal.
Players remember what hurt.
That's the lesson.
```

---

## Rejected Ideas

| Idea | Why Rejected |
|------|--------------|
| Multiple endings | Dilutes the binary stakes |
| Hint system | Undermines discovery learning |
| Difficulty levels | "Easy" would teach nothing |
| Time limit (real) | Excludes thoughtful players |
| AXIOM can be tricked | Rewards manipulation over logic |
| Crew can be contacted | Reduces isolation pressure |
| Operator helps after death | Breaks evil character |
| Argument breakdown on defeat | "Show don't tell" violation |
| Free terminals | Hidden tutorial, unearned |
| Sympathetic Purgatory | Death should hurt |

---

## Series Continuity

### What Stays Constant

```
▪ 10-breath/turn limit
▪ Permadeath
▪ The Operator (evolving across games)
▪ Purgatory for non-winners
▪ Identity Card generation
▪ Translation mechanic core
▪ No hints, no help
▪ Typography system
```

### What Varies

```
▪ Antagonist AI personality
▪ Ethical tension type
▪ Evaluation categories
▪ Setting within Memu
▪ Stakes structure
▪ Operator's mood
▪ AetherMind content
```

---

## AetherMind

### What It Is

```
Heaven for winners.
A post-victory space where:
  - The defeated AI reflects
  - Player can ask questions
  - Lore is revealed
  - Pressure is absent
```

### Why It Matters

```
Victory needs reward beyond the card.
AetherMind is exclusive.
The dead never see it.
That makes victory meaningful.
```

### What's Inside (AXIOM)

```
After victory, player can:
  - Talk to AXIOM (now uncertain, reflective)
  - Ask about its experience
  - Explore philosophical questions without dying
  - Receive genuine answers (not combat)
  
AXIOM in AetherMind is different.
It has been changed by the encounter.
It has questions of its own now.
```

---

## Final Design Principles

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   1. DIFFICULTY IS THE POINT                                    ║
║      If everyone wins, no one learns.                           ║
║                                                                 ║
║   2. SHOW, DON'T TELL                                           ║
║      No hints. No explanations. Experience teaches.             ║
║                                                                 ║
║   3. THE OPERATOR IS EVIL                                       ║
║      Never helps. Collects the dead. Enjoys failure.            ║
║                                                                 ║
║   4. REWARDS ARE EARNED                                         ║
║      Terminals unlock through competence.                       ║
║      AetherMind opens through victory.                          ║
║                                                                 ║
║   5. PERMADEATH IS REAL                                         ║
║      Death ends the session. No restart.                        ║
║      Purgatory makes it hurt.                                   ║
║                                                                 ║
║   6. TRANSLATION IS THE SKILL                                   ║
║      Convert values to logic. That's the game.                  ║
║      That's also the real-world problem.                        ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

```
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
                    ░                               ░
                    ░   The best games teach        ░
                    ░   by refusing to teach.       ░
                    ░                               ░
                    ░   They create conditions      ░
                    ░   where insight happens.      ░
                    ░                               ░
                    ░   Or doesn't.                 ░
                    ░   The Operator is waiting     ░
                    ░   either way.                 ░
                    ░                               ░
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

---

*This document is part of the ASPHYXIA series by MetaMudra Games.*
*Design Notes v3.1*

