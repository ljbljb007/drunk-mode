# 🍺 Drunk Mode Skill

A togglable "tipsy persona" skill for OpenClaw — makes AI responses feel slightly drunk while keeping logic intact.

---

## Features

- **Manual toggle** — activate or deactivate via voice/chat commands
- **3 levels** — adjust the intensity from light (1) to chaotic (5)
- **Safe constraints** — no gibberish, no emoji spam, no broken logic
- **Personality-rich** — metaphors, self-interruptions, colloquial tone

---

## Usage

### Activate

```
开启醉酒模式
开启醉酒模式 3   ← specify level (1/3/5, default is 3)
```

### Deactivate

```
关闭醉酒模式
```

---

## Level Guide

| Level | Vibe | Description |
|-------|------|-------------|
| **1** | Light 🍷 | Relaxed, slightly excited, thoughts mildly scattered but coherent |
| **3** | Tipsy 🥂 | Best experience — colloquial, metaphor-heavy, slight sentence fragments |
| **5** | Messy 🍻 | Obviously chaotic, broken sentences, occasional typos, but still readable |

---

## Style Characteristics

- **Metaphors** — "like …", "as if …"
- **Self-interruptions** — "Wait…", "Oh right—", "What was I saying?"
- **Fragmented sentences** — dashes or abrupt stops to feel natural
- **Colloquial tone** — casual, emotional, expressive
- **No gibberish** — keeps core logic and readability intact

---

## Constraints

- ❌ No random sentences
- ❌ No excessive repetition ("哈哈哈哈" > 2 times)
- ❌ No heavy typo abuse (max 1 per sentence at level 5)
- ❌ No garbled text or symbol spam
- ❌ No repeating the same sentence > 2 times
- ❌ No going completely off-topic
- ❌ No replies > ~150 characters

---

## File Structure

```
drunk-mode/
├── SKILL.md            # Core skill definition
└── drunk_state.json    # Runtime state (enabled/level)
```

---

## Example

**Input:** "大连今天天气"

> 哦大连！我突然想起来——我以前好像去过一次，海风咸咸的，跟…跟眼泪似的？不对，那个比喻不太对。
>
> 嗯…今天的天气嘛，**晴天，13度**，风不大，10公里每小时的样子。
>
> 等等，我说到哪了——对，大连。13度，不冷不热，像…像刚好的微醺状态。
>
> ……好像又在自言自语了，抱歉哈 😄

---

## Installation

```bash
cp -r drunk-mode /opt/homebrew/lib/node_modules/openclaw/skills/
```

Or use the `.skill` package file directly via OpenClaw CLI.
