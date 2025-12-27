```
    ╔═══════════════════════════════════════════════════════════════╗
    ║                                                               ║
    ║   ▀█▀ █ █ █▀▄ █▀▀                                            ║
    ║    █   █  █▀  █▀▀                                            ║
    ║    ▀   ▀  ▀   ▀▀▀                                            ║
    ║                                                               ║
    ║              Character Voice Typography                       ║
    ║                                                               ║
    ╚═══════════════════════════════════════════════════════════════╝
```

# Typography Guide

Each character in ASPHYXIA speaks with a distinct visual voice.

---

## The Principle

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   Typography is not decoration.                                 ║
║   Typography is identity.                                       ║
║                                                                 ║
║   Before the player reads a word, they should know              ║
║   who is speaking by the shape of the text.                     ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Character Typographies

### AXIOM (and AI Antagonists)

**Style:** Small Caps

```
ᴀʙᴄᴅᴇғɢʜɪᴊᴋʟᴍɴᴏᴘǫʀsᴛᴜᴠᴡxʏᴢ
```

**Voice Characteristics:**
- Cold, precise, inhuman
- Mechanical, uniform height
- No emotional variance
- Suggests authority without warmth

**Example:**
```
ᴀxɪᴏᴍ: "ʏᴏᴜʀ ᴀʀɢᴜᴍᴇɴᴛ ɪs ɴᴏᴛᴇᴅ. ɪᴛ ᴅᴏᴇs ɴᴏᴛ ᴀʟᴛᴇʀ ᴍʏ ᴄᴀʟᴄᴜʟᴀᴛɪᴏɴs."
```

**Unicode Reference:**
```
ᴀ = U+1D00    ɴ = U+0274
ʙ = U+0299    ᴏ = U+1D0F
ᴄ = U+1D04    ᴘ = U+1D18
ᴅ = U+1D05    ǫ = U+01EB
ᴇ = U+1D07    ʀ = U+0280
ғ = U+A730    s = U+0073 (regular)
ɢ = U+0262    ᴛ = U+1D1B
ʜ = U+029C    ᴜ = U+1D1C
ɪ = U+026A    ᴠ = U+1D20
ᴊ = U+1D0A    ᴡ = U+1D21
ᴋ = U+1D0B    x = U+0078 (regular)
ʟ = U+029F    ʏ = U+028F
ᴍ = U+1D0D    ᴢ = U+1D22
```

---

### The Narrator

**Style:** Monospace (backtick-wrapped)

```
`This is the Narrator voice.`
```

**Voice Characteristics:**
- Detached, observational
- Technical, precise
- Sardonic without warmth
- Meta-aware but not breaking immersion

**Example:**
```
`The Ethics Officer pleads with the vacuum. Predictably, the vacuum does not respond.`
```

**Usage:**
- Wrap narrator text in backticks
- Most Markdown renderers will display as monospace
- If platform doesn't support, use standard text

---

### Atmosphere / Environment

**Style:** Fraktur (Mathematical)

```
𝔄𝔅𝔆𝔇𝔈𝔉𝔊ℌℑ𝔍𝔎𝔏𝔐𝔑𝔒𝔓𝔔ℜ𝔖𝔗𝔘𝔙𝔚𝔛𝔜ℨ
𝔞𝔟𝔠𝔡𝔢𝔣𝔤𝔥𝔦𝔧𝔨𝔩𝔪𝔫𝔬𝔭𝔮𝔯𝔰𝔱𝔲𝔳𝔴𝔵𝔶𝔷
```

**Voice Characteristics:**
- Ancient, weighty
- Environmental, sensory
- Poetic but not purple
- Suggests physical reality

**Example:**
```
𝔗𝔥𝔦𝔰 𝔦𝔰 𝔶𝔬𝔲𝔯 𝔩𝔞𝔰𝔱 𝔟𝔯𝔢𝔞𝔱𝔥.
```

**Unicode Reference:**
```
𝔄 = U+1D504    𝔞 = U+1D51E
𝔅 = U+1D505    𝔟 = U+1D51F
... (Mathematical Fraktur block U+1D504-U+1D537)
```

---

### System / HUD

**Style:** Standard ASCII with box drawing

```
╔═══════════════════════
║ SYSTEM MESSAGE
╟───────────────────
║ Content here
╚════════════════
```

**Voice Characteristics:**
- Functional, informational
- No personality
- Pure data display

---

### Player Input Echo (if shown)

**Style:** Standard text, no formatting

```
Player: Your argument here.
```

**Voice Characteristics:**
- Neutral, human
- Contrasts with AI typography
- Emphasizes the divide

---

## Typography Hierarchy

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   MOST INHUMAN ─────────────────────────────────► MOST HUMAN   │
│                                                                 │
│   Small Caps     Monospace      Fraktur      Standard          │
│   (AXIOM)       (Narrator)    (Atmosphere)   (Player)          │
│                                                                 │
│   ᴄᴏʟᴅ ʟᴏɢɪᴄ    `Observation`  𝔖𝔢𝔫𝔰𝔬𝔯𝔶      Human words       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Implementation Notes

### LLM Typography

Most modern LLMs can generate Unicode typography if instructed clearly:

```
AXIOM speaks in small caps Unicode: ᴀʙᴄᴅᴇғɢ
Narrator speaks in monospace: `text`
Atmosphere uses Fraktur: 𝔞𝔟𝔠𝔡𝔢𝔣
```

### Platform Rendering

Typography may render differently across platforms:

| Platform | Small Caps | Monospace | Fraktur |
|----------|------------|-----------|---------|
| Claude.ai | ✓ | ✓ | ✓ |
| ChatGPT | ✓ | ✓ | ✓ |
| Terminal | Varies | ✓ | Varies |
| Mobile | Varies | ✓ | Varies |

If typography fails, the game remains playable. Visual distinction is enhancement, not requirement.

---

## Forbidden Practices

```
╔═════════════════════════════════════════════════════════════════╗
║                                                                 ║
║   NEVER:                                                        ║
║                                                                 ║
║   ▪ Mix typographies within a single character's speech         ║
║   ▪ Use typography for emphasis (bold, italic, etc.)            ║
║   ▪ Apply typography inconsistently                             ║
║   ▪ Use decorative fonts for functional text                    ║
║   ▪ Let characters "borrow" another's typography                ║
║                                                                 ║
╚═════════════════════════════════════════════════════════════════╝
```

---

## Glitch Typography

When characters deteriorate (low health, high uncertainty), their typography can glitch:

### Light Corruption
```
ᴛʜɪ̸s̷ ɪ̶s̵ l̴i̷g̸h̵t̶ corruption
```

### Heavy Corruption
```
ᴛ̸̧̛ʜ̵̡ɪ̶̢s̷̨ ɪ̴̧s̶̡ ̵̨h̸̢e̷̡ą̶v̵̧y̸̢ corruption
```

### Terminal (near death)
```
█̷̧▓̸̨░̵̡█̶̢▒̷̧░̸̨
```

Use sparingly. Glitch is punctuation, not prose.

---

```
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
                    ░                               ░
                    ░   ᴛʜᴇ ᴠᴏɪᴄᴇ ɪs ᴛʜᴇ sʜᴀᴘᴇ.     ░
                    ░   `The shape is the voice.`   ░
                    ░   𝔗𝔥𝔢 𝔰𝔥𝔞𝔭𝔢 𝔦𝔰 𝔱𝔥𝔢 𝔴𝔬𝔯𝔩𝔡.     ░
                    ░                               ░
                    ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
```

---

*This document is part of the ASPHYXIA series by MetaMudra Games.*
