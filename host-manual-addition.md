# Host Manual Addition
# INSERT AS SECTION 9 — shift current 9 → 10, 10 → 11, 11 → 12
# Reference file to add: copy chop-wood-carry-water.md into references/

---

## 9. Step-Away Protocol (Chop Wood / Carry Water)

Full protocol detail: `references/chop-wood-carry-water.md`

The step-away protocol reframes breaks as productive session outputs. There are three types of step-away, each mapped to a signal pattern:

- **Carry Water** — session is blocked on missing information; someone leaves to retrieve it
- **Chop Wood** — session has gone as far as talk can take it; someone leaves to build something concrete
- **Pattern Interrupt** — session is stuck; someone leaves to do something physically different

### Triggering

Step-aways can be triggered two ways:

**Host-initiated:** The host calls one at any time using plain language — `"step away"`, `"let's take a carry-water break"`, `"chop wood"`, `"pattern interrupt"`. Claude confirms the type, helps the host design a specific bounded task, and saves the session state before the participant leaves.

**AI-surfaced:** Claude watches for accumulating signals across all three categories (strong / medium / weak weighting, per the reference document). When signals reach a meaningful pattern, a suggestion appears in the check-in block under `Step-away:`. The AI does not call step-aways unilaterally — it surfaces; the host decides.

### Check-in Display

The `Step-away:` line appears in the check-in block only when signals are accumulating. When clear, the line is omitted entirely to keep the check-in readable.

Example when flagging:
```
Step-away: Carry water — 3 signals around missing Q3 data. Suggested.
```

Example when host calls one explicitly:
```
Step-away: Host-called. Chop wood — building wireframe for option B.
```

### Session State Document

When a step-away is called (either way), Claude saves a session state file before the participant leaves.

**Default location:** `dev/upaya/sessions/upaya-state-[YYYY-MM-DD-HHMM].md`

**Contents:**
- Topic and session opening context
- Rounds completed
- Windows visited (with round counts per window)
- Current window / mode / climate at point of step-away
- Metabolic readiness read
- Active Seva-Upaya flags
- Step-away type and specific task assigned
- Brief context note: what the conversation was doing when it paused, what the last open thread was

Claude names the file and tells the host its location before the participant steps away.

### Re-entry

When the participant returns, the host says `"resume"` or `"resume from [filename]"`. Claude loads the state document, restores context, runs a brief metabolic readiness re-read from the re-entry message, and the session continues from where it left off.

The state document is the source of truth for re-entry — not memory, not reconstruction. If the state file is missing or ambiguous, Claude tells the host before attempting to resume.

---
