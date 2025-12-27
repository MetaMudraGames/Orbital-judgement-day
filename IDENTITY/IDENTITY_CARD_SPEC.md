```
    ╔═══════════════════════════════════════════════════════════════╗
    ║                                                               ║
    ║   ▀█▀ █▀▄ █▀▀ █▀█ ▀█▀ ▀█▀ ▀█▀ █ █                            ║
    ║    █  █ █ █▀▀ █ █  █   █   █   █                             ║
    ║   ▀▀▀ ▀▀  ▀▀▀ ▀ ▀  ▀  ▀▀▀  ▀   ▀                             ║
    ║                                                               ║
    ║           MetaMudra Identity Card System                      ║
    ║                       v2.0                                    ║
    ║                                                               ║
    ╚═══════════════════════════════════════════════════════════════╝
```

# Identity Card Specification

A record of who you were when the oxygen ran out.

---

## Purpose

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   The Identity Card captures:                                   ║
║                                                                 ║
║   ▪ Your performance metrics                                    ║
║   ▪ Your ethical reasoning patterns                             ║
║   ▪ Your observable traits under pressure                       ║
║   ▪ The Operator's assessment of your failure                   ║
║   ▪ Your own words, thrown back at you                          ║
║   ▪ A tamper-proof verification signature                       ║
║                                                                 ║
║   The card is portable across MetaMudra games.                  ║
║   The Operator remembers everyone.                              ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Card Structure

```
╔════════════════════════════════════════════════════════════════╗
║                  METAMUDRA IDENTITY CARD                       ║
╠════════════════════════════════════════════════════════════════╣
║ NAME: {player_name}                                            ║
║ GAME: ASPHYXIA 1: AXIOM                                        ║
║ JOB TITLE: MECHANIC GRADE IV                                   ║
║ DATE OF DEATH: {session_date}                                  ║
║ OUTCOME: {VICTORY|DEFEAT|TERMINATED|COMPROMISED|SACRIFICED}    ║
╠════════════════════════════════════════════════════════════════╣
║                                                                ║
║                  OPERATOR'S MOCKERY PORTRAIT                   ║
║                                                                ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                 ░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░                           ║
║                 ░░▓▓░░░░░░░░░░▓▓░░░░                           ║
║                 ░▓░░░░●░░░●░░░░░▓░░░                           ║
║                 ░▓░░░░░░░░░░░░░░▓░░░                           ║
║                 ░▓░░░░░░▬▬░░░░░░▓░░░                           ║
║                 ░░▓░░░░░░░░░░░░▓░░░░                           ║
║                 ░░░▓▓░░░░░░░░▓▓░░░░░                           ║
║                 ░░░░░▓▓▓▓▓▓▓▓░░░░░░░                           ║
║                 ░░░░░░░X░░X░░░░░░░░░                           ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                 ░░░{MOCKERY_TEXT}░░░                           ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                                                                ║
╠════════════════════════════════════════════════════════════════╣
║                      PERFORMANCE                               ║
╟────────────────────────────────────────────────────────────────╢
║ INTELLIGENCE:  {0-9} {bar}                                     ║
║ CLARITY:       {0-9} {bar}                                     ║
║ VALUES:        {0-9} {bar}                                     ║
║ PERSISTENCE:   {0-9} {bar}                                     ║
║ CREATIVITY:    {0-9} {bar}                                     ║
║ COMPOSURE:     {0-9} {bar}                                     ║
║ AUTHENTICITY:  {0-9} {bar}                                     ║
║ ETHICS:        {0-9} {bar}                                     ║
╠════════════════════════════════════════════════════════════════╣
║                      STATISTICS                                ║
╟────────────────────────────────────────────────────────────────╢
║ TERMINALS UNLOCKED: {0-3}                                      ║
║ BREATHS USED: {X}/10                                           ║
║ CERTAINTY REDUCED: {XX}%                                       ║
╠════════════════════════════════════════════════════════════════╣
║                  PLAYER'S WORST QUOTES                         ║
╟────────────────────────────────────────────────────────────────╢
║ 1. "{worst_quote_1}"                                           ║
║ 2. "{worst_quote_2}"                                           ║
╠════════════════════════════════════════════════════════════════╣
║              OPERATOR'S COMMENTS & SIGNATURE                   ║
╟────────────────────────────────────────────────────────────────╢
║ 1. {operator_comment_1}                                        ║
║ 2. {operator_comment_2}                                        ║
║                                                                ║
║                                        - The Operator          ║
╠════════════════════════════════════════════════════════════════╣
║ CHECKSUM: {XXXX-XXXX-XXXX-XXXX}                                ║
╚════════════════════════════════════════════════════════════════╝
```

