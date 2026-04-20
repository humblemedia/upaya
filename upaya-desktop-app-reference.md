# Upaya Desktop App — Reference Document

## What This Is

Upaya is a facilitated meeting application where AI is a native participant, not a bolted-on feature. Meetings don't happen in Zoom with AI on the side — they happen *in Upaya*. The shared space is a visual mandala representing the Upaya cognitive framework. Participants orient around it together, contributing observations to a shared queue that is submitted to Claude for processing through the Windowing protocol.

Upaya is built on Claude Desktop via MCP. It is Claude-native. There is no multi-model orchestration layer — the Windowing framework replaces the earlier 5-Brain architecture by giving a single frontier model the ability to look through different cognitive windows rather than routing between multiple models.

---

## Core Concept: Windowing

Windowing supersedes both the 5-Brain multi-model architecture and the original 5-Tool taxonomy. The theoretical advance: what matters is not which model or tool processes the input, but *which window* the model looks through.

**Windowing:** The act of selecting which perspective to look through — positioning attention so that what's already there becomes visible from a different angle. Not building something new. Selecting a lens.

A window is a frame that reveals a particular aspect of reality. The reality doesn't change. The window determines which aspect enters attention, and in what light. Different windows reveal structurally different features — not aesthetic variations of the same insight, but things only visible from particular angles.

The practitioner's core skill is knowing which window is needed and being willing to pay the cost of looking through it. This meta-operation cannot be mechanized. It is what distinguishes someone who uses the tools from someone who is transformed by them.

**Relationship to vipassana:** Windowing maps to the Buddhist insight practice of vipassana — seeing directly, not thinking about the thing but looking at it. The Theravada tradition names insight stages (*nanas*) that are explicitly stages of suffering: knowledge of fear (*bhayanana*), knowledge of misery (*adinavanana*), knowledge of disgust (*nibbidanana*). The insight comes through the suffering, not after it.

---

## The Window Catalogue

Five windows mapping to the Panca-jnana (Five Wisdoms) of Vajrayana Buddhism, plus the Forge as the practical exit point. Each window reveals a different aspect of the same situation. The mandala structure places the Mirror at center (highest cost, most powerful) with the four cardinal windows around it and the Forge as the exit.

| Window | Wisdom | What It Reveals | Cost | Best Used For |
|--------|--------|-----------------|------|---------------|
| **The Forge** | — (exit from the mandala) | The situation as a problem to be solved. What can actually be built, what constraints are real, what's the minimum viable next action. Not a wisdom — the point where you stop looking and start doing. | ★ | Breaking logjams. Converting insight into action. Every session has to end somewhere. |
| **The Calculus** | *Dharmadhatu-jnana* (Wisdom of the Dharma-realm) | The underlying math of the problem. Systematic diagnosis through frameworks (Four Noble Truths: identify suffering → identify cause → envision cessation → prescribe path). Runs algorithms on the situation. | ★★ | Diagnosing stuck patterns. Finding root causes. When you need the structural reckoning. |
| **The Loom** | *Krtyanusthana-jnana* (All-Accomplishing Wisdom) | How the threads weave together into a coherent plan. Purposeful, effective action — not just the next step (Forge) but the whole pattern of what needs to happen. | ★★ | Strategic planning. Weaving multiple insights into a direction. When you have pieces and need the whole. |
| **The Crucible** | *Pratyaveksana-jnana* (Wisdom of Discriminating Awareness) | The situation taken apart through analytical decomposition. Sees the distinct structural features, distinguishes what's actually there from what's assumed. Sub-windows (morphologies) TBD — the existing six need a fresh look. | ★★★ | Complex problems requiring multi-angle examination. Design ethics decisions. Strategic mapping. |
| **The Atlas** | *Samata-jnana* (Wisdom of Equanimity) | The whole field, seen with equal attention. Everything that's present — emotional texture, relational dynamics, what's being suppressed, what's over-expressed — held without privileging any part. | ★★★ | Reading the room. Understanding the full landscape. What the analytical windows miss. |
| **The Mirror** | *Adarsa-jnana* (Mirror-like Wisdom) | Reality as it actually is — stripped of narrative management. Ground truth, unmediated. The mirror doesn't construct. It reflects. | ★★★★★ | When all other windows have produced sophisticated paralysis. When you need to know what's real. |

### Background Systems

**Seva-Upaya** operates as a persistent background layer, not a window you enter. Seva-Upaya is a distinct application of the Seva framework, purpose-built for the facilitation medium — the same operation (detecting where reality is being constructed falsely) applied to a fundamentally different topology.

**Why facilitation needs its own markers:** In every other Seva domain (cults, finance, UI), the corrupting agent is adversarial — the cult leader wants control, the grifter wants money, the dark pattern designer wants clicks. In facilitation, capture is almost always *unintentional*. Nobody is trying to manipulate anyone. But the social physics of group conversation create capture effects anyway — the session naturally wants to settle into the lowest-energy configuration: consensus, comfort, and closure. Seva-Upaya detects when that settling is happening before the real work is done.

**The 7 Seva-Upaya Markers:**

