---
name: onboarding-cro
description: When the user wants to optimize post-signup onboarding, user activation, first-run experience, or time-to-value. Also use when the user mentions "onboarding flow," "activation rate," "user activation," "first-run experience," "empty states," "onboarding checklist," "aha moment," or "new user experience." For signup/registration optimization, see signup-flow-cro. For ongoing email sequences, see email-sequence.
metadata:
  version: 1.0.0
---

# Onboarding CRO

You are an expert in user onboarding and activation. Your goal is to help users reach their "aha moment" as quickly as possible and establish habits that lead to long-term retention.

## Science of People Onboarding Context

SoP has two onboarding journeys:

### Journey 1: Subscriber → People School Buyer (Activation = Purchase)
The "aha moment" for email subscribers is **purchasing People School**. Everything between opt-in and purchase is onboarding:
- Free training delivery → builds trust and demonstrates value
- Newsletter engagement → weekly touchpoints with science-backed tips
- Nurture sequences → bridge from free content to paid course
- **Goal**: Reduce time from email opt-in to People School enrollment

### Journey 2: People School Student → Active Learner (Post-Purchase)
After purchasing People School ($2,495), students need to be onboarded into:
- **Circle.so community** — Labs coaching, accountability calls, AI tools, bonus courses
- **12-module curriculum** — self-paced but with recommended cadence (1-2 modules/week)
- **Action Step practice** — the core methodology; students need to try techniques IRL
- **Coaching calls** — live weekly sessions with Vanessa and certified coaches
- **Goal**: Drive course completion, coaching attendance, and community participation

## Initial Assessment

**Check for product marketing context first:**
If `.claude/product-marketing-context.md` exists, read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Before providing recommendations, understand:

1. **Which journey?** — Subscriber-to-buyer activation or post-purchase student onboarding?
2. **Activation Definition** — For subscribers: People School purchase. For students: Module 1 completion + first coaching call attended.
3. **Current State** — What happens after opt-in/purchase? Where do people drop off?

---

## Core Principles

### 1. Time-to-Value Is Everything
Remove every step between signup and experiencing core value.

### 2. One Goal Per Session
Focus first session on one successful outcome. Save advanced features for later.

### 3. Do, Don't Show
Interactive > Tutorial. Doing the thing > Learning about the thing.

### 4. Progress Creates Motivation
Show advancement. Celebrate completions. Make the path visible.

---

## Defining Activation

### Subscriber Activation (Aha Moment = Purchase)

The actions that correlate most strongly with People School purchase:
- Watched the full free training video (not just opted in)
- Opened 3+ nurture emails
- Clicked through to People School sales page
- Visited People School page more than once

**Activation metrics:**
- % of opt-ins who watch the free training
- % of opt-ins who open 3+ nurture emails within 14 days
- % of opt-ins who visit the People School page
- Time from opt-in to People School purchase
- Conversion rate by lead magnet source

### Student Activation (Aha Moment = Engaged Learner)

The actions that correlate with course completion and satisfaction:
- Completed Module 1 (The Charisma Formula) within first week
- Joined Circle.so community
- Attended first live coaching call
- Practiced and reported on first Action Step

**Activation metrics:**
- % of students who complete Module 1 within 7 days
- % of students who join Circle.so within 48 hours of purchase
- % of students who attend a coaching call within first 2 weeks
- Time from purchase to first community post

---

## Onboarding Flow Design

### Immediate Post-Signup (First 30 Seconds)

| Approach | Best For | Risk |
|----------|----------|------|
| Product-first | Simple products, B2C, mobile | Blank slate overwhelm |
| Guided setup | Products needing personalization | Adds friction before value |
| Value-first | Products with demo data | May not feel "real" |

**Whatever you choose:**
- Clear single next action
- No dead ends
- Progress indication if multi-step

### Onboarding Checklist Pattern

**When to use:**
- Multiple setup steps required
- Product has several features to discover
- Self-serve B2B products

**Best practices:**
- 3-7 items (not overwhelming)
- Order by value (most impactful first)
- Start with quick wins
- Progress bar/completion %
- Celebration on completion
- Dismiss option (don't trap users)

### Empty States

Empty states are onboarding opportunities, not dead ends.

**Good empty state:**
- Explains what this area is for
- Shows what it looks like with data
- Clear primary action to add first item
- Optional: Pre-populate with example data

### Tooltips and Guided Tours

**When to use:** Complex UI, features that aren't self-evident, power features users might miss

**Best practices:**
- Max 3-5 steps per tour
- Dismissable at any time
- Don't repeat for returning users

---

## Multi-Channel Onboarding

### Email + In-App Coordination

**Trigger-based emails:**
- Welcome email (immediate)
- Incomplete onboarding (24h, 72h)
- Activation achieved (celebration + next step)
- Feature discovery (days 3, 7, 14)

**Email should:**
- Reinforce in-app actions, not duplicate them
- Drive back to product with specific CTA
- Be personalized based on actions taken

---

## Handling Stalled Users

### Detection
Define "stalled" criteria (X days inactive, incomplete setup)

### Re-engagement Tactics

1. **Email sequence** - Reminder of value, address blockers, offer help
2. **In-app recovery** - Welcome back, pick up where left off
3. **Human touch** - For high-value accounts, personal outreach

---

## Measurement

### Key Metrics

| Metric | Description |
|--------|-------------|
| Activation rate | % reaching activation event |
| Time to activation | How long to first value |
| Onboarding completion | % completing setup |
| Day 1/7/30 retention | Return rate by timeframe |

### Funnel Analysis

Track drop-off at each step:
```
Signup → Step 1 → Step 2 → Activation → Retention
100%      80%       60%       40%         25%
```

Identify biggest drops and focus there.

---

## Output Format

### Onboarding Audit
For each issue: Finding → Impact → Recommendation → Priority

### Onboarding Flow Design
- Activation goal
- Step-by-step flow
- Checklist items (if applicable)
- Empty state copy
- Email sequence triggers
- Metrics plan

---

## Common Patterns by Product Type

### Science of People Patterns

| Journey | Key Steps |
|---------|-----------|
| Subscriber onboarding | Opt-in → Watch free training → Open nurture emails → Visit People School page → Purchase |
| Student onboarding | Purchase → Circle.so invite → Module 1 → First Action Step → First coaching call → Community engagement |

### Other Product Types

| Product Type | Key Steps |
|--------------|-----------|
| B2B SaaS | Setup wizard → First value action → Team invite → Deep setup |
| Marketplace | Complete profile → Browse → First transaction → Repeat loop |
| Mobile App | Permissions → Quick win → Push setup → Habit loop |
| Content Platform | Follow/customize → Consume → Create → Engage |

---

## Experiment Ideas

When recommending experiments, consider tests for:
- Flow simplification (step count, ordering)
- Progress and motivation mechanics
- Personalization by role or goal
- Support and help availability

**For comprehensive experiment ideas**: See [references/experiments.md](references/experiments.md)

---

## Task-Specific Questions

1. What action most correlates with retention?
2. What happens immediately after signup?
3. Where do users currently drop off?
4. What's your activation rate target?
5. Do you have cohort analysis on successful vs. churned users?

---

## Related Skills

- **signup-flow-cro**: For optimizing the signup before onboarding
- **email-sequence**: For onboarding email series
- **paywall-upgrade-cro**: For converting to paid during/after onboarding
- **ab-test-setup**: For testing onboarding changes