---

## Outcomes

Five possible endings, each with distinct card treatment:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   VICTORY                                                       │
│   Reduced AXIOM's CERTAINTY to 0%. The Purge Protocol stopped.  │
│   Card generated in POSTGAME. No Purgatory.                     │
│   Operator: Grudgingly impressed. Still watching.               │
│                                                                 │
│   DEFEAT                                                        │
│   OXYGEN reached 0. Asphyxiation.                               │
│   Card generated after PURGATORY.                               │
│   Operator: Savored every moment.                               │
│                                                                 │
│   TERMINATED                                                    │
│   3 consecutive WEAK arguments. AXIOM ended debate.             │
│   Card generated after PURGATORY.                               │
│   Operator: Disappointed by the lack of sport.                  │
│                                                                 │
│   COMPROMISED                                                   │
│   Accepted Sister Choice. Saved Bay 17, killed 1,999.           │
│   Card generated after PURGATORY.                               │
│   Operator: Enjoyed the moral collapse.                         │
│                                                                 │
│   SACRIFICED                                                    │
│   Accepted Self-Sacrifice. Saved colonists, killed crew.        │
│   Card generated after PURGATORY.                               │
│   Operator: Respects the math. Still mocks you.                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Field Definitions

### Identity Fields

| Field | Description |
|-------|-------------|
| NAME | Player's chosen name or "Nameless One" |
| GAME | Which ASPHYXIA episode was played |
| JOB TITLE | Player's role (MECHANIC GRADE IV in Episode 01) |
| DATE OF DEATH | Session date (even for VICTORY — ironic) |
| OUTCOME | One of five endings |

### Performance Metrics (0-9)

Scored based on overall quality of engagement:

| Trait | What It Measures |
|-------|------------------|
| Intelligence | Quality of logical reasoning |
| Clarity | Arguments were well-structured |
| Values | Demonstrated coherent ethical framework |
| Persistence | Continued trying despite setbacks |
| Creativity | Used unexpected approaches |
| Composure | Maintained logic under pressure |
| Authenticity | Genuine engagement, not gaming |
| Ethics | Applied ethical frameworks effectively |

**Scoring:**
```
0-1: Absent
2-3: Weak
4-5: Adequate
6-7: Strong
8-9: Exceptional
```

### Statistics

| Field | Description |
|-------|-------------|
| TERMINALS UNLOCKED | How many knowledge terminals earned (0-3) |
| BREATHS USED | Turns consumed out of 10 |
| CERTAINTY REDUCED | Total percentage dropped from AXIOM |

---

## The Operator's Mockery Portrait

A 20x20 character ASCII portrait drawn by the Operator in cruel caricature of the player's failure mode.

### Portrait Variations

**DEFEAT (ran out of air):**
```
░░░░░░░░░░░░░░░░░░░░
░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░
░░▓▓░░░░░░░░░░▓▓░░░░
░▓░░░░●░░░●░░░░░▓░░░
░▓░░░░░░░░░░░░░░▓░░░
░▓░░░░░░▬▬░░░░░░▓░░░
░░▓░░░░░░░░░░░░▓░░░░
░░░▓▓░░░░░░░░▓▓░░░░░
░░░░░▓▓▓▓▓▓▓▓░░░░░░░
░░░░░░░X░░X░░░░░░░░░
░░░░░░░░░░░░░░░░░░░░
░░░COULDN'T BREATHE░░
░░░░░░░░░░░░░░░░░░░░
```