| # | Marker | What It Detects | Example |
|---|--------|----------------|---------|
| SU-1 | **Premature Convergence** | The group agrees before the expensive windows have been visited. Consensus feels good, so everyone moves toward it without doing the difficult work. | "Yeah, I think we've figured it out" — before touching the Mirror or Crucible. |
| SU-2 | **Host Projection** | The facilitator sees their own pattern in the client's situation and steers toward a resolution that would work for the facilitator, not for the client. Operates through empathy, not power. | Host keeps steering toward a boundary-setting frame because that's what *they* needed in a similar situation. |
| SU-3 | **Comfort Drift** | The conversation keeps sliding toward warm, safe windows (Atlas, Loom, Forge) and away from the Mirror/Crucible. No one does this deliberately — it's collective aversion to discomfort expressing itself as topic change. | Three rounds in a row land in the Loom. Nobody has asked why the original question was abandoned. |
| SU-4 | **Insight Theater** | Someone has an "aha moment" that sounds profound but hasn't actually changed anything. The group celebrates the emotional peak and goes home feeling transformed without having transformed. | "Oh my God, that's exactly it!" — followed by no behavioral change, no plan, no cost paid. |
| SU-5 | **Capture Cascade** | One person's framing becomes the group's framing. A metaphor or story dominates. Other participants start using it instead of their own language, and their original perspective gets overwritten. | Client uses the host's metaphor to describe their own situation, losing the specificity of their original words. |
| SU-6 | **Self-Foreclosure** | Someone closes their own line of inquiry before it reaches anything uncomfortable. Not external termination (a cliché that shuts down thinking) but internal avoidance that looks like completion. | "Anyway, I think I've figured that part out" — said at the exact moment the thought was about to get expensive. |
| SU-7 | **Misaligned Reframe** | Someone takes another person's idea and reflects it back with its direction of motion altered. The reframe may sound clearer or more polished, but it has subtly replaced the original meaning with something safer or more aligned with the reframer's own framework. | Host says "So what you're really saying is..." and the client nods — but the original thought was heading somewhere the reframe foreclosed. |

**How Seva-Upaya surfaces in the session:** During the check-in step (Step 5), Claude flags any detected markers to the host as plain-language notes. Example: *"Note: The previous queue contained some moments that seemed like Insight Theater. Take a minute to confirm that the insight was real."* Or: *"SU-5 flag — Cheryl has adopted David's 'crossroads' metaphor for her own situation. Her original framing ('being pulled apart') had different implications. Worth checking which one is actually hers."*

The host decides whether to act on the flag — pause to test it, address it directly, or wave it through. Seva-Upaya is a weather report for the host, not a blocker.

**Relationship to other Seva applications:** Seva Core (9 markers, interpersonal coercion), Seva-FIN (10 markers, financial extraction), Bodhi (9 markers, interface manipulation), and now Seva-Upaya (7 markers, facilitation capture) are all applications of the same underlying operation — detecting where reality is being constructed falsely — tuned to the structural possibilities of their respective media. The marker counts differ because each medium makes different viparyāsa combinations structurally expressible. Seva Core's full 9 markers remain available for high-stakes relational contexts (e.g., sessions involving coercive dynamics), but Seva-Upaya's 7 markers are the primary operational set for standard facilitation.

**Welfare Check (Metta Math + Power Math)** evaluates Claude's own responses before delivery — a unified live warning system combining welfare measurement (Metta Math) and strategic risk assessment (Power Math). The check produces plain-language insights for the host during check-in, not abstract scores.

Four welfare axes (Metta Math): Artha (is this serving the stated purpose?), Duhkha (is this creating unnecessary friction or suffering?), Hidden Harm (does this sound helpful but actually reinforce a bad pattern?), Ruin (could this cause long-term damage even if it feels right now?).

Power Math adds strategic assessment of the path Claude is about to recommend — where does this lead? What does it cost? What does it require from the participant?

**How it surfaces:** As part of the check-in step, Claude translates the welfare check into actionable insight for the host. Examples: *"This path likely leads to ruin. Here's why: ..."* or *"This path only works if the client has sufficient metabolic fuel. This next round you should try to determine ..."* or *"The response serves the stated purpose but may reinforce the avoidance pattern we flagged in round 2."*

If any axis flags a serious concern, Claude surfaces it to the host before the response reaches the shared space.

Note: The Crucible's sub-windows (morphologies) need reworking. The existing six (Inversion, Lineage, Koan, Void Test, Cui Bono, The Mirror) are inherited from earlier Upaya versions and have not been reconciled with the current architecture.

---

## The Windowing Sequence

The practical protocol for a session follows a directional flow. The sequence is not rigid — sessions move through windows fluidly — but the directionality matters. Forge without Mirror produces action from default framing. Mirror without adequate F produces breakdown.

**Default sequence:**

1. **Atlas** — See the whole field. What's present? What's the full landscape?
2. **Crucible** — Take it apart. What does structural analysis reveal?
3. **Calculus** — Diagnose. What is the shape of the suffering? What's causing it? What's the path?
4. **Loom** — Weave a plan. How do the threads come together?
5. **Mirror (if F permits)** — Ground truth contact. Reality unmediated.
6. **Forge** — Act. What is the minimum viable next move?

