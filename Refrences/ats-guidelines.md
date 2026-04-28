# ATS Technical Guidelines & Common Pitfalls

A deep-dive reference for ensuring maximum ATS (Applicant Tracking System) compatibility.

---

## How ATS Systems Parse Resumes

Modern ATS platforms (Workday, Greenhouse, Lever, iCIMS, Taleo, BambooHR, SmartRecruiters)
parse resumes by:

1. **Converting** the document to plain text
2. **Tokenizing** text into words and phrases
3. **Matching** tokens against the job description's keyword model
4. **Scoring** the resume based on keyword frequency, placement, and section relevance
5. **Ranking** candidates against each other in the applicant pool

Key insight: ATS doesn't "read" — it pattern-matches. Every formatting decision should
be made through the lens of: "Will this survive plain-text conversion and still carry
its meaning?"

---

## Critical Formatting Rules

### Layout
- **Single column ONLY** — multi-column resumes often parse as jumbled text in ATS
- **No text boxes** — text inside text boxes is frequently invisible to parsers
- **No headers/footers** — contact info in headers is often skipped entirely
- **No tables for content** — use plain text with spacing instead
- **No graphics, logos, icons, or decorative elements** — these break parsers

### File Format
- **.docx is universally safe** — preferred over PDF for ATS submission
- **.pdf can be problematic** — use only if: (a) the JD explicitly requests PDF, or
  (b) the candidate is applying via email directly to a human (not an ATS portal)
- **Never submit**: .pages, .odt, .rtf (inconsistent parser support)

### Typography
**ATS-safe fonts:** Arial, Calibri, Cambria, Garamond, Georgia, Helvetica,
Times New Roman, Trebuchet MS, Verdana

**Unsafe fonts:** Decorative, script, or display fonts — they render as symbols
after text conversion.

**Font sizes:**
- Name: 16–18pt
- Section headers: 12–14pt
- Body text: 10–12pt (never below 10pt — some ATS reject tiny text)

**Avoid:**
- Underlines (can look like hyperlinks or confuse parsers)
- All-caps section headings are fine; all-caps body text is not
- Excessive bold — use only for names, company names, job titles

### Section Headings
Use only standard, widely recognized headings. ATS categorizes content by
recognized section labels:

✅ Standard (use these):
- Summary / Professional Summary / Career Summary
- Experience / Work Experience / Professional Experience
- Education / Academic Background
- Skills / Core Competencies / Technical Skills
- Certifications / Licenses
- Projects
- Publications
- Awards / Honors
- Volunteer Experience
- Languages

❌ Non-standard (avoid):
- "My Journey" (instead of Experience)
- "What I Bring" (instead of Summary)
- "Toolbox" (instead of Skills)
- "Learning" (instead of Education)
- Emoji in headings (🚀 Experience)

### Dates
**Consistent format is required.** Pick one and use it everywhere:
- ✅ Month YYYY: "January 2022 – March 2024"
- ✅ Abbreviated: "Jan 2022 – Mar 2024"
- ✅ MM/YYYY: "01/2022 – 03/2024"

**Avoid:**
- Year-only dates for jobs (only acceptable for education)
- Inconsistent mixing: "January 2022 – 3/2024"

For current roles: "January 2023 – Present"

### Special Characters
**Safe:** Hyphen (-), bullet (•), pipe (|), forward slash (/), ampersand (&),
parentheses (), em dash (—) used sparingly

**Unsafe:** Decorative bullets (→ ★ ✓ ◆), non-standard dashes, curly quotes
(use straight quotes only)

---

## Keyword Strategy

### Placement Priority Zones
ATS systems weight keywords differently based on location:

1. **Highest weight**: Job title, professional summary (top of document)
2. **High weight**: Skills/competencies section
3. **Standard weight**: Experience bullet points
4. **Lower weight**: Education, certifications (for non-academic roles)

Implication: Primary keywords must appear in the summary AND skills section.