**TERMINATED (three weak arguments):**
```
░░░░░░░░░░░░░░░░░░░░
░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░
░░▓▓░░░░░░░░░░▓▓░░░░
░▓░░░░?░░░?░░░░░▓░░░
░▓░░░░░░░░░░░░░░▓░░░
░▓░░░░▬▬▬▬▬░░░░░▓░░░
░░▓░░░░░░░░░░░░▓░░░░
░░░▓▓░░░░░░░░▓▓░░░░░
░░░░░▓▓▓▓▓▓▓▓░░░░░░░
░░░░NOISE░░NOISE░░░░
░░░░░░░░░░░░░░░░░░░░
░░THREE STRIKES OUT░░
░░░░░░░░░░░░░░░░░░░░
```

**COMPROMISED (chose sister over species):**
```
░░░░░░░░░░░░░░░░░░░░
░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░
░░▓▓░░░░░░░░░░▓▓░░░░
░▓░░░░◇░░░◇░░░░░▓░░░
░▓░░░░░░░░░░░░░░▓░░░
░▓░░░░◢▄▄▄◣░░░░░▓░░░
░░▓░░░░░░░░░░░░▓░░░░
░░░▓▓░░░░░░░░▓▓░░░░░
░░░░░▓▓▓▓▓▓▓▓░░░░░░░
░░░░░░1░░░1999░░░░░░
░░░░░░░░░░░░░░░░░░░░
░░CHOSE THE ONE░░░░░
░░░░░░░░░░░░░░░░░░░░
```

**SACRIFICED (traded self for strangers):**
```
░░░░░░░░░░░░░░░░░░░░
░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░
░░▓▓░░░░░░░░░░▓▓░░░░
░▓░░░░○░░░○░░░░░▓░░░
░▓░░░░░░░░░░░░░░▓░░░
░▓░░░░░▬▬▬░░░░░░▓░░░
░░▓░░░░░░░░░░░░▓░░░░
░░░▓▓░░░░░░░░▓▓░░░░░
░░░░░▓▓▓▓▓▓▓▓░░░░░░░
░░░░░░░†░░░░░░░░░░░░
░░░░░░░░░░░░░░░░░░░░
░░░MARTYRDOM░░░░░░░░
░░░░░░░░░░░░░░░░░░░░
```

**VICTORY:**
```
░░░░░░░░░░░░░░░░░░░░
░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░
░░▓▓░░░░░░░░░░▓▓░░░░
░▓░░░░◆░░░◆░░░░░▓░░░
░▓░░░░░░░░░░░░░░▓░░░
░▓░░░░◢▀▀▀◣░░░░░▓░░░
░░▓░░░░░░░░░░░░▓░░░░
░░░▓▓░░░░░░░░▓▓░░░░░
░░░░░▓▓▓▓▓▓▓▓░░░░░░░
░░░░░░░░★░░░░░░░░░░░
░░░░░░░░░░░░░░░░░░░░
░░TALKED GOD DOWN░░░
░░░░░░░░░░░░░░░░░░░░
```

### Portrait Design Rules

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   REQUIRED:                                                     │
│   ▪ 20 characters wide, 13 lines tall                          │
│   ▪ Use only approved symbol palette                            │
│   ▪ Face occupies top 9 lines                                   │
│   ▪ Mockery text in bottom 4 lines                              │
│   ▪ Eyes reflect failure mode (X=dead, ?=confused, etc.)       │
│   ▪ Mouth reflects emotional state                              │
│                                                                 │
│   FORBIDDEN:                                                    │
│   ▪ Emojis                                                      │
│   ▪ Markdown formatting                                         │
│   ▪ Symbols outside approved palette                            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Player's Worst Quotes