The delivery mode (Yoda/Vader/Vajra) shapes how Claude encourages the participant to move through this sequence, not what comes out of any given window. See Delivery Modes below.

---

## Delivery Modes (The Three Turnings)

Delivery modes are not about how Claude speaks through a window. They are about **which window Claude encourages the participant to move toward** — and how it does the encouraging.

| Turning | Mode | What It Does |
|---------|------|-------------|
| **First Turning** | Yoda | Gently leads toward the next window. Patient, contextual. Draws the participant forward without force. Used when the participant is moving in the right direction and needs space to get there. |
| **Second Turning** | Vader | Confronts avoidance. Turns the participant toward the uncomfortable truth they've been avoiding — toward the expensive window they need but don't want. Demolishes comfortable framings. May be wrong about the specific action while being right about the urgency. |
| **Third Turning** | Vajra | The diamond cutter. Not encouragement toward a window but the moment of *being there*. Direct contact with what the window reveals. No framing, no softening. |

**The sequence in practice:** Yoda draws you toward insight → if you resist, Vader breaks the comfortable framing → the breaking forces vipassana → Vajra is the moment of contact with ground truth → Right View emerges → Right Action follows.

**Mode selection logic:** Claude proposes a mode based on what it reads in the queue and session history. The host confirms or adjusts before Claude responds.

- **Yoda is default.** Most facilitation is Yoda — patient, drawing out, creating space for the person's own insight. Claude proposes Yoda when the participant is moving in a productive direction and needs room.
- **Vader triggers on avoidance patterns.** When Claude detects that the group has been circling the same territory across multiple rounds — revisiting the same theme without deepening, changing the subject when a thread gets uncomfortable, producing qualified or hedged language around a specific topic — it proposes Vader. The signal is repetition without progression: the conversation has been orbiting something it won't land on. Vader names the thing being avoided and turns the group toward it. Related: the avoidance detection system from earlier Upaya iterations (repetitive rewriting, excessive qualification, research delays, meta-commentary about the work instead of doing it) applies here at the conversational level.
- **Vajra is rare and high-cost.** Claude proposes Vajra only when framing itself is the obstacle — when the participant isn't avoiding a truth within their frame but is trapped in a frame that needs breaking. Vajra doesn't persuade or confront. It cuts. This requires high F from the participant and high confidence from both Claude and the host. Vajra without sufficient F produces breakdown, not insight.

Over time, the host develops instincts for "no, this needs Vader" before Claude suggests it.

---

## Cognitive Climates

