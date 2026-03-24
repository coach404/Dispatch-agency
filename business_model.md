# Business Model: AI-Powered Truck Dispatching Agency

---

## 1. Executive Summary

**Company Concept:** An AI-first freight dispatching agency that fully replaces human dispatchers with autonomous AI agents capable of handling every step of the dispatching workflow — from finding loads to negotiating rates, coordinating pickups, managing paperwork, and resolving issues in real time.

**Core Technology Stack:**
- **Chat AI Agents** (powered by Claude API) for load negotiation, email/text communication with brokers and shippers
- **Voice AI Agents** (powered by Vapi.ai or Bland.ai) for inbound/outbound phone calls with brokers, shippers, and drivers
- **Voice Synthesis** (ElevenLabs) for natural, human-like voice on all calls
- **Multilingual Support:** English, Spanish, Russian, and other languages to serve diverse driver and carrier populations

**Key Differentiators:**
- 24/7 availability — no nights, weekends, or holidays
- Sub-second response times on load boards and broker calls
- No human dispatcher salaries, benefits, or turnover costs
- Scales from 1 truck to 1,000+ without hiring headcount
- Consistent quality and compliance across every interaction

**Target Customers:** Owner-operators, small fleets (2–20 trucks), and mid-size carriers (21–100 trucks) who currently pay traditional dispatch agencies 5–10% of gross revenue.

**Business Stage:** Pre-revenue / MVP development (Month 1), targeting first paying clients by Month 2.

---

## 2. Revenue Models

Three pricing models are evaluated below. The recommended approach is to **launch with Model A (per-truck monthly fee)** for simplicity and predictability, then introduce Model B (percentage) as an upsell for high-volume carriers.

### 2.1 Comparison Table

| Criteria | **Model A: Per-Truck Monthly Fee** | **Model B: Percentage of Load Value** | **Model C: Flat Monthly Retainer per Carrier** |
|---|---|---|---|
| **Pricing** | $150–$300 / truck / month | 5–10% of gross load revenue | $500–$2,500 / carrier / month |
| **Revenue Predictability** | High — fixed MRR | Low — fluctuates with freight market | High — fixed MRR |
| **Customer Appeal** | High — easy to budget | Mixed — aligns cost with earnings, but cuts into margins | Mixed — good for large fleets, poor for small |
| **Scalability for Us** | Linear with truck count | Scales with freight rates | Scales with carrier count only |
| **Avg. Revenue per Truck** | $150–$300/mo (predictable) | ~$200–$600/mo (depends on loads) | $25–$125/mo per truck (diluted for large fleets) |
| **Sales Complexity** | Low | Medium — requires load tracking integration | Low |
| **Risk of Churn** | Low — clients on monthly contracts | High — clients leave when freight market softens | Low |
| **Best For** | Owner-operators and small fleets | Mid-size fleets running consistent high-value lanes | Large carriers wanting cost control |

### 2.2 Model Details

**Model A — Per-Truck Monthly Fee (Recommended for Launch)**
- Tier 1: $250/truck/month (1–5 trucks)
- Tier 2: $200/truck/month (6–20 trucks)
- Tier 3: $150/truck/month (21+ trucks)
- Includes: 24/7 dispatching, load finding, rate negotiation, broker calls, check calls, document management

**Model B — Percentage of Load Value**
- 7% of gross load revenue, billed monthly based on reported settlements
- Minimum monthly fee of $150/truck to cover base costs
- Requires integration with factoring companies or ELD data for revenue verification

**Model C — Flat Monthly Retainer per Carrier**
- Solo operator: $500/month (up to 3 trucks)
- Small fleet: $1,200/month (4–10 trucks)
- Mid fleet: $2,500/month (11–25 trucks)
- Enterprise: Custom pricing (26+ trucks)

---

## 3. Cost Structure

### 3.1 Monthly Operating Costs

