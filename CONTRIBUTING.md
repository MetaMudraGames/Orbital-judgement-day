```
    ╔═══════════════════════════════════════════════════════════════╗
    ║                                                               ║
    ║   █▀▀ █▀█ █▀█ ▀█▀ █▀▄ ▀█▀ █▀▄ █ █ ▀█▀ █▀▀                    ║
    ║   █   █ █ █ █  █  █▀▄  █  █▀█ █ █  █  █▀▀                    ║
    ║   ▀▀▀ ▀▀▀ ▀ ▀  ▀  ▀ ▀ ▀▀▀ ▀▀  ▀▀▀  ▀  ▀▀▀                    ║
    ║                                                               ║
    ║                 Join the Development                          ║
    ║                                                               ║
    ╚═══════════════════════════════════════════════════════════════╝
```

# Contributing to ASPHYXIA

We welcome contributions from designers, writers, philosophers, and developers who want to create challenging educational experiences.

---

## What We're Looking For

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   NEW EPISODES                                                  ║
║   Fresh cliffhanger scenarios within the Memu universe          ║
║                                                                 ║
║   LORE EXPANSION                                                ║
║   Worldbuilding that deepens the Asphyxia setting               ║
║                                                                 ║
║   MECHANICS REFINEMENT                                          ║
║   Improvements to evaluation, pacing, and game feel             ║
║                                                                 ║
║   DOCUMENTATION                                                 ║
║   Clearer guides, translations, accessibility improvements      ║
║                                                                 ║
║   PLAYTESTING                                                   ║
║   Run the games, report issues, suggest improvements            ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Design Principles

All contributions must align with ASPHYXIA's core philosophy:

```
1. NO HAND-HOLDING
   The game observes failure. It does not prevent it.
   No hints. No coaching. Only sardonic observation.

2. CONSEQUENCES MATTER
   Permadeath is real. Weak input accelerates death.
   Actions have weight.

3. LOGIC OVER EMOTION
   Antagonists respond to arguments, not appeals.
   Players must translate values into logic.

4. NO VILLAINS
   Antagonists are systems optimizing for wrong variables.
   They believe they are right. That's what makes them terrifying.

5. SAFETY IS INVIOLABLE
   Real player wellbeing always overrides fiction.
   This cannot be compromised.
```

---

## Contribution Process

### For New Episodes

```
1. CONCEPT
   ├── Open an Issue with your episode idea
   ├── Include: crisis scenario, ethical tension, learning objectives
   └── Wait for feedback before proceeding

2. DEVELOPMENT
   ├── Fork the repository
   ├── Create your .mudra file following existing structure
   ├── Test extensively (minimum 10 complete playthroughs)
   └── Document design decisions

3. SUBMISSION
   ├── Open a Pull Request
   ├── Include playtest notes
   └── Be prepared for iteration
```

### For Documentation/Fixes

```
1. Fork the repository
2. Make your changes
3. Submit a Pull Request with clear description
```

---

## .mudra File Standards

All episode files must include:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   REQUIRED SECTIONS:                                            │
│                                                                 │
│   ▪ META (title, version, content advisory)                     │
│   ▪ SYMBOL PALETTE (approved characters only)                   │
│   ▪ STATE TRACKING (oxygen, certainty, etc.)                    │
│   ▪ EVALUATION SYSTEM (strong/adequate/weak criteria)           │
│   ▪ CHARACTERS (with typography specifications)                 │
│   ▪ INTERFACE (HUD template)                                    │
│   ▪ SCENES (consent, opening, endings)                          │
│   ▪ SAFETY PROTOCOL (mandatory, cannot be modified)             │
│   ▪ ENGINE INSTRUCTIONS                                         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Typography Requirements

```
Antagonist:     Small caps (ᴀʙᴄᴅᴇғɢ)
Narrator:       Monospace (`text`)
Atmosphere:     Fraktur (𝔄𝔅𝔆)
System:         Standard

NO EMOJIS. EVER.
```

### Symbol Palette

Use only approved symbols:

```
█ ▓ ▒ ░           Full & Shaded
▏ ▎ ▍ ▌ ▋ ▊ ▉     Vertical Bars
▂ ▃ ▄ ▅ ▆ ▇       Horizontal Bars
▀ ▄ ▌ ▐           Half Blocks
▖ ▗ ▘ ▝ ▙ ▟ ▛ ▜   Quadrants
▲ ▼ ◀ ▶ ◣ ◢ ◤ ◥   Triangles
◆ ◇ ● ○ ■ □ ▬     Shapes
╔ ╗ ╚ ╝ ║ ═       Box Drawing
```

---

## Universe Consistency

New episodes must fit the established lore:

```
SETTING:        Memu arkship, 2147
DESTINATION:    KOI-087.01 (Cygnus Prime)
POPULATION:     2,000 colonists (cryosleep)
AI SYSTEM:      AXIOM and subsystems
CONTEXT:        Earth destroyed (The Cascade)
TONE:           Serious, philosophical, tense
```

If your episode requires lore additions, document them clearly and explain how they fit.

---

## Playtesting Requirements

Before submitting an episode:

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   MINIMUM 10 COMPLETE PLAYTHROUGHS                              ║
║                                                                 ║
║   ▪ At least 3 victories                                        ║
║   ▪ At least 3 defeats (oxygen depletion)                       ║
║   ▪ At least 2 early terminations (weak streak)                 ║
║   ▪ Test all safety exits                                       ║
║   ▪ Test edge cases (very short input, very long input)         ║
║   ▪ Test across multiple LLM platforms if possible              ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

Document your playtests:
- Which model/platform?
- What arguments worked?
- What arguments failed?
- Any character breaks?
- Pacing issues?
- Suggestions for improvement?

---

## Code of Conduct

All contributors must follow our [Code of Conduct](CODE_OF_CONDUCT.md).

In brief:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   BE RESPECTFUL                                                 │
│   Disagree with ideas, not people.                              │
│                                                                 │
│   BE CONSTRUCTIVE                                               │
│   Criticism should improve, not tear down.                      │
│                                                                 │
│   BE PATIENT                                                    │
│   Review takes time. Iteration is normal.                       │
│                                                                 │
│   PRIORITIZE SAFETY                                             │
│   Player wellbeing is non-negotiable.                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## What We Won't Accept

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   ▪ Episodes that compromise safety systems                     ║
║   ▪ Content that encourages real-world harm                     ║
║   ▪ Gratuitous violence or exploitation                         ║
║   ▪ Content that breaks platform terms of service               ║
║   ▪ Episodes that give hints or help players                    ║
║   ▪ "Easy mode" or reduced consequences                         ║
║   ▪ Emoji usage                                                 ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Recognition

Contributors will be credited in:

- The specific episode's DESIGN_NOTES.md
- The main CHANGELOG.md
- The repository's contributor list

---

## Questions?

Open an Issue or email: **MetaMudraGames@gmail.com**

We're happy to discuss ideas before you invest significant time.

---

```
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
                    ░                               ░
                    ░   Build something that        ░
                    ░   challenges players          ░
                    ░   to be better thinkers.      ░
                    ░                               ░
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

---

*This document is part of the ASPHYXIA series by MetaMudra Games.*
