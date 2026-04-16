<div align="center">

```
███╗   ██╗██╗████████╗███████╗██████╗ ██╗   ██╗██████╗ ██████╗ ██╗   ██╗
████╗  ██║██║╚══██╔══╝██╔════╝██╔══██╗██║   ██║██╔══██╗██╔══██╗╚██╗ ██╔╝
██╔██╗ ██║██║   ██║   █████╗  ██████╔╝██║   ██║██║  ██║██║  ██║ ╚████╔╝ 
██║╚██╗██║██║   ██║   ██╔══╝  ██╔══██╗██║   ██║██║  ██║██║  ██║  ╚██╔╝  
██║ ╚████║██║   ██║   ███████╗██████╔╝╚██████╔╝██████╔╝██████╔╝   ██║   
╚═╝  ╚═══╝╚═╝   ╚═╝   ╚══════╝╚═════╝  ╚═════╝ ╚═════╝ ╚═════╝    ╚═╝   
```

**Redesigning social interaction in nightlife.**

*Go out. Not alone.*

[![Status](https://img.shields.io/badge/status-in%20development-blueviolet?style=flat-square)](/)
[![Platform](https://img.shields.io/badge/platform-iOS%20%2F%20Android-black?style=flat-square)](/)
[![Market](https://img.shields.io/badge/market-Korea%20%F0%9F%87%B0%F0%9F%87%B7-red?style=flat-square)](/)
[![License](https://img.shields.io/badge/license-private-lightgrey?style=flat-square)](/)

</div>

---

## What is NITEBUDDY?

NITEBUDDY is a social matching platform that structurally eliminates the emotional friction and safety risks involved in finding a nightlife companion — built on an **anonymous, group-first architecture**.

> "We don't match people. **We connect situations and groups.**"

---

## Problem

Young adults in their 20s–30s repeatedly want to go to clubs and bars — but keep stopping themselves.

| Who | What they experience |
|-----|----------------------|
| Men | Rejection feels personal → emotional damage |
| Women | Safety threats, DM fatigue, unwanted exposure |
| Both | Want to keep their nightlife separate from their social identity — being seen at clubs or bars can damage how they're perceived by friends, colleagues, or acquaintances |

**Core insight:** People don't stop because they have "no one to go with." They stop because there's **no structure that makes it feel safe and normal to try.**

---

## Solution — 5 Immutable UX Principles

### 1. Anonymous to users. Known to the system.
- Between users: no real names, no phone numbers
- System side: account continuity + behavior tracking + repeat violations trigger restrictions
- → **Accountability without exposure**

### 2. No 1:1 matching
- Group-only outings (even 2 people are framed as a "group of 2")
- → Removes emotional stakes, blocks romantic/sexual framing

### 3. Waiting and rejection are system states
- No read receipts. No response timers. No rejection messages.
- Language used: *"Group conditions not yet met."*
- → Emotion is directed at the system, not the person

### 4. Connections end automatically
- Group chat auto-closes after the outing. No personal DMs. Re-contact only via system.
- → Eliminates persistent relationships = increased safety

### 5. Doing nothing should be safe by default
- Women: zero exposure without opting in; silence is always valid
- Men: no signal that they've been ignored

---

## Safety Architecture

```
How other apps fail              NITEBUDDY's approach
────────────────────             ──────────────────────────────
Full anonymity              →    Pseudonymity + system accountability
Report-only after the fact  →    Preventive design + post-incident enforcement
Direct person-to-person     →    Group-mediated, limited interaction
Persistent relationships    →    Time-limited + auto-terminated
```

Safety is built on three pillars: **Predictability + Control + Accountability**

---

## Competitive Differentiation

| Dimension | Existing Apps / Open Chats | NITEBUDDY |
|-----------|---------------------------|-----------|
| Core unit | Individual profile | **Group** |
| Response pressure | Immediate replies expected | Waiting normalized |
| Communication | DM-based | System-mediated |
| Rejection meaning | Personal failure | Conditions not met |
| Safety model | Reactive (post-incident) | **Proactive (structural)** |

---

## Revenue Model

> **Venues pay. Users don't.**

**Primary (B2B)**
- Club / bar partner registration fee
- Premium venue visibility
- Time-slot group creation rights

**Secondary (later stage)**
- Brand partnerships / event sponsorships / non-intrusive ads

---

## B2B Data Pipeline

What partner venues get — powered by group-level location intelligence:

```
Location sampling (user-consented)
            ↓
Staypoint Detection
(radius 80–120m, 12–15 min dwell, speed < 2.0 m/s)
            ↓
Venue Attribution Model (Softmax scoring)
            ↓
Group-level confidence aggregation (HCVS)
            ↓
Partner KPI Report
```

**What clubs receive:** Predictable visit demand + hourly heatmaps + neighborhood benchmarking data

---

## MVP Scope

- [x] Account creation (anonymous-based)
- [x] Group creation & joining
- [x] Waiting → Approval / Conditions-not-met UX
- [x] Report function (system review, no auto-ban)
- [x] Basic location-based filtering
- [ ] B2B partner dashboard *(v2)*
- [ ] High-frequency location tracking session *(v2)*

---

## Expansion Vision

```
Phase 1   Seoul nightlife pilot (Hongdae / Gangnam / Itaewon)
    ↓
Phase 2   Domestic city expansion
    ↓
Phase 3   Cities → Cultural regions → Events / Festivals / Travel
```

Growth strategy: No individual virality → **Venue-led onboarding**  
*"This is just how it works here."*

---

## Tech Stack

| Layer | Stack |
|-------|-------|
| Mobile | iOS / Android *(platform TBD)* |
| Backend | TBD |
| Database | Supabase |
| Location | GPS Staypoint Detection (rule-based) |
| Auth | Anonymous accounts + system-level tracking |

---

## Legal & Compliance

- Location data collection subject to Korean Personal Information Protection Act & Location Information Act review
- App Store review risk (nightlife-adjacent app policies) to be assessed
- All data collection requires explicit user consent

---

## Project Structure

```
NITEBUDDY/
├── brief.md              ← Project definition document
├── /docs                 ← Design docs, PRD, Research
├── /src                  ← Source code
├── /design               ← UI/UX design assets
└── /infra                ← Infrastructure configuration
```

---

<div align="center">

**NITEBUDDY** — Built by [Sean You](/)

*Standardizing social interaction in nightlife culture.*

</div>