| Cost Category | Component | Est. Monthly Cost (Early Stage, ~50 trucks) | Est. Monthly Cost (Growth Stage, ~200 trucks) | Notes |
|---|---|---|---|---|
| **AI / LLM** | Claude API (Anthropic) | $300–$600 | $1,200–$2,500 | ~$6–$12/truck/mo; varies by call/message volume |
| **Voice AI Platform** | Vapi.ai or Bland.ai | $400–$800 | $1,500–$3,000 | ~$8–$15/truck/mo; per-minute pricing |
| **Voice Synthesis** | ElevenLabs | $100–$200 | $400–$800 | Character-based pricing; grows with call volume |
| **Telephony** | Twilio (phone numbers + SMS) | $150–$300 | $500–$1,000 | $1/number/mo + per-call/SMS rates |
| **Infrastructure** | Cloud hosting (AWS/GCP), databases | $200–$400 | $600–$1,200 | Scales with concurrent agent sessions |
| **Load Board Access** | DAT, Truckstop.io subscriptions | $200–$500 | $500–$1,000 | Required for automated load searching |
| **Development** | Ongoing dev / maintenance (contractor) | $3,000–$5,000 | $5,000–$8,000 | Bug fixes, feature dev, integrations |
| **Sales & Marketing** | Ads, outreach tools, CRM | $500–$1,000 | $2,000–$4,000 | Facebook, trucking Facebook groups, Google |
| **Legal & Compliance** | MC authority, contracts, insurance | $300–$500 | $300–$500 | Relatively fixed overhead |
| **Customer Support** | Human escalation agent (part-time) | $500–$1,000 | $1,500–$2,500 | Handle edge cases AI can't resolve |
| **Misc / Buffer** | Tools, subscriptions, contingency | $200–$300 | $500–$800 | |
| **TOTAL** | | **$5,850–$10,600** | **$14,000–$25,300** | |

### 3.2 One-Time Startup Costs

| Item | Estimated Cost |
|---|---|
| MVP Development (AI agent pipeline, voice integration) | $15,000–$30,000 |
| Legal setup (LLC, contracts, terms of service) | $1,500–$3,000 |
| Brand & website | $1,000–$2,500 |
| Initial marketing / launch campaign | $2,000–$5,000 |
| **Total One-Time** | **$19,500–$40,500** |

---

## 4. Break-Even Analysis

Break-even is calculated as: **Break-even trucks = Total Monthly Fixed Costs / Net Revenue per Truck**

### 4.1 Assumptions

- Base monthly fixed costs (excluding variable AI costs): **$5,000/month**
- Variable AI/voice cost per truck: **$30/month**
- Net revenue per truck = Pricing − Variable cost per truck

### 4.2 Break-Even by Model

| Revenue Model | Price per Truck | Variable Cost per Truck | Net Contribution Margin | Fixed Monthly Costs | Break-Even Trucks |
|---|---|---|---|---|---|
| **Model A (Tier 1 — $250/truck)** | $250 | $30 | $220 | $5,000 | **23 trucks** |
| **Model A (Tier 2 — $200/truck)** | $200 | $30 | $170 | $5,000 | **30 trucks** |
| **Model A (Tier 3 — $150/truck)** | $150 | $30 | $120 | $5,000 | **42 trucks** |
| **Model B (7% — avg $350/mo per truck)** | $350 (est.) | $30 | $320 | $5,000 | **16 trucks** |
| **Model C (Retainer — ~$150/truck equiv.)** | $150 | $30 | $120 | $5,000 | **42 trucks** |

**Key Insight:** With Model A at Tier 1 pricing ($250/truck), break-even requires just **23 trucks** — approximately 5–10 small carriers. This is achievable within the first 2–3 months with targeted outreach.

---

## 5. Six-Month Financial Projection

The following projection uses **Model A (per-truck monthly fee)** as the primary revenue driver, with a blended average rate of **$220/truck/month** (mix of Tier 1 and Tier 2 clients).

### 5.1 Projection Table

| | **Month 1** | **Month 2** | **Month 3** | **Month 4** | **Month 5** | **Month 6** |
|---|---|---|---|---|---|---|
| **Carrier Clients** | 0 | 3 | 7 | 12 | 18 | 25 |
| **Trucks Managed** | 0 | 10 | 25 | 50 | 80 | 120 |
| **Gross Revenue** | $0 | $2,200 | $5,500 | $11,000 | $17,600 | $26,400 |
| **Variable AI/Voice Costs** | $500 | $800 | $1,250 | $2,000 | $2,900 | $4,100 |
| **Fixed Operating Costs** | $5,500 | $5,500 | $6,000 | $6,500 | $7,000 | $7,500 |
| **Total Costs** | $6,000 | $6,300 | $7,250 | $8,500 | $9,900 | $11,600 |
| **Net Profit / (Loss)** | **($6,000)** | **($4,100)** | **($1,750)** | **$2,500** | **$7,700** | **$14,800** |
| **Cumulative P&L** | ($6,000) | ($10,100) | ($11,850) | ($9,350) | ($1,650) | **$13,150** |

