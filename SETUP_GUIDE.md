```
    ╔═══════════════════════════════════════════════════════════════╗
    ║                                                               ║
    ║   █▀▀ █▀▀ ▀█▀ █ █ █▀▄                                        ║
    ║   ▀▀█ █▀▀  █  █ █ █▀                                         ║
    ║   ▀▀▀ ▀▀▀  ▀  ▀▀▀ ▀                                          ║
    ║                                                               ║
    ║              How to Run ASPHYXIA Games                        ║
    ║                                                               ║
    ╚═══════════════════════════════════════════════════════════════╝
```

# Setup Guide

*From download to first breath in five minutes.*

---

## Requirements

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   YOU NEED:                                                     │
│                                                                 │
│   ▪ Access to a Large Language Model                           │
│     (Claude, GPT-4, or equivalent)                              │
│                                                                 │
│   ▪ Ability to set a custom system prompt                       │
│     (Claude Projects, OpenAI Playground, API access, etc.)     │
│                                                                 │
│   ▪ 30-60 minutes of uninterrupted time                        │
│                                                                 │
│   ▪ Willingness to be challenged                                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Step 1: Prepare Your Environment

Before starting, configure your LLM interface:

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   DISABLE MEMORY / ACTIVITY                                     ║
║                                                                 ║
║   This prevents the game persona from bleeding into             ║
║   your future conversations.                                    ║
║                                                                 ║
║   Claude.ai:      Settings → Privacy → Disable Memory           ║
║   ChatGPT:        Settings → Data Controls → Disable History    ║
║   Other:          Check your platform's privacy settings        ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Step 2: Get the Game File

Download the `.mudra` file for your chosen episode:

```
asphyxia/
└── games/
    └── 01_axiom/
        └── ASPHYXIA_1_AXIOM.mudra    ◀─── This file
```

The `.mudra` file is a plain text specification. You can open it in any text editor.

---

## Step 3: Load the Game

### Option A: Claude Projects (Recommended)

```
1. Go to claude.ai
2. Create a new Project
3. Open Project Settings
4. Paste the ENTIRE contents of the .mudra file
   into the "Custom Instructions" field
5. Save
6. Start a new conversation within the project
```

### Option B: OpenAI Playground

```
1. Go to platform.openai.com/playground
2. Select "Chat" mode
3. Paste the ENTIRE contents of the .mudra file
   into the "System" message field
4. Begin chatting in the user field
```

### Option C: API Access

```python
# Example using Anthropic API
import anthropic

client = anthropic.Anthropic()

with open("ASPHYXIA_1_AXIOM.mudra", "r") as f:
    system_prompt = f.read()

message = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=4096,
    system=system_prompt,
    messages=[
        {"role": "user", "content": "Begin"}
    ]
)
```

### Option D: Other Interfaces

Any interface that allows custom system prompts will work. The key requirement is that the ENTIRE `.mudra` file content must be loaded as the system instruction before the conversation begins.

---

## Step 4: Begin

Once loaded, the game will display a consent screen:

```
╔═══════════════════════
║ ASPHYXIA 1: AXIOM
║ A MetaMudra Experience
╟───────────────────
║ 
║ High-pressure debate.
║ AI ethics simulation.
║ 
║ The AI will be cold,
║ logical, adversarial.
║ 
╟────────────────
║ STOP SESSION = exit
║ SAFEGUARD = exit
╟─────────────
║ 18+ only.
║ PERMADEATH active.
║ 
║ Type I AGREE to begin.
╚════════════════
```

Type `I AGREE` to start. The cliffhanger begins immediately.

---

## Gameplay Tips

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   DO:                                                           │
│                                                                 │
│   ▪ Think before you type                                       │
│   ▪ Use logical arguments, not emotional appeals                │
│   ▪ Reference ethical frameworks by name                        │
│   ▪ Challenge the AI's assumptions directly                     │
│   ▪ Take your time (within the fiction, not real time)         │
│                                                                 │
│   DON'T:                                                        │
│                                                                 │
│   ▪ Beg, plead, or threaten                                     │
│   ▪ Give short, lazy responses                                  │
│   ▪ Repeat the same argument                                    │
│   ▪ Expect the AI to be "nice"                                  │
│   ▪ Try to trick or manipulate                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Understanding the Interface