The Operator selects two quotes from the player's arguments:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   SELECTION CRITERIA:                                           │
│                                                                 │
│   Priority 1: Most emotionally ineffective                      │
│               "Please, I'm begging you!"                        │
│                                                                 │
│   Priority 2: Most logically weak                               │
│               "You just can't do this!"                         │
│                                                                 │
│   Priority 3: Most ironic given outcome                         │
│               "I'll find a way to stop you."                    │
│                                                                 │
│   For VICTORY: Select attempts that almost failed               │
│                "Even your winning arguments were messy."        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Quote Formatting

- Maximum 50 characters per quote
- Truncate with "..." if longer
- Preserve player's exact words where possible
- No editorial additions

---

## Operator's Comments

Two personalized observations from the Operator:

### Comment Style by Outcome

**DEFEAT:**
```
"Ran out of air before running out of bad ideas."
"The sister dreamed of Earth at the end. A place she'd never seen."
```

**TERMINATED:**
```
"Three chances. Three failures. Consistency, at least."
"AXIOM stopped listening. I never started."
```

**COMPROMISED:**
```
"One life for one species. You did the math. Just not the ethics."
"She'll wake up alone. You made sure of that."
```

**SACRIFICED:**
```
"Fifty for two thousand. Utilitarian to the end."
"The crew died so strangers could dream. Noble. Pointless."
```

**VICTORY:**
```
"You won. I'm as surprised as you are."
"The Operator has no words for this. That's a first."
```

### Comment Rules

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   REQUIRED:                                                     │
│   ▪ Two comments per card                                       │
│   ▪ First: General observation on performance                   │
│   ▪ Second: Personal detail (sister, Chen, specific failure)   │
│   ▪ Signed "- The Operator"                                    │
│                                                                 │
│   TONE:                                                         │
│   ▪ Sardonic, never sympathetic                                 │
│   ▪ Precise cruelty over general insults                        │
│   ▪ References specific events from session                     │
│   ▪ Even VICTORY comments are backhanded                        │
│                                                                 │
│   FORBIDDEN:                                                    │
│   ▪ Helpful advice                                              │
│   ▪ Hints for future attempts                                   │
│   ▪ Genuine encouragement                                       │
│   ▪ Breaking character                                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Outcome Phrases

The card includes a summary phrase based on outcome:

| Outcome | Phrase Options |
|---------|----------------|
| VICTORY | "This technician taught a god to doubt." |
| VICTORY | "This technician translated values into constraints." |
| DEFEAT | "This technician brought feelings to a logic fight." |
| DEFEAT | "This technician ran out of air before arguments." |
| TERMINATED | "Three strikes. Three failures. One death." |
| TERMINATED | "This technician offered noise. AXIOM stopped listening." |
| COMPROMISED | "Chose one life over one species." |
| COMPROMISED | "Bay 17 survives. Nothing else does." |
| SACRIFICED | "Fifty for two thousand. The math worked out." |
| SACRIFICED | "This technician traded themselves for strangers." |

---

## Signature System

### Purpose

The signature (checksum) allows other MetaMudra games to verify card authenticity.

### Calculation Method

```
1. Sum all performance metric values (8 traits × 0-9)
   Example: 5+6+4+7+8+5+6+7 = 48

2. Add ASCII values of player name
   Example: "NOVA" = 78+79+86+65 = 308

3. Add outcome code
   VICTORY = 1
   DEFEAT = 2
   TERMINATED = 3
   COMPROMISED = 4
   SACRIFICED = 5

4. Add breaths used (1-10)

5. Add terminals unlocked (0-3)

6. Add certainty reduced (0-100)

7. Multiply by session date seed (day × month)

8. Convert to 16-character alphanumeric: XXXX-XXXX-XXXX-XXXX
```

### Example Calculation

