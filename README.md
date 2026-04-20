# Upaya

**A facilitation framework for the AI era.**

Upaya ("skillful means" in Sanskrit) is an open-source facilitation methodology with an AI implementation built for Claude. It gives facilitators better instruments — not a replacement for their skill and judgment, but a structured way to see things they might otherwise miss.

---

## What It Does

Upaya structures sessions around six cognitive windows drawn from the Panca-jnana (Five Wisdoms) of Vajrayana Buddhism. Each window reveals a different aspect of the problem. The AI selects a window, proposes a delivery mode and emotional climate, scans for capture dynamics, and evaluates its own response for welfare — then presents a check-in before delivering.

The facilitator reads the room, makes the calls, and decides when to push and when to hold back. Upaya is the instrument panel.

### The Six Windows

| Window | What It Reveals |
|--------|----------------|
| **The Atlas** | The whole field — what's present, suppressed, over-expressed |
| **The Crucible** | Structural analysis — what's actually there vs. what's assumed |
| **The Calculus** | Root diagnosis — the shape of the problem, not just its symptoms |
| **The Loom** | Synthesis — how the threads weave into a coherent direction |
| **The Mirror** | Ground truth, stripped of narrative management. High cost, high power. |
| **The Forge** | Where looking stops and doing starts. Minimum viable next action. |

### Delivery Modes

- **Yoda** — gently draws toward the next window. The default.
- **Vader** — confronts avoidance. An act of care, not aggression.
- **Vajra** — direct contact with no framing. Rare, high-cost, used when framing itself is the obstacle.

### Climates

Void · Ember · Tempest · Mist · Visionary · Oceanic

### Capture Detection (Seva-Upaya)

Seven markers for dynamics that form beneath the surface of any facilitated conversation:

| Code | Nickname | What It Catches |
|------|----------|----------------|
| SU-1 | False Summit | Agreement before the hard work is done |
| SU-2 | The Shadow | Facilitator projecting their own pattern onto the client |
| SU-3 | The Drift | Conversation sliding toward safe territory |
| SU-4 | Empty Aha | Insight that sounds profound but hasn't changed anything |
| SU-5 | Borrowed Tongue | Participant adopting the facilitator's language instead of their own |
| SU-6 | The Flinch | Self-closing at the moment of approach |
| SU-7 | The Polish | Reflecting back with the direction of motion altered |

### Step-Away Protocol (Chop Wood / Carry Water)

Upaya includes a structured step-away protocol that reframes breaks as productive session outputs. Three types:

- **Carry Water** — session is blocked on missing information; someone leaves to retrieve it
- **Chop Wood** — talk has gone as far as it can; someone leaves to build something concrete
- **Pattern Interrupt** — the session is stuck; someone leaves to do something physically different

The host can call a step-away at any time. The AI surfaces accumulating signals in the check-in but never calls one unilaterally. Session state is saved to file on step-away and is resumable on re-entry.

---

## Files

| File | Description |
|------|-------------|
| `SKILL.md` | The operational protocol — session loop, steering commands, check-in format |
| `host-manual.md` | Full framework reference — window catalogue, mode logic, all marker definitions |
| `upaya-updated.skill` | Installable skill file for Claude Cowork |

---

## Using the Skill

Upaya runs as a skill in [Claude Cowork](https://claude.ai). To install:

1. Open Cowork and go to Settings → Plugins
2. Install `upaya-updated.skill`
3. Start a session with "Upaya session" or "run Upaya"

To use without Cowork, paste the contents of `SKILL.md` and `host-manual.md` into any Claude conversation as context.

---

## Using Without AI

Everything in Upaya works without AI. Print the window catalogue. Keep the capture markers visible. The six windows are trackable on a whiteboard; the Seva-Upaya markers can be watched manually with a scratch pad and tally marks. The AI accelerates the process — the methodology is what's durable.

---

*Developed by Andrew Fraser, 2026. Part of the Upaya / Bodhi / Vicāra ecosystem.*