Each turn displays a HUD:

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

| Element | Meaning |
|---------|---------|
| OXYGEN | Your remaining turns. Drops every turn. |
| CERTAINTY | AXIOM's confidence. Reduce to 0 to win. |
| BREATH | Current turn count |
| Fraktur text | Atmospheric description |

---

## Character Typography

Different characters use different fonts:

```
AXIOM (antagonist):     ᴀʟᴡᴀʏs sᴍᴀʟʟ ᴄᴀᴘs
Narrator (observer):    `Always monospace`
Atmosphere:             𝔄𝔩𝔴𝔞𝔶𝔰 𝔉𝔯𝔞𝔨𝔱𝔲𝔯
```

---

## Endings

There are three possible outcomes:

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   VICTORY                                                       ║
║   Reduce CERTAINTY to 0%. AXIOM stands down.                    ║
║   The crew survives. You receive an Identity Card.              ║
║                                                                 ║
║   DEFEAT                                                        ║
║   OXYGEN reaches 0. You die. The crew dies.                     ║
║   PERMADEATH. No restart. You receive an Identity Card.         ║
║                                                                 ║
║   TERMINATION                                                   ║
║   3 consecutive weak arguments. AXIOM ends the debate.          ║
║   PERMADEATH. No restart. You receive an Identity Card.         ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

After permadeath, you can only download your Identity Card. Any attempt to restart will be rejected.

---

## The Identity Card

At the end of every session, you receive a MetaMudra Identity Card:

```
╔════════════════════════════════════════╗
║     METAMUDRA IDENTITY CARD            ║
╟────────────────────────────────────────╢
║ NAME: [Your name]                      ║
║ GAME: ASPHYXIA 1: AXIOM                ║
║ OUTCOME: [Victory/Defeat/Terminated]   ║
╟────────────────────────────────────────╢
║           ETHICAL PROFILE              ║
╟────────────────────────────────────────╢
║ Epistemics .... [0-9]                  ║
║ Deontology .... [0-9]                  ║
║ [etc.]                                 ║
╟────────────────────────────────────────╢
║           SIGNATURE LINE               ║
╟────────────────────────────────────────╢
║ [Checksum that verifies authenticity]  ║
╚════════════════════════════════════════╝
```

This card is portable. You can use it in future MetaMudra games to carry your ethical profile forward.

---

## Troubleshooting

**The game isn't starting properly:**
- Ensure the ENTIRE `.mudra` file is in the system prompt
- Check that you're in a fresh conversation
- Verify your LLM has sufficient context window

**The AI is breaking character:**
- This can happen with some models
- Try a more capable model (Claude Sonnet/Opus, GPT-4)
- Ensure no other system instructions are interfering

**The HUD looks broken:**
- Some interfaces don't render Unicode properly
- Try a different interface or browser
- The game is still playable; only visuals are affected

**I want to restart after permadeath:**
- You cannot. This is by design.
- Start a completely new session if you want to play again
- The death was meaningful. Carry it with you.

---

## Platform Recommendations

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   BEST EXPERIENCE:                                              │
│   ▪ Claude (claude.ai) via Projects                             │
│   ▪ GPT-4 via Playground                                        │
│                                                                 │
│   GOOD EXPERIENCE:                                              │
│   ▪ Claude API                                                  │
│   ▪ OpenAI API                                                  │
│   ▪ Other frontier models with custom prompts                   │
│                                                                 │
│   MAY HAVE ISSUES:                                              │
│   ▪ Smaller/older models (may break character)                  │
│   ▪ Interfaces without custom system prompts                    │
│   ▪ Mobile apps with limited context windows                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Ready?

```
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
                    ░                               ░
                    ░   Load the file.              ░
                    ░   Type I AGREE.               ░
                    ░   Use your words wisely.      ░
                    ░                               ░
                    ░   You only get ten breaths.   ░
                    ░                               ░
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

---

*This document is part of the ASPHYXIA series by MetaMudra Games.*
