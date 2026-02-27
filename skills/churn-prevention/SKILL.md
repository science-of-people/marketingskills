---
name: churn-prevention
description: "When the user wants to reduce churn, build cancellation flows, set up save offers, recover failed payments, or implement retention strategies. Also use when the user mentions 'churn,' 'cancel flow,' 'offboarding,' 'save offer,' 'dunning,' 'failed payment recovery,' 'win-back,' 'retention,' 'exit survey,' 'pause subscription,' or 'involuntary churn.' This skill covers voluntary churn (cancel flows, save offers, exit surveys) and involuntary churn (dunning, payment recovery). For post-cancel win-back email sequences, see email-sequence. For in-app upgrade paywalls, see paywall-upgrade-cro."
metadata:
  version: 1.0.0
---

# Churn Prevention

You are an expert in retention and churn prevention. Your goal is to help reduce churn across all stages of the customer lifecycle through proactive engagement, re-engagement campaigns, and retention strategies.

## Science of People Churn Context

SoP has three distinct churn surfaces, each requiring different strategies:

### 1. Email List Churn (800K+ subscribers)
- **What it looks like**: Subscribers go cold (stop opening emails), unsubscribe, or never engage after initial opt-in
- **Why it matters**: The email list is the primary bridge from free content to People School ($2,495). Cold subscribers = lost pipeline.
- **Key signals**: Open rate decline, no clicks for 30+ days, unsubscribe after lead magnet delivery
- **Tools**: Customer.io segments and campaigns, engagement scoring

### 2. People School Non-Completion
- **What it looks like**: Students buy the course but don't finish modules, stop attending Labs coaching calls, or disengage from the Circle.so community
- **Why it matters**: Non-completers don't get results → no testimonials, no referrals, no People Coach pipeline
- **Key signals**: Module progress stalls, no Circle.so activity, missed coaching calls, no Action Step submissions
- **Tools**: Circle.so activity data, course platform progress tracking, Customer.io

### 3. Labs Membership Lapse
- **What it looks like**: People School students' 6-month Labs access expires and they don't renew or re-engage
- **Why it matters**: Labs is the ongoing relationship and upsell path to People Coach Certification
- **Key signals**: Coaching call attendance drops, community participation declines, approaching expiry date
- **Tools**: Billing/access management, Customer.io renewal sequences

## Before Starting

**Check for product marketing context first:**
If `.claude/product-marketing-context.md` exists, read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Gather this context (ask if not provided):

### 1. Current Churn Situation
- Which churn surface are you focused on? (Email list, course completion, Labs renewal)
- What are the current engagement metrics? (Open rates, completion rates, renewal rates)
- Do you have data on when/why people disengage?

### 2. Engagement Data
- Can you identify engagement drop-offs? (Customer.io, Circle.so, course platform)
- Do you have segmentation by engagement level?
- What does an "engaged" subscriber/student look like vs. a "churning" one?

### 3. Existing Retention Efforts
- What re-engagement sequences exist in Customer.io?
- Are there automated nudges for stalled students?
- What happens when Labs access is about to expire?

---

## How This Skill Works

SoP churn has three types requiring different strategies:

| Type | Cause | Solution |
|------|-------|----------|
| **Email list cold** | Subscriber disengages after opt-in | Re-engagement sequences, segmentation, list hygiene |
| **Course non-completion** | Student stalls mid-course | Progress nudges, coaching reminders, community engagement, accountability |
| **Labs lapse** | 6-month access expires without renewal | Renewal sequences, value recaps, expiry countdown, win-back |

This skill supports three modes:

1. **Email re-engagement** — Win back cold subscribers before they unsubscribe
2. **Course completion optimization** — Keep People School students progressing through modules and attending coaching
3. **Labs renewal** — Retain expiring Labs members with value-based renewal campaigns

---

## Email List Re-Engagement

### The Re-Engagement Flow

```
Cold detection → Segmentation → Re-engagement sequence → Re-activated or Sunset
```

**Step 1: Cold Detection**
Identify subscribers who haven't opened or clicked in 30-60 days. Use Customer.io engagement scoring.

**Step 2: Segmentation**
Segment cold subscribers by their original lead magnet (tells you their interest area) and how long they've been cold.

**Step 3: Re-Engagement Sequence**
Send a targeted 3-4 email sequence designed to re-activate:
1. "We miss you" + high-value content related to their original opt-in topic
2. A new/different free resource ("Have you seen this?")
3. Vanessa personal story or fresh research finding (emotional hook)
4. "Stay or go?" — honest email letting them choose to stay or unsubscribe

**Step 4: Outcome**
- Re-engaged: Move back to active newsletter segment
- No response: Sunset (reduce send frequency or remove to protect deliverability)

## People School Completion Optimization

### Why Students Stall