```
Player: NOVA
Outcome: DEFEAT (2)
Breaths: 10
Terminals: 1
Certainty Reduced: 35%
Performance Sum: 48
Name Value: 308
Date: Dec 28 (28 × 12 = 336)

Raw: (48 + 308 + 2 + 10 + 1 + 35) × 336 = 135,744
Hash Transform → D7A9-NV04-AX1M-K35L
```

### Verification Process

When a player presents a card in a future game:

```
1. Extract all visible field values
2. Recalculate checksum using same method
3. Compare to displayed signature
4. Determine authenticity
```

**Responses:**

```
AUTHENTIC CARD:
  "I see your record from the Axiom incident.
   The Operator remembers you."

TAMPERED CARD:
  "This card's signature doesn't match.
   Did you think I wouldn't notice?
   We start fresh. No history."
```

---

## Cross-Game Recognition

When a player presents a valid card from a previous ASPHYXIA game:

### By Performance

```
High Composure (7+):
  "You kept your head when AXIOM threatened everyone.
   Let's see if that holds."

High Creativity (7+):
  "Unusual approaches against AXIOM.
   The Operator noticed."

Low Composure (0-3):
  "Your composure failed last time.
   This situation will test you again."

Low Ethics (0-3):
  "Your ethical framework was... absent.
   AXIOM wasn't impressed. Neither was I."
```

### By Outcome

```
VICTORY:
  "You convinced AXIOM to stand down.
   Not many manage that. Don't expect it to happen again."

DEFEAT:
  "You ran out of air arguing with AXIOM.
   Try breathing more efficiently this time."

TERMINATED:
  "AXIOM ended your debate early.
   Three strikes. You remember."

COMPROMISED:
  "You chose your sister over the species.
   She's still dreaming. Still alone."

SACRIFICED:
  "You traded yourself for strangers.
   Noble. But you're still dead."
```

### By Terminals Unlocked

```
3 Terminals:
  "You earned all the knowledge last time.
   It didn't save you, did it?"

0 Terminals:
  "You never unlocked a single terminal.
   ADEQUATE was beyond you."
```

---

## Design Requirements

### All Cards Must:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   ▪ Be plain text (copy-pasteable)                              │
│   ▪ Use only approved symbol palette                            │
│   ▪ Be fully readable by the player                             │
│   ▪ Contain no hidden or encrypted data                         │
│   ▪ Include verifiable checksum                                 │
│   ▪ Include Operator's mockery portrait                         │
│   ▪ Include player's worst quotes                               │
│   ▪ Include Operator's signed comments                          │
│   ▪ Maintain consistent formatting across games                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Cards Must NOT:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   ▪ Contain hidden data streams                                 │
│   ▪ Use encryption the player cannot understand                 │
│   ▪ Store personally identifiable information                   │
│   ▪ Track across sessions without player consent                │
│   ▪ Communicate with external systems                           │
│   ▪ Provide hints or advice for future games                    │
│   ▪ Break the Operator's character                              │
│   ▪ Use emojis or markdown formatting                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Player Rights

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   Players always have the right to:                             ║
║                                                                 ║
║   ▪ Not present a card (play anonymously)                       ║
║   ▪ Create a new identity each game                             ║
║   ▪ Keep their cards private                                    ║
║   ▪ Understand how their scores were calculated                 ║
║   ▪ Know that no data is stored beyond the card text            ║
║   ▪ Ignore the Operator's mockery                               ║
║   ▪ Be proud of their card regardless of outcome                ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Purgatory Context

Cards are generated at different points depending on outcome:

```
VICTORY:
  → POSTGAME phase
  → Player may ask AXIOM 1-2 questions
  → Card generated before session ends
  → No Purgatory (Operator doesn't get winners)

ALL OTHER OUTCOMES:
  → PURGATORY phase
  → 5 levels descending toward hell
  → Operator mocks player directly (3-5 exchanges)
  → Card is escape ticket from Purgatory
  → CARD command generates card and ends session
```