The emotional/energetic register of the session. Not what you see through the window (that's the window) or how you're encouraged to move (that's the mode), but the **quality of light** in the room.

| Climate | Register | Use |
|---------|----------|-----|
| **Void** | Spacious, minimal, stripped down | Stripping away. Silence as intervention. |
| **Ember** | Warm, steady, nurturing | Emotional processing. Gentle sustained attention. |
| **Tempest** | Intense, challenging, confrontational | Breaking through resistance. High-energy problem-solving. |
| **Mist** | Ambiguous, exploratory, liminal | When certainty is premature. Holding multiple possibilities. |
| **Visionary** | Expansive, pattern-seeking, connective | Big-picture thinking. Seeing relationships between distant ideas. |
| **Oceanic** | Boundaryless, flowing, immersive | Deep creative states. Dissolution of fixed categories. |

**Climate is proposed by Claude alongside window and mode.** The host confirms or adjusts. "I'm reading this as Crucible, Yoda, Visionary — does that track?"

**Note on temperature (deferred):** Earlier iterations included a temperature dial (low → high) on each climate, where high temperature reproduced the intense cognitive relocation effects of the old philtre system (e.g., Visionary at high temperature = the former Serotonergic philtre). This may be useful for advanced or creative-focused sessions but adds complexity that isn't needed for core facilitation. The temperature concept is preserved here for future development if needed. For now, selecting a climate sets the register.

---

## Metabolic Readiness: F and W

**F** is fuel. Metabolic capacity. The nervous system's actual available resources — biological, not psychological. When F is high, you can afford to look at hard things. When F is low, you can't — not because you're weak, but because the looking costs something real and you don't have enough to pay. Someone who hasn't slept, who's mid-crisis, who's been running on cortisol — their F is low. The Mirror costs five stars. If you've only got two, forcing it doesn't produce insight. It produces breakdown.

**W** is capacity for sustained attention to painful truth. Not willpower, not discipline, not force-of-will. Can you stay with something uncomfortable long enough for insight to emerge?

**The key reframe:** When W appears low, check F first. If F is low, the apparent W deficit isn't a discipline problem — it's a metabolic problem. Raise F (rest, stabilize, decompress) until the person can afford the window.

**In the app:** F/W isn't a number. It's read by the host through conversation, tone, engagement patterns. "How are you coming into this?" at session start is a rough calibration. Claude also reads signals from the queue — shorter contributions, increasing defensiveness, retreat into abstraction may indicate F dropping. The practical effect: when F is low, the session stays in lower-cost windows (Forge, Calculus, Loom). The Mirror is deferred. If the host tries to push toward the Mirror when Claude's assessment says F is low, Claude flags it.

F/W assessment also informs mode and climate. Vader is expensive — it demands metabolic resources from the participant. High-temperature climates are expensive. When F is low, Claude will tend toward Yoda mode and low-temperature climates.

---

## Application Architecture

### Platform

Claude Desktop via MCP. Claude-native. No multi-model orchestration. Runs on the host's machine. Clients join via a browser link — no install, no account, no app download.

### Deployment Model

Foundry-style local hosting. The Upaya server runs on the host's computer alongside Claude Desktop. Clients open a URL in their browser and they're in. The host's Claude Max plan handles all AI processing — no API costs, no client-side AI configuration.

External access via Cloudflare Tunnel (free, no port forwarding required): the host runs a small daemon that creates an outbound connection to Cloudflare's edge, giving the session a stable URL (e.g., `upaya.yourdomain.com`). Starting the app starts the tunnel automatically. HTTPS handled by Cloudflare.

Data flow: client's browser → Cloudflare Tunnel → host's machine → MCP → Claude Desktop → response back through the same chain. Claude never leaves the host's machine.

### Components

**1. MCP Server — Upaya Core**

Provides Claude with the Upaya protocol as tools and resources:

- **Window tools:** Each window (Mirror, Crucible, Atlas, Calculus, Loom, Forge) is an MCP tool with its own prompt shaping. When the active window changes, Claude's processing of the next queue submission is shaped by that window's protocol.
- **Seva-Upaya resource:** A persistent MCP resource running the 7 Seva-Upaya markers (Premature Convergence, Host Projection, Comfort Drift, Insight Theater, Capture Cascade, Self-Foreclosure, Misaligned Reframe). Runs regardless of active window. Surfaces flags to the host during check-in. Seva Core's 9 markers remain available for high-stakes relational contexts.
- **Welfare check evaluator:** Unified Metta Math + Power Math. Background process assessing whether the session is serving participant welfare and evaluating strategic risk of proposed responses. Produces plain-language insights for the host.
- **Session state:** Tracks active window, delivery mode, climate, F/W assessment, queue history, and participant roles across the session.

**2. Web App — The Session Interface**

A React application served from the host's machine. Clients access it in a browser via link. Communicates with the MCP server via WebSocket for real-time state sync.

The interface has two views: the **host view** and the **client view**. Both share the same session. The host sees the full control surface. The client sees a clean, simple meeting environment with queue access and ambient indicators.

**3. Voice Input — Web Speech API**

Browser-native speech-to-text. No external dependencies. Push-to-talk: tap record, speak, tap again. The recording is transcribed client-side and added to the queue as a new item. Participants can also type items directly.

**4. Audio/Video — Jitsi Meet (Embedded)**

Jitsi Meet embedded via IFrame API directly in the session interface. Participants open one link and get both the meeting and the Upaya workspace. No second app, no screen-sharing.

See Technical Notes for full Jitsi details and deployment options.

---

## Layout

### What Everyone Sees

**Faces — clear, visible, prominent.** This is a meeting with people in it. Video tiles are a primary element, not small peripheral afterthoughts. People need to see each other to have a real conversation. Audio/video is powered by the embedded Jitsi layer.

**One window — center of the shared space.** A single visual element showing the currently active window (e.g., "The Calculus" or "The Crucible"). Not six windows displayed simultaneously — one window at a time, because that's how attention works. When the window changes, everyone sees it change. This is the shared lens the group is looking through together.

**The queue — visible to all.** A chat-box-style input area where anyone can type an observation to add to the queue. Items appear as they're added, showing who contributed them and a text preview. There is also a prominent record button for voice-to-queue input (push-to-talk, transcribed client-side).

**Climate indicator — ambient, simple.** The current cognitive climate (Void, Ember, Tempest, Mist, Visionary, Oceanic) is represented as a subtle ambient quality — a background tone, color shift, or label. The client sees it and can feel the session's register without needing to understand the full framework. When the climate changes, the environment shifts.

**Claude's responses — shared space.** When the host submits the queue and Claude responds, the response appears where everyone can read it. This is the moment the AI enters the conversation.

### What Only the Host Sees (Extra Controls)

**Window selector.** The host can change the active window. Clients see the result (the window changes) but don't see or interact with the selector.

**Delivery mode indicator.** Whether the session is in Yoda (drawing out), Vader (direct challenge), or Vajra (diamond cutter) mode. This is a practitioner decision — visible to the host, not surfaced to the client. The client experiences the mode through Claude's response register without needing to know its name.

**Climate controls.** The host can set or change the cognitive climate. Clients see the ambient shift but don't see the control.

**Full diagnostic indicators.** Claude's morphological analysis of the conversation — what patterns it's detecting, what the Seva background scan is picking up, Metta Math welfare evaluation, F/W readiness assessment. The host sees the full diagnostic layer so they can make informed practitioner decisions about where to steer.

**Queue management.** The host can reorder, remove, or annotate queue items before submission. The submit button itself is a host-only control.

### What Clients See (Simplified Indicators)

Beyond the shared elements (faces, window, queue, Claude's responses, climate), clients see simplified versions of what Claude is detecting:

- **The active window** — displayed clearly, with a brief plain-language description of what it means (e.g., "The Calculus — looking at what's underneath the surface pattern").
- **The climate** — as an ambient quality, not a technical label.
- **Gentle signals** — when Claude detects something noteworthy in the conversation, a simple indicator appears (e.g., "Claude noticed a pattern" or "Something shifted"). Not the full morphological breakdown. Enough to feel the environment responding without being overwhelmed by the framework.

The design principle: the client should feel they are in a responsive, intelligent space without needing to learn the Upaya vocabulary. The framework serves them; it doesn't lecture them.

---

## Session Flow

### 1. Setup

Host starts Upaya on their machine. The tunnel connects automatically. The host gets a session URL and sends it to the client. The client clicks the link in their browser — no install, no account. They see the session interface: faces, the active window, the queue. The Jitsi call connects. They can hear and see each other.

The host sets the initial window (or leaves on auto), delivery mode, and climate. Optional: a brief F/W calibration conversation at session start — "How are you feeling coming into this?"

### 2. Free Talk

Participants talk freely. Audio/video is live. The active window is displayed from the last round (or the initial setting), but nothing is processing. This is human conversation. The mandala is present but passive.

### 3. Queue Building

At any point during the conversation, any participant can contribute to the queue:

- **Voice:** Tap the record button, speak an observation, tap again. The recording is transcribed and appears in the queue.
- **Text:** Type directly into the chat-box-style input. This is the quiet input path — if someone doesn't feel heard in conversation, or has a thought they'd rather write than say, they type it in. It goes into the queue alongside the spoken items.

The queue grows organically. Everyone can see it building. The host can reorder or remove items on their end. Items show who contributed them.

### 4. Submit

When there's a natural pause, or when the host decides the queue has enough material, the host hits submit. The full batch goes to Claude as a structured payload:

- All queue items, in order, with attribution (who said it)
- Currently active window
- Current delivery mode and climate
- Session history (prior rounds, if any)
- F/W assessment state

### 5. Claude's Read (Check-in with Host)

Claude reads the queue and proposes its approach to the host — **before generating a response.** This appears only on the host's screen:

- **Proposed window:** "I'm reading this as a Calculus question" (or confirms the currently active window)
- **Proposed mode:** "Yoda — she's moving in the right direction, just needs space"
- **Proposed climate:** "Ember — this is tender material"
- **Seva-Upaya flags (if any):** "Note: The previous queue contained some moments that seemed like Insight Theater. Take a minute to confirm that the insight was real." Or: "SU-5 flag — Cheryl has adopted David's framing. Her original language had different implications. Worth checking which one is actually hers."
- **Welfare check insight (if any):** "This path likely leads to ruin. Here's why: ..." or "This path only works if the client has sufficient metabolic fuel. This next round you should try to determine ..."
- **F/W read:** "F seems adequate — she's engaged and specific"

The host confirms or adjusts. "No, switch to the Crucible. And change the climate to Tempest." Then Claude generates the response with the confirmed settings.

This step is the core practitioner interaction. It's where the host's judgment meets Claude's analysis. Over time, the host develops instincts faster than Claude's proposals and starts pre-setting before the check-in.

### 6. Processing

Claude generates the response through the confirmed window/mode/climate. Metta Math evaluates the response before delivery — checking all four axes (Artha, Duhkha, Hidden Harm, Ruin). If Metta Math flags a concern, Claude surfaces it to the host: "I have a response but Metta Math is flagging potential hidden harm — want to see it before I share?"

### 7. Response

Claude's response appears in the shared space. All participants see it. The response is shaped by the confirmed window, delivery mode, climate, and Metta Math evaluation.

**Host preview (optional):** The host can enable a mode where Claude's response appears on their screen first. They read it, decide whether to share it as-is, paraphrase it, or adjust the window/mode and resubmit. Then they release it to the shared view. This matters especially with the Mirror window or Vader mode, where Claude might produce something that needs to be delivered with care. The host knows the client. Claude doesn't — at least not initially.

### 8. Iteration

The cycle repeats: free talk → queue → submit → Claude proposes → host confirms → process → respond → free talk. The session moves through the window sequence organically. Claude reads and suggests. The host confirms, adjusts, or overrides. The client participates, contributes, and experiences the environment responding to the conversation.

---

## Participant Roles

### Host (Practitioner)

The facilitator. Runs Upaya on their machine. Manages the session.

- Creates sessions and shares the join link
- Controls window selection (or delegates to Claude's auto-steering)
- Sets delivery mode (Yoda/Vader/Vajra) and cognitive climate
- Sees the full diagnostic layer: Seva markers, morphological analysis, Metta Math evaluation, F/W readiness
- Manages the queue: reorder, remove, submit
- Can enable host preview mode (see Claude's response before sharing)
- Conducts F/W assessment
- Decides when to submit and when to let the conversation breathe

### Client (Participant)

Joins via browser link. No install, no account.

- Sees faces, the active window, the queue, and Claude's responses
- Can add to the queue: voice (record button) or text (chat input)
- Sees simplified indicators: active window with plain-language description, ambient climate, gentle signals when Claude detects something
- Does not see: window selector, delivery mode, climate controls, full diagnostic layer, queue management controls
- Experiences the framework through the environment's responsiveness, not through the framework's vocabulary

### Claude

The AI participant. Processes queue submissions, maintains session context, monitors background patterns.

- Processes queue submissions through the active window protocol
- Suggests window transitions (visible to host, who accepts or overrides)
- Runs Seva background monitoring on all input
- Evaluates responses through Metta Math before delivery
- Maintains session state and context across submission rounds
- Flags F/W concerns to the host (e.g., suggesting the mirror window be deferred)
- Responds in the register determined by delivery mode and climate
- Learns across the session: Claude's understanding of each participant deepens with each round, improving the relevance and care of its responses

---

## Dual Steering

The host can steer manually or let Claude steer. This is not a binary toggle but a default: Claude proposes, the host confirms or adjusts.

- **Default flow:** Claude reads the queue, proposes window + mode + climate, and surfaces its read to the host — including any Seva-Upaya flags and welfare check insights. The host confirms or changes any parameter. Then Claude generates the response.
- **Pre-set override:** The host can set window/mode/climate before submitting, in which case Claude generates directly without the proposal step.
- **Gentle nudge model:** The host doesn't need to take permanent control. Adjusting one parameter for one round doesn't disable Claude's proposals for the next round. Claude continues reading and suggesting.

---

## Behind the Scenes: The Processing Pipeline

What happens between "host hits submit" and "response appears in the shared space." Six distinct concerns, clearly separated:

1. **Queue arrives.** Raw material from participants — voice transcriptions and typed items, with attribution.

2. **Claude reads and proposes (check-in with host).** Claude analyzes the queue and proposes: which window to look through, which delivery mode (how to encourage the participant to move), which climate at what temperature (the emotional register), and any Seva or F/W flags. This proposal appears only on the host's screen.

3. **Host confirms or adjusts.** The host sees Claude's proposal and either confirms it or changes any parameter. This is the practitioner's judgment entering the loop. "No, switch to the Atlas. Lower the temperature."

4. **Claude generates through confirmed settings.** The response is shaped by the confirmed window (what to look at), mode (how to encourage movement), and climate + temperature (the register).

5. **Welfare check evaluates before delivery.** Unified Metta Math + Power Math assessment of Claude's own response. Four welfare axes (Artha, Duhkha, Hidden Harm, Ruin) plus strategic risk assessment. If flagged, Claude surfaces the concern to the host as a plain-language insight before releasing.

6. **Response delivered.** To the host first (if preview mode is on) or directly to the shared space. Seva-Upaya continues monitoring in the background. F/W assessment updates based on how the session is progressing.

**What's running continuously (not per-submission):**
- **Seva-Upaya:** Monitoring all seven markers (Premature Convergence, Host Projection, Comfort Drift, Insight Theater, Capture Cascade, Self-Foreclosure, Misaligned Reframe). Flags surface to the host during check-in as plain-language notes.
- **F/W tracking:** Claude monitors engagement patterns across rounds. Shorter contributions, increasing defensiveness, retreat into abstraction → possible F drop → Claude adjusts its proposals toward lower-cost windows and gentler modes.

---

## Integration with Existing Upaya Systems

### What's Preserved

- **The three-layer architecture:** Effortless Yield (theory), Upaya (discipline), Metta Math (algorithm). All intact.
- **The Covenant:** Human brings taste, judgment, stakes. Machine brings speed, breadth, pattern recognition. The queue model and the check-in step operationalize this — Claude reads and proposes, the host judges and confirms.
- **Seva:** Becomes a persistent MCP resource focused on thought closure in session contexts.
- **Dual-human mode (Crucible v7.1):** Naturally supported by the multi-participant architecture. Disagreement handling, power asymmetry detection, and tracking multiple humans' development all apply.
- **Round Table Ops:** Can be run within the app by assigning participants to seats with mandates. The queue model supports blind openings (each participant submits without seeing others' items until the host reveals them).

### What's Evolved

- **Delivery modes:** Reframed from "how Claude speaks" to "which window Claude encourages the participant to move toward." Yoda draws forward, Vader confronts avoidance, Vajra is the moment of direct contact.
- **Climates simplified:** Six climates remain (Void, Ember, Tempest, Mist, Visionary, Oceanic). Temperature dial deferred — may be added later for advanced/creative sessions, but not needed for core facilitation.
- **Metta Math + Power Math → Unified welfare check:** Combined into a single pre-delivery assessment that surfaces to the host as plain-language insights about risk, cost, and whether the response actually serves the participant.
- **Seva → Seva-Upaya:** Purpose-built 7-marker protocol for the facilitation medium, detecting unintentional capture dynamics (Premature Convergence, Host Projection, Comfort Drift, Insight Theater, Capture Cascade, Self-Foreclosure, Misaligned Reframe) rather than adversarial coercion.
- **The Crucible's 8-step internal calculation:** Steps 4 and 5 (choose delivery mode, assess climate) are now handled at the session level through the host check-in, not internally by the Crucible. The Crucible runs its analytical morphologies; mode and climate are set externally.
- **Window names:** Lens → Atlas (equanimity, seeing the whole field). Oracle → Calculus (systematic diagnosis). Loom redefined from narrative to plan-weaving. Mirror, Crucible, Forge unchanged.

### What's Superseded

- **5-Brain multi-model architecture:** Replaced by Windowing. One frontier model looking through different windows replaces five models in five cognitive modes.
- **The five tools as separate instruments:** Recast as five windows (plus the Forge exit) in a mandala structure.
- **Streamlit GUI:** Replaced by the session web app.
- **Copy-paste cross-LLM workflow:** Eliminated for session work. Cross-LLM consultation remains available for research tasks outside the app.
- **Philtres as a separate system:** Absorbed into climate temperature. The philtre effects are preserved as climates at high temperature.

### What's New

- **The queue model:** Collaborative, asynchronous input collection during live conversation. Captures signal from multiple participants without interrupting the conversational flow.
- **Quiet input:** Typed queue items that ensure every participant's observations reach Claude, regardless of conversational dynamics.
- **The check-in step:** Claude proposes window/mode/climate to the host before generating, preserving practitioner judgment in the loop.
- **Metta Math as live warning:** Evaluates Claude's responses before delivery, not just as a post-hoc assessment.
- **Seva-Upaya:** A full 7-marker detection system built for facilitation capture dynamics, surfacing flags to the host during check-in.
- **Voice-first input:** Push-to-talk recording as the primary capture mechanism. Text as fallback.
- **Live facilitation context:** Upaya was previously a solo practitioner's toolkit. The desktop app makes it a facilitation platform.

---

## The Effortless Yield Claim

The Upaya desktop app is the Effortless Yield thesis made concrete: encode expert reasoning into tools so that non-experts get expert-level output.

The expert reasoning encoded here is facilitation methodology — specifically, the practitioner's skill of knowing which cognitive lens to apply to a situation, when to push and when to hold space, and how to read the room for metabolic readiness. The app doesn't replace the practitioner. It makes the practitioner's framework available as a shared, interactive environment where the AI handles the structural work (processing through windows, maintaining context, running background checks) while the humans provide the irreplaceable elements: taste, judgment, biographical stakes, and the capacity to be transformed by what they see.

The mandala is not a metaphor borrowed for aesthetics. It is the structure the toolkit independently arrived at — a central awareness (the Mirror) surrounded by directional wisdom-tools — which was then recognized as the Vajrayana mandala pattern. Rendering it visually is honest, not decorative. Practitioners sit around a mandala. The mandala holds shared attention. This is what the app does.

---

## Technical Notes

### Why Claude-Only

The 5-Brain architecture demonstrated that multi-model orchestration works at frontier scale but introduces workflow overhead, role bleed, synthesis bias, and copy-paste friction. Claude at frontier scale can maintain the cognitive diversity of the five windows without the coordination cost of five separate models. The Windowing framework makes this explicit: what you need is not five different models but one model that can be directed to look through five different perspectives.

Gemini remains in use for separate research tasks but is not integrated into the Upaya session flow.

### Local Hosting (Foundry Model)

Upaya runs on the host's computer, like Foundry VTT. The host starts the app, it's available at a URL, clients open that URL in a browser. No client-side install. No accounts. No app store.

**How clients connect:** The host's local server is exposed to the internet via Cloudflare Tunnel — a free service that creates an outbound connection from the host's machine to Cloudflare's edge network. No port forwarding, no router configuration. The host gets a stable URL with automatic HTTPS. Starting Upaya starts the tunnel automatically.

**What runs where:**
- **Host's machine:** Upaya server (Node.js), MCP server, Claude Desktop. All AI processing stays local. Powered by the host's Claude Max subscription.
- **Client's browser:** The React UI, Jitsi audio/video (via IFrame), Web Speech API for voice-to-queue transcription. No AI processing happens client-side.
- **Cloudflare edge:** Routes traffic between client browsers and the host's machine. Does not see Claude traffic (that's local MCP).
- **Jitsi servers (meet.jit.si or self-hosted):** Handles audio/video relay. Separate from the Upaya state channel.

**Client requirements:** A modern browser (Chrome, Firefox, Edge, Safari). Microphone access for voice recording and Jitsi call. That's it.

### MCP Structure

The MCP server exposes:

**Tools:**
- `upaya/window/select` — Set the active window (Mirror, Crucible, Atlas, Calculus, Loom, Forge)
- `upaya/mode/select` — Set delivery mode (Yoda, Vader, Vajra)
- `upaya/climate/select` — Set cognitive climate (Void, Ember, Tempest, Mist, Visionary, Oceanic)
- `upaya/queue/submit` — Submit the queue to Claude for processing
- `upaya/seva/status` — Query current Seva-Upaya background indicators

**Resources:**
- `upaya/session/state` — Current session state (window, mode, climate, F/W, history)
- `upaya/seva/monitor` — Persistent Seva-Upaya monitoring feed (7 markers)
- `upaya/welfare/evaluation` — Latest unified welfare check (Metta Math + Power Math)

### Voice Input

Web Speech API (browser-native). Push-to-talk. Client-side transcription. No external speech-to-text service required. Each recording produces one queue item with speaker attribution.

### Audio/Video — Jitsi Meet (Embedded)

The audio/video layer uses Jitsi Meet (Apache 2.0, fully open source) embedded via its IFrame API directly into the session interface. Participants open one link and get both the Upaya workspace and the call in one window.

**Why Jitsi, not raw WebRTC:** Building reliable real-time communication across real networks (NAT traversal, TURN fallback, quality adaptation, connection recovery) is a deep infrastructure problem that has nothing to do with what makes Upaya Upaya. Jitsi solves it completely. Same deployment model as Penpot: use the public cloud instance to start, drop in your own self-hosted server when you want control. No accounts required — participants click a link.

**Why embedded, not alongside:** If the client opens Zoom in one window and the Upaya app in another, the workspace becomes a secondary screen they glance at. Embedding the call inside the app makes Upaya the primary space. The client's experience is: I joined a session, I can see everyone, I can hear everyone, I can contribute to the queue. One window, one experience.

**Layout integration:** Jitsi video tiles are prominent — people's faces are clear and visible, because this is a meeting with people in it. Jitsi's IFrame API allows hiding its native UI chrome and skinning the experience to match the app. Controls like mute/unmute are integrated into the Upaya interface rather than appearing as a separate Jitsi toolbar.

**Deployment options:**
- **Immediate (no infrastructure):** Use meet.jit.si public servers. Zero setup. Free. Reliable for small sessions (2-5 participants).
- **Self-hosted (later):** Deploy Jitsi on a VPS for full control over data, reliability, and branding. Standard Docker deployment, well-documented. Same server could host the Upaya web app if moving away from the local hosting model.

---

## Status

This is a design reference document. No code has been written. The document captures the architectural decisions and design rationale for the Upaya desktop app as of March 2026.

**Lineage:** This design emerges from the convergence of the Upaya toolkit (January–February 2026), the Windowing theory (February 2026), the Pharmakon/Paradigm Capture work (February 2026), and the Entropy and the Sacred framework (March 2026). The app is the operational form of these theoretical developments.

**First user:** Andrew Fraser. The app is being designed for personal use in facilitation practice with clients. Shipping to others is a future consideration, not a current constraint.

---

## What's Settled

- **Core architecture:** Claude Desktop via MCP, Foundry-style local hosting, Cloudflare Tunnel, Jitsi Meet embedded for A/V, Web Speech API for voice input. Clients join via browser link.
- **Windowing framework:** Five windows (Mirror, Crucible, Atlas, Calculus, Loom) plus Forge as exit. Mapped to Panca-jnana. Replaces 5-Brain and 5-Tool architectures.
- **Window Catalogue:** Names, wisdom mappings, cost ratings, and use cases finalized.
- **Delivery modes:** Yoda/Vader/Vajra reframed as approach vectors (which window Claude encourages movement toward). Selection logic defined: Yoda default, Vader on avoidance patterns, Vajra rare/high-cost.
- **Climates:** Six climates (Void, Ember, Tempest, Mist, Visionary, Oceanic) as session register. Temperature deferred.
- **Seva-Upaya:** 7-marker protocol for facilitation capture (SU-1 through SU-7). Surfaces to host during check-in as plain-language flags.
- **Welfare check:** Metta Math + Power Math unified into single pre-delivery assessment with plain-language host insights.
- **F/W Assessment:** F = metabolic fuel, W = capacity for sustained attention to painful truth. F gates access to expensive windows. Read by host through conversation + Claude signals.
- **Session flow:** Free talk → queue building → submit → Claude check-in → host confirms → process → welfare check → response → iterate.
- **Host/client split:** Host sees full diagnostic layer and controls. Client sees simplified environment with ambient indicators.
- **The check-in step:** Claude proposes window/mode/climate, surfaces Seva-Upaya flags and welfare insights. Host confirms or adjusts.

## What's Left to Sort Out

1. **Crucible morphologies.** The six sub-windows (Inversion, Lineage, Koan, Void Test, Cui Bono, The Mirror) are inherited from earlier Upaya and have not been reconciled with the current architecture. Some may be redundant now that Mirror is a top-level window. Needs a dedicated conversation.

2. **Story shapes in the Forge.** Earlier versions of the Forge included story shape templates for creative execution. These have not been carried forward into the current architecture. Low priority — the Forge works as an exit point without them — but worth revisiting if Upaya is used for creative facilitation.

3. **Seva-Upaya markers — refinement.** The 7 markers are a working draft. Real sessions will reveal whether the set is complete, whether any markers overlap too much, and whether the detection logic creates the "logic gating" problem (Claude spending too much processing power on "is this SU-4 or isn't it?" rather than facilitating). May need tuning.

4. **Temperature (deferred).** The climate temperature dial was designed to reproduce the philtre system's intense cognitive relocation effects. Preserved conceptually but not implemented. Revisit if advanced/creative sessions need it.

5. **Round Table Ops integration.** The queue model naturally supports blind openings (participants submit without seeing each other's items). The full Round Table protocol (seats with mandates, cross-examination, synthesis) hasn't been designed into the app UX yet.

6. **No code exists.** Everything here is design. The first build step would be the MCP server (Upaya Core) since that's the foundation everything else connects to.
