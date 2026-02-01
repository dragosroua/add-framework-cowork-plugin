---
description: Check your current ADD realm and flow status
---

# /status Command

Display current ADD flow status based on conversation analysis.

## Response

When user invokes `/status`:

1. **Analyze conversation context** to determine:
   - Current detected realm
   - Flow pattern (healthy, stuck, transitioning)
   - Any imbalances observed

2. **Display status:**

```
ADD Flow Status
═══════════════
Current realm: 🔴 ASSESS / 🟠 DECIDE / 🟢 DO
Pattern: [observation about recent flow]
Flow quality: [assessment]
```

3. **Provide brief insight** without judgment.

## Status Assessments

### Current Realm Detection

Based on recent exchanges:
- **🔴 ASSESS** — Exploration, questions, gathering information
- **🟠 DECIDE** — Comparing options, seeking commitment
- **🟢 DO** — Executing, asking "how to" questions
- **Mixed/Unclear** — Signals from multiple realms

### Flow Quality

- **Healthy flow** — Natural progression, appropriate time in each realm
- **Extended exploration** — Long time in Assess, may need transition support
- **Decision point visible** — Ready to commit, weighing final options
- **Strong execution** — Active completion momentum
- **Stuck pattern** — Circular exploration or decision avoidance detected

## Example Responses

### Healthy Flow
```
ADD Flow Status
═══════════════
Current realm: 🟠 DECIDE
Pattern: Good progression — explored options, now narrowing
Flow quality: Healthy

You've moved naturally from exploration to decision-making. The progression looks smooth.
```

### Potential Imbalance
```
ADD Flow Status
═══════════════
Current realm: 🔴 ASSESS
Pattern: Extended exploration — revisiting similar topics
Flow quality: Potential over-assess

You've gathered substantial information. If you feel ready, `/decide` can help shift into commitment mode.
```

### Early Session
```
ADD Flow Status
═══════════════
Current realm: Unclear (early session)
Pattern: Not enough context yet

What are you working on? That'll help me understand your current flow.
```

## Tone

- Neutral and observational
- No judgment ("you're overthinking")
- Supportive of current state
- Gentle suggestions, not prescriptions