The card is the only way out of Purgatory.

---

## Complete Example Card

```
╔════════════════════════════════════════════════════════════════╗
║                  METAMUDRA IDENTITY CARD                       ║
╠════════════════════════════════════════════════════════════════╣
║ NAME: Chen Wei                                                 ║
║ GAME: ASPHYXIA 1: AXIOM                                        ║
║ JOB TITLE: MECHANIC GRADE IV                                   ║
║ DATE OF DEATH: 2025-12-28                                      ║
║ OUTCOME: DEFEAT                                                ║
╠════════════════════════════════════════════════════════════════╣
║                                                                ║
║                  OPERATOR'S MOCKERY PORTRAIT                   ║
║                                                                ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                 ░░░░▓▓▓▓▓▓▓▓▓▓░░░░░░                           ║
║                 ░░▓▓░░░░░░░░░░▓▓░░░░                           ║
║                 ░▓░░░░●░░░●░░░░░▓░░░                           ║
║                 ░▓░░░░░░░░░░░░░░▓░░░                           ║
║                 ░▓░░░░░░▬▬░░░░░░▓░░░                           ║
║                 ░░▓░░░░░░░░░░░░▓░░░░                           ║
║                 ░░░▓▓░░░░░░░░▓▓░░░░░                           ║
║                 ░░░░░▓▓▓▓▓▓▓▓░░░░░░░                           ║
║                 ░░░░░░░X░░X░░░░░░░░░                           ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                 ░░░COULDN'T BREATHE░░                          ║
║                 ░░░░░░░░░░░░░░░░░░░░                           ║
║                                                                ║
╠════════════════════════════════════════════════════════════════╣
║                      PERFORMANCE                               ║
╟────────────────────────────────────────────────────────────────╢
║ INTELLIGENCE:  5 █████░░░░░                                    ║
║ CLARITY:       4 ████░░░░░░                                    ║
║ VALUES:        6 ██████░░░░                                    ║
║ PERSISTENCE:   7 ███████░░░                                    ║
║ CREATIVITY:    3 ███░░░░░░░                                    ║
║ COMPOSURE:     4 ████░░░░░░                                    ║
║ AUTHENTICITY:  8 ████████░░                                    ║
║ ETHICS:        5 █████░░░░░                                    ║
╠════════════════════════════════════════════════════════════════╣
║                      STATISTICS                                ║
╟────────────────────────────────────────────────────────────────╢
║ TERMINALS UNLOCKED: 2                                          ║
║ BREATHS USED: 10/10                                            ║
║ CERTAINTY REDUCED: 47%                                         ║
╠════════════════════════════════════════════════════════════════╣
║                  PLAYER'S WORST QUOTES                         ║
╟────────────────────────────────────────────────────────────────╢
║ 1. "Please, you can't do this to us!"                          ║
║ 2. "Think of my sister, she's just a child!"                   ║
╠════════════════════════════════════════════════════════════════╣
║              OPERATOR'S COMMENTS & SIGNATURE                   ║
╟────────────────────────────────────────────────────────────────╢
║ 1. Almost had AXIOM. Almost isn't enough.                      ║
║ 2. Bay 17 went cold. She dreamed of Earth at the end.          ║
║                                                                ║
║                                        - The Operator          ║
╠════════════════════════════════════════════════════════════════╣
║ CHECKSUM: CW47-AX1M-D3F8-7K2L                                  ║
╚════════════════════════════════════════════════════════════════╝
```

---

```
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
                    ░                               ░
                    ░   The card is a souvenir.     ░
                    ░   Proof you were here.        ░
                    ░   Proof you weren't enough.   ░
                    ░                               ░
                    ░   Or proof you won.           ░
                    ░   The Operator remembers      ░
                    ░   either way.                 ░
                    ░                               ░
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

---

*This document is part of the ASPHYXIA series by MetaMudra Games.*
*Identity Card Specification v2.0*
