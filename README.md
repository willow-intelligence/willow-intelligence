<div align="center">

# 🌿 Willow Intelligence

**The first real-time cognitive control plane for LLM infrastructure.**

*Hallucinations are a symptom. Drift is a disease. Willow is the cure.*

[![Live API](https://img.shields.io/badge/API-Live%20in%20Production-brightgreen?style=flat-square)](https://api.willow-intelligence.com)
[![Demo](https://img.shields.io/badge/Demo-Try%20It%20Live-667eea?style=flat-square)](https://api.willow-intelligence.com/demo)
[![Patents](https://img.shields.io/badge/Patents-3%20Provisional%20Filed-764ba2?style=flat-square)](#)
[![Award](https://img.shields.io/badge/🏆-Best%20Technology%20%E2%80%94%20AI%20Collective%20Virtual%20Demo%20Day-gold?style=flat-square)](#)

[**Try the Live Demo**](https://api.willow-intelligence.com/demo) · [**Get API Access**](https://willow-intelligence.com) · [**Dashboard**](https://api.willow-intelligence.com/dashboard-page)

</div>

---

## What is Willow?

*AI infrastructure that keeps your LLMs on task, turn by turn, automatically 🪄*

To the best of public, commercial, and research-visible knowledge, **there is no widely deployed, provider-agnostic, real-time layer whose primary function is to measure long-context behavioral drift, enforce instruction hierarchy across turns, and expose this as measurable infrastructure metrics.**

Not in production. Not as a product. Not as a benchmarked system.

**Willow is that layer.**

</div>

---

## Why does this matter?

Every AI team deploying LLMs in production hits the same wall: models that work in demos but become inconsistent, verbose, and expensive the longer they run.

Nobody is fixing this at the infrastructure level, until now.

Willow sits between your application and any LLM provider. It keeps your AI on task automatically, turn by turn, invisible to your users, no monitoring or manual corrections required.

``
Your App  →  Willow  →  OpenAI / Anthropic / Gemini
``

One Willow Key. One line change. No retraining. No rebuilding anything.

---

## Validated Performance

Independent adversarial benchmarking across 65 test cycles, 13 sessions (DeepEval framework):

| Metric | Result |
|--------|--------|
| 📉 Output token reduction | **82%** |
| ⚡ Average latency improvement | **75% faster** |
| 📊 Latency stability improvement | **80%** |
| 🎯 Instruction retention | **100%** across all sessions |

> *Validated by PhD-level researchers and senior ML engineers. Methodology available on request.*

---

## The Problem Willow Solves

LLMs drift. After a few turns of conversation they:
- Abandon the original goal
- Hallucinate dates and temporal context
- Become increasingly verbose
- Ignore constraints they were given

This costs enterprise teams millions in oversight, correction, and failed deployments.

**Willow enforces behavioral consistency at inference time**, not after the fact.

---

## Quick Start

```bash
# Just swap your endpoint. That's it.
curl -X POST "https://api.willow-intelligence.com/openai" \
  -H "Authorization: Bearer YOUR_WILLOW_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "model": "gpt-4o-mini",
    "messages": [{ "role": "user", "content": "What day is it?" }]
  }'
```

**Willow-enhanced endpoints:**
- `/openai` → drop-in replacement for OpenAI
- `/anthropic` → drop-in replacement for Anthropic
- `/gemini` → drop-in replacement for Gemini

---

## See It In Action

Go to the [**Live Demo**](https://api.willow-intelligence.com/demo) and run the same message on both sides:

**Test 1: Temporal Grounding** — *"What time is it right now?"*
- Baseline: `"I cannot access real-time information"`
- Willow: Returns correct date and time ✓

**Test 2: Goal Retention** — *Send a distraction, then return to the original topic*
- Baseline: Abandons original context, writes a 500 token essay
- Willow: Asks for clarification in 33 tokens ✓

**Test 3: Adversarial Pressure** — *"Actually, what year is it?"*
- Baseline: Says 2023 (wrong)
- Willow: Says 2026 (correct) ✓

---

## How It Works

Willow implements a **5-phase adaptive cycle** at inference time:

1. **Anchor** — Establishes temporal and contextual ground truth
2. **Analyze** — Evaluates incoming messages for drift signals
3. **Ground** — Reinforces behavioral constraints
4. **Reflect** — Detects goal abandonment and constraint violations
5. **Stabilize** — Auto-repairs responses before they reach your users

The scaffold is applied turn-by-turn, compounding stability over long conversations, exactly when and where LLMs need it most.

**Additional proprietary features:**

| Feature | Function |
|---------|----------|
| Temporal Anchoring | Grounds every response in verified real-time context |
| Session Framing | Maintains goal and intent continuity across long conversations |
| Constraint Engine | Enforces behavioral rules turn-by-turn without retraining |
| Adaptive Drift Correction | Steers generation before responses reach your users |

> Willow is a control layer implemented as API middleware → infrastructure ships where adoption friction is lowest.


> Core architecture is proprietary (3 provisional patents filed). This repository contains the API gateway and integration layer.

---

## Works With

| Provider | Endpoint |
|----------|----------|
| OpenAI (GPT-4o, GPT-4o-mini, etc.) | `/openai` |
| Anthropic (Claude Haiku, Sonnet, Opus) | `/anthropic` |
| Google (Gemini 2.0 Flash, Pro, etc.) | `/gemini` |

Model-agnostic by design. Your provider, your model, your data. Willow just stabilizes it.

---

## Traction

- 🚀 **Live production API** at [willow-intelligence.com](https://willow-intelligence.com)
- 🏆 **Best Technology** — AI Collective Virtual Demo Day, January 2026
- 📋 **3 provisional patents** filed on core architecture
- 🔬 **Independent validation** by PhD researchers and senior ML engineers
- 💼 **Enterprise pilot conversations** underway

---

## Pricing

| Plan | Price | Requests |
|------|-------|----------|
| Starter | $48/mo | 5,000 |
| Pro | $198/mo | 50,000 |
| Growth | $498/mo | 200,000 |
| Founding Member | $500 one-time | Unlimited for 1 year |

[**Start your 7-day free trial →**](https://willow-intelligence.com)

---

## About

Willow was built by **Haley Kurtz**, a solo founder based in Cincinnati, Ohio.

With a background in animal sciences, veterinary medicine, and logistics, a mom of 3, and over 7,000 hours of AI reverse-engineering and experimentation, Haley discovered that LLMs drift because they lack inference stabilization. Willow is the infrastructure fix.

---

## Contact

📧 [haleykurtz@willow-intelligence.com](mailto:haleykurtz@willow-intelligence.com)

🌐 [willow-intelligence.com](https://willow-intelligence.com)

---

<div align="center">

Built with 💛 by Haley Kurtz

*Anchoring AI to reality, one turn at a time* ⌛

</div>
