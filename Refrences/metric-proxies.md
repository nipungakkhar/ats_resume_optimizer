# Metric Proxies & Estimation Benchmarks

Use this file during Phase 4 (Metric Excavation) to suggest plausible ranges when
a candidate says "I don't know the exact number." Present the range, let the candidate
confirm or correct it, and mark confirmed estimates with "approximately" or "~".

Never fabricate — always get candidate confirmation before using any estimate.

---

## How to Use This File

1. Identify the candidate's role and industry
2. Find the relevant benchmark section below
3. Suggest the range to the candidate:
   > "Based on typical [role] teams, a [X] person support team usually handles
   > roughly [Y–Z] tickets/week. Does that sound right for your team?"
4. Candidate confirms → use with "approximately" prefix
5. Candidate corrects → use their number directly

---

## By Role Type

### Software Engineering
| What to estimate | Typical range | Excavation question |
|---|---|---|
| App/service users | 1K–5M depending on company size | "How many users did the product serve at its peak?" |
| Bugs/issues resolved | 5–30/sprint for mid-level | "How many tickets did you typically close per sprint?" |
| Uptime / reliability | 99.5–99.99% for production | "Was there an SLA? What was the uptime target?" |
| Deploy frequency | Daily → quarterly | "How often were releases pushed to production?" |
| Code review throughput | 5–20 PRs/week | "Roughly how many pull requests did you review weekly?" |
| CI/CD time reduction | 30–80% improvement | "How long did builds take before vs. after your pipeline work?" |
| Team size | 3–15 for most squads | "How many engineers were on your immediate team?" |
| Sprint velocity | 20–80 story points | "Did your team track story points or velocity?" |

### Data Science / Analytics
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Data volume | GBs to PBs depending on scale | "How much data were you processing daily/weekly?" |
| Model accuracy improvement | 5–30% lift | "What was the baseline accuracy vs. your model's?" |
| Dashboards built | 3–20 per analyst/year | "How many dashboards or reports did you own?" |
| Stakeholders served | 5–200 depending on role | "How many teams or people relied on your reports?" |
| Prediction/classification tasks | Varies widely | "Was there a business outcome tied to the model's predictions?" |
| Time saved via automation | 2–20 hrs/week | "What was being done manually before your solution?" |
| A/B tests run | 2–20/quarter | "How many experiments did you design or analyze?" |

### Marketing
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Email list size | 1K–500K for B2B, larger for B2C | "How large was your email list or subscriber base?" |
| Email open rate | 20–35% B2B, 15–25% B2C | "Do you know your average open or click-through rate?" |
| Monthly web traffic | 5K–5M depending on company | "Did you have access to Google Analytics? Rough monthly visits?" |
| Social media followers | 500–500K+ | "What was the follower count when you managed those accounts?" |
| Campaign budget | $5K–$500K/quarter | "What was your typical campaign budget?" |
| Lead generation | 50–5,000 MQLs/month | "How many leads or MQLs were you generating per month?" |
| Conversion rate | 1–5% for most B2B funnels | "Do you know the conversion rate from lead to opportunity?" |
| Ad spend managed | $5K–$2M/month | "What was your total paid media budget?" |

### Sales / Business Development
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Annual quota | $500K–$5M for mid-market AE | "What was your annual quota?" |
| Quota attainment | % of quota hit | "Did you hit, exceed, or fall short of quota? By roughly how much?" |
| Pipeline generated | 3–5× quota in pipeline | "How much pipeline did you generate per quarter?" |
| Deal size (ACV) | $10K–$500K for B2B SaaS | "What was your average deal size?" |
| Accounts managed | 20–200 for account management | "How many accounts were in your book of business?" |
| Win rate | 15–35% for most B2B | "What was your rough win rate or close rate?" |
| Sales cycle | 30–180 days B2B | "How long was your average sales cycle?" |