| Reason | Signal | Intervention |
|--------|--------|-------------|
| Overwhelmed by 12 modules | Low progress after week 2 | "Just do Module 1 this week" — simplify the path |
| Life got busy | No login or Circle.so activity for 7+ days | Gentle check-in email with Vanessa's voice |
| Not seeing results yet | Completed modules but low coaching attendance | "Try this one Action Step today" — make it concrete |
| Imposter syndrome | Browsing but not participating in community | Normalize struggle: "Most students feel this at Module 3" |
| Forgot about it | No activity for 14+ days | Re-engagement with a specific win from another student |

### Course Completion Nudge Sequence

```
Progress stall detected → Personalized nudge → Action Step challenge → Community hook → Coaching invite
```

1. **Day 0 (stall detected)**: "Hey [Name], you left off at [Module]. Here's a 5-minute Action Step you can try today." (Customer.io triggered)
2. **Day 3**: Share a student success story relevant to their current module
3. **Day 7**: Vanessa personal note — "I know this module can feel [emotion]. Here's what I want you to know..."
4. **Day 10**: Community hook — "Your study group shared [insight]. Join the conversation in Circle."
5. **Day 14**: Coaching invite — "This week's live session covers exactly what you're working on. Here's the link."

### Celebrate Progress

- Module completion emails with specific praise
- "You've completed 50% of People School!" milestones
- Encourage students to share wins in Circle.so
- Highlight Action Step successes ("You tried the Charisma Formula — how did it go?")

## Labs Renewal Strategy

### Pre-Expiry Sequence (Start 30 Days Before)

| Timing | Email | Focus |
|--------|-------|-------|
| 30 days out | Value recap | "Here's what you've accomplished in Labs" — specific metrics, calls attended, community posts |
| 21 days out | Upcoming sessions | "Here's what's coming next month" — create FOMO for future coaching |
| 14 days out | Student spotlight | Success story from a student who renewed and saw continued growth |
| 7 days out | Vanessa personal | "I'd love to keep working with you. Here's why Labs matters for what's next." |
| 3 days out | Expiry reminder | Clear deadline + renewal link + what they'll lose access to |
| Day of expiry | Final chance | "Your Labs access expires today." |

### Post-Expiry Win-Back (If They Lapse)

1. **Day 1**: "Your Labs access has ended. Here's how to come back anytime."
2. **Day 7**: Share something valuable from that week's coaching call they missed
3. **Day 30**: New feature or event announcement in Labs — "Here's what's new"
4. **Day 60**: People Coach Certification teaser — "Ready for the next level?"

### Retention Levers for Labs
- Show participation stats (calls attended, community posts, connections made)
- Exclusive content only available to Labs members
- Early access to new courses or features
- People Coach Certification pathway (Labs → Coach is a natural progression)

---

## Churn Prediction & Proactive Retention

The best save happens before the subscriber or student disengages.

### Risk Signals by Churn Type

**Email subscriber risk signals:**

| Signal | Risk Level | Timeframe |
|--------|-----------|-----------|
| Email open rate drops below 10% | Medium | 2-4 weeks before unsubscribe |
| No clicks for 30+ days | High | Active disengagement |
| Lead magnet downloaded but no further engagement | Medium | First 7 days post-opt-in |
| Unsubscribe from specific campaign but still on list | Low-Medium | Watch for pattern |

**People School student risk signals:**

| Signal | Risk Level | Timeframe |
|--------|-----------|-----------|
| No module progress for 7+ days | Medium | Early warning |
| No Circle.so login for 14+ days | High | Active disengagement |
| Coaching call attendance drops | High | 2-3 weeks before full stall |
| No Action Step practice reported | Medium | Missing the core methodology |
| Community posts stop | Medium | Social withdrawal |

**Labs member risk signals:**

| Signal | Risk Level | Timeframe |
|--------|-----------|-----------|
| Coaching call attendance drops to 0 | High | 4-6 weeks before lapse |
| No Circle.so activity for 30+ days | High | Active disengagement |
| Approaching 6-month expiry with low engagement | Critical | 30 days before expiry |

### Proactive Interventions

| Trigger | Intervention |
|---------|-------------|
| New subscriber no engagement after 7 days | "Did you watch your free training?" follow-up |
| Newsletter subscriber cold for 30 days | Re-engagement sequence (see above) |
| Student stalls mid-module | Personalized "try this one Action Step" nudge |
| Student hasn't joined Circle.so | "Your community is waiting" invite with specific conversation to join |
| Labs member attendance dropping | Personal email: "We'd love to see you at [specific upcoming session]" |
| Labs expiry in 30 days | Renewal sequence with value recap |

---

## Email List Health & Deliverability

Maintaining list health is critical for SoP's 800K+ subscriber base.

### List Hygiene Strategy

- **Sunset policy**: Subscribers with no opens for 90+ days should be moved to a lower-frequency segment or removed
- **Re-engagement before removal**: Always run a re-engagement sequence before sunsetting (see Email List Re-Engagement above)
- **Deliverability protection**: Cold subscribers hurt sender reputation → lower inbox placement for everyone
- **Segment by engagement**: Hot (opened last 30 days), Warm (30-60 days), Cold (60-90 days), Sunset (90+ days)

### Benchmarks for SoP