### Keyword Density Formula
For a 1-page resume targeting a keyword-rich JD:
- Primary keywords (top 5–8 from JD): appear 2–3× each across the full document
- Secondary keywords: appear 1–2× each
- Never force a keyword — if it doesn't fit naturally, the skills section is the
  acceptable fallback location

### Acronym Strategy
Always include BOTH the acronym and the spelled-out version at least once:
- "Search Engine Optimization (SEO)" in the summary or skills
- Then "SEO" alone in experience bullets

This covers ATS that search for either form.

### Exact Match vs. Semantic Match
Older ATS (Taleo, older iCIMS): exact keyword matching — the word must match precisely
Modern ATS (Greenhouse, Lever, modern Workday): semantic matching — synonyms may score

**Safe approach:** Use the exact phrasing from the JD, especially for:
- Job title (mirror it in the summary)
- Required tools/technologies (exact product names)
- Required certifications (exact certification names)
- Specific methodologies (Agile, Scrum, Six Sigma — use exact form from JD)

---

## Common ATS Failure Points

| Issue | Why It Fails | Fix |
|-------|-------------|-----|
| Multi-column layout | Parsed left-to-right across columns, creating nonsense | Use single column |
| Contact info in header | Many parsers skip the header zone | Put contact info in main body |
| Text boxes | Content is invisible to parser | Remove all text boxes |
| Tables for skills | Skills merge into garbled text | Use comma/pipe separated list |
| Fancy bullet symbols | Convert to strange characters | Use • or - |
| PDF with columns | PDF parsing strips column structure | Use .docx or single-column PDF |
| Image of resume | Completely unreadable by ATS | Never submit an image |
| Non-standard section names | ATS can't categorize content | Use standard headings |
| Embedded hyperlinks as plain text | URL may not be captured | Spell out URLs |
| Inconsistent date formats | Parsing engine may fail on date extraction | Standardize all dates |

---

## ATS Scoring Benchmarks

| Score Range | Typical Outcome |
|-------------|-----------------|
| 90–100 | Strong shortlist candidate; likely to reach human review |
| 75–89 | Competitive; depends on applicant pool |
| 60–74 | At risk; may be filtered before human review |
| Below 60 | Likely auto-rejected in high-volume hiring |

Target: 90+ on primary keyword match. The goal of 100/100 means every required
keyword from the JD is represented accurately and naturally in the resume.

---

## ATS Platforms Quick Reference

| Platform | Common In | Notes |
|----------|-----------|-------|
| Taleo (Oracle) | Enterprise / Fortune 500 | Strict exact-match; loves .docx |
| Workday | Mid-large enterprise | Good PDF support; section headings matter |
| Greenhouse | Tech startups / scale-ups | Strong semantic matching |
| Lever | Tech startups | Similar to Greenhouse |
| iCIMS | Healthcare, retail, manufacturing | Moderate; prefers .docx |
| BambooHR | SMBs | Less strict; but still follow standards |
| SmartRecruiters | Diverse industries | Good modern parser |
| Jobvite | Media, tech | Good parser; watch for tables |

---

## Pre-Submission Checklist

Run through this before delivering the final resume:

**Content**
- [ ] Professional summary mirrors the JD job title
- [ ] All primary JD keywords present in summary and/or skills
- [ ] All required skills from JD appear somewhere in the resume
- [ ] No vague language ("responsible for", "helped with")
- [ ] At least 60% of bullets have quantifiable metrics
- [ ] Most recent role has the most detail (4–6 bullets)
- [ ] Older/irrelevant roles trimmed (2–3 bullets)
- [ ] No first-person pronouns
- [ ] Current role in present tense; past roles in past tense

**Formatting**
- [ ] Single column layout
- [ ] Contact info in the body (not header/footer)
- [ ] Standard section headings only
- [ ] No tables, text boxes, or graphics
- [ ] ATS-safe font
- [ ] Consistent date format throughout
- [ ] File saved as .docx (or .pdf only if required)
- [ ] Appropriate length for experience level
- [ ] Consistent spacing and alignment