### Customer Success / Support
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Accounts managed | 30–200 depending on tier | "How many customer accounts were you responsible for?" |
| ARR managed | $500K–$10M for CSM | "What was the total ARR in your book of business?" |
| NPS / CSAT score | NPS 30–70, CSAT 85–95% | "Did your team track NPS or CSAT? What was your score?" |
| Churn rate reduced | 1–10% reduction | "Did you have a target churn rate? How did yours compare?" |
| Tickets handled | 20–100/week for support | "Roughly how many tickets or cases did you handle per week?" |
| First response time | 1–24 hours | "What was your first response time SLA?" |
| Renewal rate | 85–98% for healthy SaaS | "What was your renewal or retention rate?" |

### Operations / Project Management
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Budget managed | $50K–$50M+ | "What was the total budget you were responsible for?" |
| Team size | 3–50 for most PM roles | "How many people were on the team or project?" |
| Projects run simultaneously | 2–15 | "How many projects were you managing at once?" |
| Process time reduced | 20–70% | "How long did the process take before vs. after?" |
| On-time delivery rate | 80–98% | "What percentage of projects delivered on time?" |
| Cost savings | 10–40% reduction | "Did the new process reduce costs? Rough estimate?" |
| Vendors/contracts managed | 5–50 | "How many vendors or suppliers did you manage?" |

### Finance / Accounting
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Budget overseen | $500K–$500M+ | "What was the total budget you managed or reported on?" |
| Cost savings delivered | $50K–$10M | "Did any of your work result in measurable cost savings?" |
| Reports produced | Weekly, monthly, quarterly | "How frequently did you produce financial reports? For how many stakeholders?" |
| Forecast accuracy | 90–98% | "Did you have a forecast accuracy KPI? What did you achieve?" |
| Audit findings reduced | # of findings | "Did the number of audit findings change under your watch?" |
| Compliance rate | % | "Was there a compliance rate or control metric you owned?" |

### HR / People / Talent
| What to estimate | Typical range | Excavation question |
|---|---|---|
| Roles hired/year | 10–200 for mid-sized TA team | "How many positions did you fill in a year?" |
| Time-to-fill | 30–90 days | "What was your average time-to-fill for open roles?" |
| Employee headcount managed | 50–5,000 | "How large was the employee population you supported?" |
| Retention rate | 80–95% | "Did you track retention or turnover rates? What were they?" |
| Training programs | # of programs / # of participants | "How many employees went through training programs you designed?" |
| Offer acceptance rate | 70–95% | "What was your offer acceptance rate?" |
| eNPS or engagement score | 30–70 | "Did the company run engagement surveys? What was the score?" |

---

## Estimation Conversation Templates

Use these scripts verbatim or adapt them to the candidate's situation:

**Template 1 — Volume estimate:**
> "Let's figure this out together. How many people were on your team? And roughly
> how many clients/users/tickets did the team handle? That gives us a per-person
> number we can use."

**Template 2 — Before/after estimate:**
> "Think about the first week you started this project vs. six months in. What felt
> noticeably different? Faster? Fewer errors? Let's put a rough number on that."

**Template 3 — Revenue/cost estimate:**
> "You don't need the exact finance figure. Was it closer to $10K, $100K, or $1M
> in impact? Even a rough order of magnitude is useful and honest with an 'approximately.'"

**Template 4 — Relative performance:**
> "Were you hitting your targets? Exceeding them? By how much roughly — 10% above,
> 50% above? Top quartile of your team? That's a metric too."

**Template 5 — Team/scope proxy:**
> "Even if you can't quantify the outcome, we can quantify the scope. How many
> countries, offices, systems, or product lines were involved?"

---

## Proxy Scale Language (When No Number Exists)

If estimation genuinely fails, default to this hierarchy:

1. **Count** — "Managed 14 client accounts across 3 verticals"
2. **Frequency** — "Delivered weekly executive reports to 6 C-suite stakeholders"
3. **Comparative** — "Reduced process from 3-day manual cycle to same-day automation"
4. **Scope** — "Led 9-person cross-functional team spanning engineering, design, and product"
5. **Sequence** — "Designed and shipped 4 major product releases in 18 months"

Even one of these transforms a vague bullet into a concrete, credible statement.