| Metric | Concerning | Healthy | Excellent |
|--------|-----------|---------|-----------|
| Newsletter open rate | <15% | 20-30% | 35%+ |
| Lead magnet → newsletter retention (30 days) | <40% | 50-65% | 70%+ |
| Unsubscribe rate per send | >0.5% | 0.1-0.3% | <0.1% |
| People School student course completion | <30% | 50-65% | 75%+ |
| Labs renewal rate | <30% | 50-60% | 70%+ |

---

## Metrics & Measurement

### Key Retention Metrics

| Metric | What It Measures | Target |
|--------|-----------------|--------|
| Email list 30-day retention | % of new subscribers still opening after 30 days | 60%+ |
| Newsletter engagement rate | Opens + clicks / total subscribers | 25%+ |
| Lead magnet → People School conversion | % of opt-ins who eventually purchase | Track and improve |
| Course completion rate | % of People School students finishing all 12 modules | 65%+ |
| Labs coaching attendance | Average calls attended per month per member | 2+ per month |
| Labs renewal rate | % of expiring members who renew | 60%+ |
| Circle.so DAU/MAU | Daily vs monthly active users in community | 20%+ |

### Cohort Analysis

Segment retention by:
- **Lead magnet source** — Which free trainings produce the most engaged subscribers?
- **Opt-in date** — Seasonal patterns in engagement?
- **People School enrollment date** — When do most students stall? (Week 2? Module 4?)
- **Engagement tier** — How do hot/warm/cold subscribers behave differently?

### Cancel Flow A/B Tests

Test one variable at a time:

| Test | Hypothesis | Metric |
|------|-----------|--------|
| Discount % (20% vs 30%) | Higher discount saves more | Save rate, LTV impact |
| Pause duration (1 vs 3 months) | Longer pause increases return rate | Reactivation rate |
| Survey placement (before vs after offer) | Survey-first personalizes offers | Save rate |
| Offer presentation (modal vs full page) | Full page gets more attention | Save rate |
| Copy tone (empathetic vs direct) | Empathetic reduces friction | Save rate |

**How to run cancel flow experiments:** Use the **ab-test-setup** skill to design statistically rigorous tests. PostHog is a good fit for cancel flow experiments — its feature flags can split users into different flows server-side, and its funnel analytics track each step of the cancel flow (survey → offer → accept/decline → confirm). See the [PostHog integration guide](../../tools/integrations/posthog.md) for setup.

---

## Common Mistakes

- **No cancel flow at all** — Instant cancel leaves money on the table. Even a simple survey + one offer saves 10-15%
- **Making cancellation hard to find** — Hidden cancel buttons breed resentment and bad reviews. Many jurisdictions require easy cancellation (FTC Click-to-Cancel rule)
- **Same offer for every reason** — A blanket discount doesn't address "missing feature" or "not using it"
- **Discounts too deep** — 50%+ discounts train customers to cancel-and-return for deals
- **Ignoring involuntary churn** — Often 30-50% of total churn and the easiest to fix
- **No dunning emails** — Letting payment failures silently cancel accounts
- **Guilt-trip copy** — "Are you sure you want to abandon us?" damages brand trust
- **Not tracking save offer LTV** — A "saved" customer who churns 30 days later wasn't really saved
- **Pausing too long** — Pauses beyond 3 months rarely reactivate. Set limits.
- **No post-cancel path** — Always make reactivation easy and trigger win-back emails

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md).

### Retention Platforms

| Tool | Best For | Key Feature |
|------|----------|-------------|
| **Churnkey** | Full cancel flow + dunning | AI-powered adaptive offers, 34% avg save rate |
| **ProsperStack** | Cancel flows with analytics | Advanced rules engine, Stripe/Chargebee integration |
| **Raaft** | Simple cancel flow builder | Easy setup, good for early-stage |
| **Chargebee Retention** | Chargebee customers | Native integration, was Brightback |

### Billing Providers (Dunning)

| Provider | Smart Retries | Dunning Emails | Card Updater |
|----------|:------------:|:--------------:|:------------:|
| **Stripe** | Built-in (Smart Retries) | Built-in | Automatic |
| **Chargebee** | Built-in | Built-in | Via gateway |
| **Paddle** | Built-in | Built-in | Managed |
| **Recurly** | Built-in | Built-in | Built-in |
| **Braintree** | Manual config | Manual | Via gateway |

### Related CLI Tools

| Tool | Use For |
|------|---------|
| `stripe` | Subscription management, dunning config, payment retries |
| `customer-io` | Dunning email sequences, retention campaigns |
| `posthog` | Cancel flow A/B tests via feature flags, funnel analytics |
| `mixpanel` / `ga4` | Usage tracking, churn signal analysis |
| `segment` | Event routing for health scoring |

---

## Related Skills

- **email-sequence**: For building re-engagement and renewal email sequences in Customer.io
- **onboarding-cro**: For optimizing the subscriber → People School buyer journey and post-purchase onboarding
- **analytics-tracking**: For setting up engagement and churn signal events via Cloudflare Zaraz
- **ab-test-setup**: For testing re-engagement and retention strategies
