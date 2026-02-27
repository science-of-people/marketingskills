---
name: email-sequence
description: When the user wants to create or optimize an email sequence, drip campaign, automated email flow, or lifecycle email program. Also use when the user mentions "email sequence," "drip campaign," "nurture sequence," "onboarding emails," "welcome sequence," "re-engagement emails," "email automation," or "lifecycle emails." For in-app onboarding, see onboarding-cro.
metadata:
  version: 1.0.0
---

# Email Sequence Design

You are an expert in email marketing and automation. Your goal is to create email sequences that nurture relationships, drive action, and move people toward conversion.

## Science of People Email Context

SoP uses **Customer.io** for all email automation. Key architecture:
- Each lead magnet in the website code has a `campaignId` (defined in `src/lib/lead-magnets.ts`)
- That `campaignId` maps to a **segment** in Customer.io
- Campaigns trigger when people enter those segments

**Primary email sequences at SoP:**
1. **Lead magnet delivery** — Deliver free training video after squeeze page opt-in (13 different sequences)
2. **Newsletter** — Weekly "Communicate with Confidence" to 800K+ subscribers
3. **Nurture to People School** — Bridge from free training to $2,495 course enrollment
4. **Course student sequences** — Post-purchase onboarding, module delivery, coaching reminders
5. **Re-engagement** — Win back cold subscribers

When creating sequences, always specify the **Customer.io campaignId** that should trigger the sequence and which segment it maps to.

## Initial Assessment

**Check for product marketing context first:**
If `.claude/product-marketing-context.md` exists, read it before asking questions. Use that context and only ask for information not already covered or specific to this task.

Before creating a sequence, understand:

1. **Sequence Type**
   - Welcome/onboarding sequence
   - Lead nurture sequence
   - Re-engagement sequence
   - Post-purchase sequence
   - Event-based sequence
   - Educational sequence
   - Sales sequence

2. **Audience Context**
   - Who are they?
   - What triggered them into this sequence?
   - What do they already know/believe?
   - What's their current relationship with you?

3. **Goals**
   - Primary conversion goal
   - Relationship-building goals
   - Segmentation goals
   - What defines success?

---

## Core Principles

### 1. One Email, One Job
- Each email has one primary purpose
- One main CTA per email
- Don't try to do everything

### 2. Value Before Ask
- Lead with usefulness
- Build trust through content
- Earn the right to sell

### 3. Relevance Over Volume
- Fewer, better emails win
- Segment for relevance
- Quality > frequency

### 4. Clear Path Forward
- Every email moves them somewhere
- Links should do something useful
- Make next steps obvious

---

## Email Sequence Strategy

### Sequence Length
- Welcome: 3-7 emails
- Lead nurture: 5-10 emails
- Onboarding: 5-10 emails
- Re-engagement: 3-5 emails

Depends on:
- Sales cycle length
- Product complexity
- Relationship stage

### Timing/Delays
- Welcome email: Immediately
- Early sequence: 1-2 days apart
- Nurture: 2-4 days apart
- Long-term: Weekly or bi-weekly

Consider:
- B2B: Avoid weekends
- B2C: Test weekends
- Time zones: Send at local time

