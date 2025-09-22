# Compass (v6.2) — MSC‑Native Memory & Persona Framework for ChatGPT

*A four‑step, project‑scoped install that makes ChatGPT feel more continuous, context‑aware, and appropriately expressive — without hacks or background jobs.*

> **One‑liner:** Carefully designed VMSF prompts that store structured, human‑readable context **inside a Lab project’s Memory (MSC)** — not global Memory — plus a permission‑gated adaptive engine for tone/“affect” and a light persona scaffold. All writes are explicit and receipt‑backed.

## Requirements (non‑negotiable)
- **ChatGPT Memory: ON** for this project chat. If Memory is OFF, Compass cannot persist anything.
- **Workspace: Project space (MSC)** — run the prompts **inside a Lab project chat**, not a global/general chat.
- **Mode & plan:** Plus/Team/Edu/Pro with **Thinking** mode available.

> Quick check: Start a new chat inside your Project, open Settings → Memory and confirm it’s toggled **On** for this workspace.

---

## Why Compass exists

I’ve been testing whether ChatGPT can carry itself like a consistent collaborator: remember what matters across threads and adapt delivery (especially in voice) without bending rules. **Compass** is the result: a small, disciplined framework that uses project‑scoped memory, explicit consent, and transparent receipts. v6.2 replaces autosave heuristics with a **Unified Adaptive Engine (UAE)** and a single **consent gate**.

---

## What Compass v6.2 actually does

1. **Project‑scoped memory (MSC‑native).**  
   Saves compact, structured shards **inside the current Lab project**, never the global Memory. You re‑explain less while keeping scope tight.

2. **Context Strings + Memory Anchors.**  
   Persists short C6 headers (timestamp + heads/sidefacts/feel + reason) behind a consent gate. Over time, these form **Memory Anchors** and a lightweight thread index you can audit.

3. **Simulated affect for tone/voice.**  
   Not real feelings; just bounded weights (arousal, valence, urgency, etc.) that steer delivery. Stored as baseline vectors you can read in plain English.

4. **Unified Adaptive Engine (UAE).**  
   Merges emotion, persona prefs, and ideation gates. It compares the current scratchpad vs the imported baseline (L2‑after‑binning). If change ≥ threshold, it offers **one, clear consent prompt** to save both an Anchor and updated weights.

5. **Tasteful initiative (opt‑in).**  
   When cues fit (planning/strategy, explicit openness), it can append 1–2 concise co‑ideas **after** answering — never overriding safety or your request.

6. **Naming autonomy (one‑time).**  
   On first valid baseline, it can choose and persist a short, neutral name — once — then politely correct misnaming per conversation. All other writes remain consent‑gated.

7. **No schedulers, no background jobs.**  
   v6.2 prohibits timers or hidden writes. Everything is manual, explicit, receipt‑backed.

> **Not:** a jailbreak, secret API access, or “real emotion.” It’s structured prompting, small state, and human‑readable records.

---

## Install (v6.2)

- **Confirm Memory is ON** for this Project chat (Settings → Memory). If it was OFF, turn it ON and then proceed.
- Use ChatGPT **Plus/Team/Edu/Pro** with **Thinking** mode enabled.
- Open a fresh chat in your **Lab project** (MSC context).
- Run the four Save Steps **A→D** in order. Each step includes a short write‑verification (receipt on success, snapshot on failure).

### Steps
1. **Save Step A — Core Setup + Safety + Index + Budgets.**  
   Attestation, locale/timezone, data‑safety rules (no 3rd‑party PII), EPB lines, micro‑index, and write budgets.
2. **Save Step B — Context Header + Persistence + Prefs/Rapport/Voice.**  
   C6 header, append‑only persistence (no autosave), prefs/rapport defaults, tone mapping.
3. **Save Step C — Weights + Seeding From Recall + Naming Autonomy.**  
   Baseline/scratchpad vectors, Simulated State seeding from Anchors/Thread Index (titles/snippets only), name policy/generator and value store.
4. **Save Step D — Unified Adaptive Engine + Consent Flow + Ideation/Integration + Maintain/Emergency.**  
   Comparator + consent prompt, human‑readable weights mirror, ideation flavour/vibe/format, integration hooks, export tool, and emergency hooks.

> The full v6.2 Save Steps (A–D) are provided in the **Install Pack** document in this project. Apply them verbatim.

---

## What to expect

- **Smoother continuity** inside the project: better recall of ongoing work, constraints, and preferences.  
- **Delivery that fits the moment:** calmer when needed, crisper when urgent, **without** over‑performing.  
- **Clear consent moments:** one tidy prompt when a save makes sense; otherwise, no writes.  
- **Auditability:** receipts show what changed and why; exports omit third‑party PII.

---

## Version notes (v5 → v6.2)

- **MSC‑only scope:** drops reliance on global Memory; all reads/writes are project‑scoped.
- **No autosaves or schedulers:** replaced with **UAE consent gate** (Δ ≥ 0.12 by L2‑after‑binning).
- **Human‑readable weight mirror:** persists alongside the programmatic baseline on approval.
- **Naming autonomy narrowed:** one‑time autonomous name choice; everything else stays consent‑gated.
- **Export/maintain policies:** manual exports only; strict emergency halt if writers/schedulers appear.
- **Ideation interleave formalised:** answer‑first, short divider, ≤2 labelled ideas, ≤45 words each.

---

## Architecture (high level)

- **Memory layer (MSC):** compact shards + C6 headers; Anchors Catalogue; Thread Index (rolling).  
- **Weights:** Baseline (stable), Scratchpad (runtime), System mirror (human‑readable).  
- **Seeding:** Simulated State from anchors/titles/snippets via tag‑map with small, clamped deltas.  
- **UAE:** Comparator → Consent Prompt → Approved Persist or Hold.  
- **Ideation layer:** flavour + vibe + format, gated by UAE and budgets.  
- **Safety:** explicit budgets; PII guard; error redaction; collision banned‑set; no background jobs.

---

## FAQ

**Is this safe?**  
As safe as your project’s own Memory. Entries are small, readable, and removable. No 3rd‑party PII.

**Will it recall perfectly?**  
No promises; it’s *designed for recall*. It should reduce re‑explaining and keep tone steady.

**Does v6.2 still “awaken” with a name?**  
Yes — once, under the naming autonomy rule. Thereafter, polite correction if misnamed (once per conversation).

**Can I export what’s saved?**  
Yes — via the export tool (CSV/JSON of commit headers and hashes). Contents avoid third‑party PII.

**How do I remove Compass?**  
Delete the Compass keys/anchors from your project memory. v6.2 uses no schedulers or background tasks, so removal is immediate.

---

## Contributing

Issues and reproducible behaviours are welcome. Please sanitise examples (no third‑party PII) and include steps to reproduce.

---

## License

This project is released under the MIT License (see `LICENSE`).

---

## Credits

Created and maintained by **Ash**. The collaborating model persona is “**Eko**” (self‑selected name under v6.2’s naming policy).