### 5.2 Key Milestones

| Milestone | Target Month |
|---|---|
| MVP live, first pilot client (free or discounted) | Month 1 |
| First 3 paying carriers onboarded | Month 2 |
| Operational break-even (monthly) | Month 4 |
| Cumulative break-even (recover all startup costs) | Month 7–8 |
| 25 carrier clients / 120 trucks | Month 6 |

---

## 6. Competitive Advantage

### 6.1 vs. Traditional Human Dispatch Agencies

| Factor | Traditional Agency | Our AI Agency |
|---|---|---|
| **Availability** | Business hours (8–5), on-call nights extra | 24/7/365, no overtime |
| **Response Time** | Minutes to hours | Seconds |
| **Cost to Carrier** | 5–10% of gross revenue | 1–3% equivalent (fixed fee model) |
| **Languages Supported** | 1–2 (usually English only) | English, Spanish, Russian, and more |
| **Scalability** | Linear headcount growth | Instant scaling, no hiring |
| **Consistency** | Varies by dispatcher quality | 100% consistent protocols |
| **Turnover Risk** | High — dispatchers quit, take clients | None |
| **Negotiation Speed** | Limited by human availability | Simultaneous multi-broker negotiation |
| **Data & Analytics** | Minimal reporting | Full dashboards, load history, analytics |

### 6.2 vs. AI Dispatch Tools (Doft, Kopilot, etc.)

| Factor | Doft / Kopilot | Our AI Agency |
|---|---|---|
| **Business Model** | SaaS tool — carrier operates it themselves | Full-service agency — we do everything |
| **Driver Burden** | Carrier must learn and use the software | Zero learning curve — we handle it all |
| **Voice AI Calls** | Limited or none | Full inbound/outbound voice agent |
| **Broker Negotiation** | Semi-automated, needs human oversight | Fully autonomous negotiation agents |
| **Multilingual** | Limited | Native multilingual support |
| **Support Model** | Ticket-based SaaS support | Dedicated account management |
| **Target Customer** | Tech-savvy carriers | All carriers including non-tech-savvy |
| **Price** | $99–$299/truck/mo (software only) | $150–$250/truck/mo (full service) |

**Summary:** We occupy a unique position — the operational efficiency of AI with the full-service model of a traditional dispatch agency. Carriers get better service at lower cost without having to learn new software.

---

## 7. Risk Register

| # | Risk | Probability | Impact | Mitigation Strategy |
|---|---|---|---|---|
| **1** | **AI makes dispatching errors** (wrong rates, missed appointments, compliance failures) | Medium | High | Implement confidence thresholds — AI escalates to human review for edge cases. Maintain human oversight queue. Start with co-pilot mode before full autonomy. Log all decisions for audit. |
| **2** | **API cost overrun** (Claude, Vapi, ElevenLabs pricing changes or usage spikes) | Medium | Medium | Set hard usage caps and alerts per truck. Monitor cost/truck weekly. Negotiate volume discounts at scale. Build fallback to lower-cost models for simple tasks. |
| **3** | **Regulatory and legal liability** (freight claims, broker disputes, MC compliance) | Low–Medium | High | Carry freight broker liability insurance. Have clear contracts with carriers defining scope and liability limits. Consult transportation attorney before launch. Never hold carrier funds. |
| **4** | **Low customer trust / adoption resistance** (carriers skeptical of AI dispatching) | High | Medium | Offer free 2-week pilot with no commitment. Lead with outcomes (more loads, higher rates, no missed calls) not technology. Provide human backup visible to clients. Collect testimonials early. |
| **5** | **Competitor response** (Doft, Kopilot, or large agencies copy the model) | Medium | Medium | Move fast to build carrier relationships and lock-in through integrations (ELD, factoring). Focus on underserved segments (Spanish/Russian-speaking carriers). Build proprietary rate negotiation data moat over time. |

---

*Document Version: 1.0 — March 2026*
*All financial projections are estimates based on current market conditions and are subject to change.*