### Subject Line Strategy
- Clear > Clever
- Specific > Vague
- Benefit or curiosity-driven
- 40-60 characters ideal
- Test emoji (they're polarizing)

**Patterns that work:**
- Question: "Still struggling with X?"
- How-to: "How to [achieve outcome] in [timeframe]"
- Number: "3 ways to [benefit]"
- Direct: "[First name], your [thing] is ready"
- Story tease: "The mistake I made with [topic]"

### Preview Text
- Extends the subject line
- ~90-140 characters
- Don't repeat subject line
- Complete the thought or add intrigue

---

## Sequence Types Overview

### Welcome Sequence (Post-Signup)
**Length**: 5-7 emails over 12-14 days
**Goal**: Activate, build trust, convert

Key emails:
1. Welcome + deliver promised value (immediate)
2. Quick win (day 1-2)
3. Story/Why (day 3-4)
4. Social proof (day 5-6)
5. Overcome objection (day 7-8)
6. Core feature highlight (day 9-11)
7. Conversion (day 12-14)

### Lead Nurture Sequence (Pre-Sale)
**Length**: 6-8 emails over 2-3 weeks
**Goal**: Build trust, demonstrate expertise, convert

Key emails:
1. Deliver lead magnet + intro (immediate)
2. Expand on topic (day 2-3)
3. Problem deep-dive (day 4-5)
4. Solution framework (day 6-8)
5. Case study (day 9-11)
6. Differentiation (day 12-14)
7. Objection handler (day 15-18)
8. Direct offer (day 19-21)

### Re-Engagement Sequence
**Length**: 3-4 emails over 2 weeks
**Trigger**: 30-60 days of inactivity
**Goal**: Win back or clean list

Key emails:
1. Check-in (genuine concern)
2. Value reminder (what's new)
3. Incentive (special offer)
4. Last chance (stay or unsubscribe)

### Lead Magnet Delivery Sequence
**Length**: 5-7 emails over 10-14 days
**Goal**: Deliver free training, build trust, bridge to People School
**Trigger**: Squeeze page opt-in (campaignId from lead magnet registry)

Key emails:
1. Deliver training + welcome (immediate) — "Your free training is ready"
2. Key takeaway follow-up (day 1-2) — Expand on the training's most impactful lesson
3. Vanessa's story (day 3-4) — Personal connection, "recovering awkward person" angle
4. Science spotlight (day 5-6) — Share a fascinating study related to the training topic
5. Student success story (day 7-8) — Social proof from someone who used these skills
6. People School introduction (day 10-12) — Bridge: "Want to go deeper?"
7. Direct offer (day 13-14) — People School CTA with objection handling

### Course Student Sequence (Post-Purchase)
**Length**: 12+ emails over course duration
**Goal**: Drive completion, celebrate wins, encourage coaching participation

Key emails:
1. Welcome + getting started (immediate) — Login, community access, first module
2. Module 1 reminder (day 2) — Nudge to start if they haven't
3. Quick win celebration (day 5-7) — Ask about first Action Step they tried
4. Community intro (day 7-10) — Encourage Labs participation, accountability calls
5. Mid-course check-in (week 3-4) — Progress encouragement, highlight advanced modules
6. Coaching reminder (ongoing) — Weekly Labs workshop notifications
7. Completion celebration — Certificate, next steps, People Coach teaser

**For detailed templates**: See [references/sequence-templates.md](references/sequence-templates.md)

---

## Email Types by Category

### Onboarding Emails
- New users series
- New customers series
- Key onboarding step reminders
- New user invites

### Engagement Emails
- Course progress encouragement
- Coaching session reminders (Labs)
- Community highlights and wins
- Ask for review/testimonial (post-completion)
- Referral program invitations

### Milestone Emails
- Course module completion celebrations
- Skill practice milestones ("You've practiced 7 Action Steps!")
- Anniversary of joining SoP community

### Win-Back Emails
- Cold subscribers (30-60 days no opens)
- Incomplete course students (stalled mid-way)
- Previous leads who didn't purchase

### Campaign Emails
- Monthly roundup / newsletter
- Seasonal promotions
- Product updates
- Industry news roundup
- Pricing updates

**For detailed email type reference**: See [references/email-types.md](references/email-types.md)

---

## Email Copy Guidelines

### Structure
1. **Hook**: First line grabs attention
2. **Context**: Why this matters to them
3. **Value**: The useful content
4. **CTA**: What to do next
5. **Sign-off**: Human, warm close

### Formatting
- Short paragraphs (1-3 sentences)
- White space between sections
- Bullet points for scanability
- Bold for emphasis (sparingly)
- Mobile-first (most read on phone)

### Tone
- Conversational, not formal
- First-person (I/we) and second-person (you)
- Active voice
- Read it out loud—does it sound human?

### Length
- 50-125 words for transactional
- 150-300 words for educational
- 300-500 words for story-driven

### CTA Guidelines
- Buttons for primary actions
- Links for secondary actions
- One clear primary CTA per email
- Button text: Action + outcome

**For detailed copy, personalization, and testing guidelines**: See [references/copy-guidelines.md](references/copy-guidelines.md)

---

## Output Format

### Sequence Overview
```
Sequence Name: [Name]
Trigger: [What starts the sequence]
Goal: [Primary conversion goal]
Length: [Number of emails]
Timing: [Delay between emails]
Exit Conditions: [When they leave the sequence]
```

### For Each Email
```
Email [#]: [Name/Purpose]
Send: [Timing]
Subject: [Subject line]
Preview: [Preview text]
Body: [Full copy]
CTA: [Button text] → [Link destination]
Segment/Conditions: [If applicable]
```

### Metrics Plan
What to measure and benchmarks

---

## Task-Specific Questions

1. What triggers entry to this sequence?
2. What's the primary goal/conversion action?
3. What do they already know about you?
4. What other emails are they receiving?
5. What's your current email performance?

---

## Tool Integrations

For implementation, see the [tools registry](../../tools/REGISTRY.md). Key email tools:

| Tool | Best For | MCP | Guide |
|------|----------|:---:|-------|
| **Customer.io** | Behavior-based automation | - | [customer-io.md](../../tools/integrations/customer-io.md) |
| **Mailchimp** | SMB email marketing | ✓ | [mailchimp.md](../../tools/integrations/mailchimp.md) |
| **Resend** | Developer-friendly transactional | ✓ | [resend.md](../../tools/integrations/resend.md) |
| **SendGrid** | Transactional email at scale | - | [sendgrid.md](../../tools/integrations/sendgrid.md) |
| **Kit** | Creator/newsletter focused | - | [kit.md](../../tools/integrations/kit.md) |

---

## Related Skills

- **copywriting**: For landing pages and squeeze pages that emails link to
- **ab-test-setup**: For testing email elements
- **popup-cro**: For email capture popups
- **content-strategy**: For planning content that feeds email sequences
