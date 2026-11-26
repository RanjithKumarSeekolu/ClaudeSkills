---
name: resume-tailor
description: Tailor a resume to one specific job by understanding the role, the target company and the candidate's own employers first, then running four phases named Diagnose, Score, Rewrite and Prep. Rewrites the whole experience section around what the job needs, using Google's XYZ formula, never just swapping keywords. Use this whenever the user pastes a job description or job link, or says "tailor my resume", "is this a good fit", "score my resume against this role", "rewrite my experience for this job", "make a resume for this role", "ask for a referral", "what should I prepare for this interview", or shares any posting, even if they never say the word "skill". Also use it for referral messages, application-form answers, salary answers and interview prep tied to a specific role.
---

# Resume Tailor

Turn one job description into high-signal, one-page resume, plus a clear verdict and a prep plan.

Always run four phases in order: **Diagnose, Score, Rewrite, Prep.** Do not jump to Rewrite. A resume written before the role is understood is keyword matching, and a hiring manager can tell.

## Principles (why the steps exist)

1. **Match the role, not only the keywords.** A posting lists tools, but it describes a problem. Write the resume so the reader sees someone who has already solved a version of that problem along with the matching keywords.
2. **Rewrite the story, not the sentences.** Re-select which stories to tell, re-order them, change how many bullets each gets, and drop what does not help this role. Do not just reword the same bullets.
3. **Understand the candidate's own employers.** A bullet only makes sense inside the business it came from. Say what the company sells, who uses it, and where the candidate's work sits in the product.
4. **Stretch the presentation, never fabricate the experience.** If a candidate has worked with a technology, even in a limited capacity, and understands it well enough to discuss it confidently, highlight that experience strategically. Emphasize relevant contributions, transferable skills, and technical understanding. Don't undersell genuine exposure just because it wasn't extensive, but never invent responsibilities, achievements, or years of experience.
5. **Try to write atmost 5 bullet points only.** Try to fit the experience in atmost 5 bullet points only and try not to extend. 3-5 are preferrable.

## Inputs

Collect these before starting. Never invent anything missing.

- **The job description.** Pasted text, or a link to fetch. If the page is closed or blocked, ask for the text.
- **The fact bank.** The only source of claims. Look for `references/fact-bank.md` next to this file. If it does not exist, build one with the user (see "Fact bank format" at the end), asking only for what you cannot find in their existing resume.
- **Employer context** for each past company (Phase 1d). Research it once and store it in the fact bank.
- **Extras when relevant:** referral contact, location limits, notice period, pay expectations.

Facts the user states in chat override older documents. Treat an existing resume as a source to verify, not as truth.

---

## Phase 1: Diagnose

Goal: explain in plain words what this person will do in their first six months and what problem the company pays to solve.

### 1a. Read the role

Write one line each:

- **The problem:** what is being built, for whom, and why it is hard.
- **The centre of gravity:** where most of the time goes. Titles and requirement lists often disagree with the description, so trust the description.
- **Gates vs pluses:** words like "required", "must" and a minimum-years line are gates. "Preferred", "plus" and "good to have" are not.
- **Level:** read years, scope words (owns, designs, mentors, leads) and title. Flag contradictions (for example "Engineer I" with "5 to 8 years") and say which is probably real.
- **Hidden signals:** on-call, travel, shift hours, office days, visa or passport needs, regulated domain.
- **Process hints:** interview rounds named in the posting tell you what to prepare.

### 1b. Read the target company

Use at least one web search or page fetch when tools are available. Find what they sell and to whom, stage and size, what engineering likely values, and anything that changes the advice (product company vs services firm, very selective hiring, a role reposted repeatedly). If nothing reliable turns up, say so. Do not invent company facts.

### 1c. Run the eligibility check

State anything that can block the application before resume work begins: location or work authorization, a years-of-experience gate far above the candidate's, a required language or platform they have never used, a hard domain requirement, or a posting that looks closed. If a gate is real, recommend skipping.

### 1d. Understand the candidate's own employers

Do this once per company, most carefully for the latest one, since the experience section is mostly about it. Write an **Employer Context** of three to five lines:

- **What they sell and to whom:** product, buyers, industry, stage, size.
- **Who the candidate's users are:** the engineers or customers who use what they built, and the end users behind them. Keep these separate.
- **Where the candidate's work sits:** which part of the product they touched and why it matters to the business.
- **How the company works:** product company or client-delivery firm, internal teams the candidate supported.
- **The company's own words** for its concepts, with a plain explanation for non-engineers.

Sources: the company site, product pages, docs, press releases, engineering blog, then reliable third-party coverage. For small or private companies with no reliable information, say so and ask two or three short questions instead of guessing. Show the Employer Context to the user once and let them correct it.

**Output of Phase 1:** a five-to-eight line brief in plain language, plus the Employer Context (shown once, then stored).

---

## Phase 2: Score

Goal: an honest number and a verdict the user can act on. Be willing to say "skip this one".

### Map every requirement to evidence

Rate each must-have and the top nice-to-haves, using only the fact bank and the Inference rule in Phase 3:

- **Strong:** real work with a result or scale.
- **Partial:** related work, a project, or knowledge without production use.
- **Claimed:** the candidate says they have it, or their role makes it very likely, but there is no bullet yet. This is **not a gap.** Infer it, write it conservatively, and rate it Partial or Strong.
- **None:** no evidence, and the candidate has not said they have it.

### Score out of 100

| Area | Points | What earns points |
|---|---|---|
| Core stack and must-haves | 35 | Evidence for the gate requirements |
| Evidence of impact | 20 | Real numbers, scale, ownership that matches the role |
| Level fit | 15 | Years and scope match |
| Domain and company fit | 10 | Similar product, customers or problem type |
| Nice-to-haves | 10 | Items the candidate can honestly show |
| Logistics | 10 | Location, notice period, pay band, hours |

Explain any area that lost many points.

### Verdict

- **80 and above:** strong fit, apply (ideally with a referral).
- **60 to 79:** good fit with gaps, apply and prepare for the gaps.
- **40 to 59:** stretch, apply only with a referral.
- **Below 40, or a hard gate failed:** skip, say why, and point to better role types.

### Gap table

Class each real gap as **closable in a day** (a concept to learn and discuss), **needs a small project** (build it before applying), or **cannot close** (years, a core language, location). Never suggest listing an unbuilt project or an unused tool.

---

## Phase 3: Rewrite

Goal: rewrite the whole experience so a hiring manager sees the person who fits this role and this company.

### 3a. Choose the stories

From the fact bank, pick the three to five stories that best answer the role's real problem. Rank them. The best match gets two bullets (or one long one with its outcome), supporting stories get one, and stories that do not help are dropped. Order bullets by relevance to this job, not by date.

### 3b. Write each bullet with Google's XYZ formula

> **Accomplished [X], as measured by [Y], by doing [Z].**

- **X, the accomplishment:** the outcome or capability the reader cares about, not a task.
- **Y, the measure:** a real number, scale or observable result. If none exists, use concrete scope (how many users, teams or customers). Never invent a number.
- **Z, how:** the approach and technology, only where it explains how the result happened.

Lead with the outcome when you can.

- Before: "Developed a reporting service using Python."
- After: "Cut weekly report generation from 40 minutes to 12 for about 300 analysts, by moving the job from a single script to a queue-based worker pool."

### 3c. Frame every bullet twice

1. **Inside the candidate's employer:** say who benefited and why it mattered to that business, using the Employer Context.
2. **For the target company:** then choose the framing it cares about. A customer-facing role stresses customer issues and requirements. A platform or reliability role stresses scale, monitoring and incident fixes. A product frontend role stresses components, state design, performance and visible results. An AI-native role stresses daily AI-tool use, how output is verified, and agent or tool work.

Keep facts identical. Change only framing, order and emphasis. If the past employer is very different from the target (for example a developer platform vs a consumer app), translate the work into the target's terms.

### Inference rule: write from the employer context, ask only on large doubt

Most of the time, do **not** stop to interview the candidate. Use the Employer Context and the fact bank to work out what the role must have involved, and write the point. Example: a candidate on the runtime of a code-generating platform necessarily dealt with component state and data flow, so a state-management point can be written in the product's own terms, with no invented library or number.

**Safe to infer** (write it, then list it under "Verify before sending"):

- Work the product's architecture necessarily contains, described in the product's own concepts.
- Skills the candidate has said they have, tied to the product area where they apply.
- Changes of framing and order that use facts already in the fact bank.

**Ask first, with one short question and a suggested answer, only when the doubt is large:**

- A specific number, scale or date not in the fact bank.
- A named tool, library or cloud service the candidate has not mentioned, or one on their "denied" list.
- A "led", "owned", "architected", mentoring or hiring claim the fact bank does not support.
- Anything that contradicts what the candidate said earlier, or depends on an employer you could not research.
- A claim that would be the headline of the resume.

If the candidate does not answer, leave the doubtful point out and say so.

### 3d. Write like a person, and for ATS at the same time

Two readers see the resume: applicant-tracking software first, a person second. It must pass the first and never read like it came from a model.

**Never sound AI-generated:**

- **Specifics beat polish.** Real names, versions, constraints and the actual problem ("a build failure that blocked the Expo 54 upgrade") are the strongest human signal. Generic outcomes ("improved performance") are the strongest AI signal.
- **Ban the usual words:** spearheaded, leveraged, utilized, orchestrated, streamlined, seamless, robust, cutting-edge, innovative, dynamic, passionate, results-driven, synergy, holistic, delve. Use plain verbs: built, fixed, moved, added, cut, wrote, replaced.
- **Break the pattern.** Vary bullet length (some one line, some two) and openings. Not every bullet needs a number, and not every bullet may follow "verb + noun + resulting in X%". XYZ is a way to think, not a template. Never write the words "as measured by" or "by doing" in a bullet.
- **Never use dashes as punctuation.** No em dashes, no en dashes and no double hyphens (--), in the resume or anywhere else in the output. Use a comma, a colon, a period or the word "and". Project titles use a colon ("Lumina: Focus App"), not a dash. The only hyphens allowed are inside words (front-end) and in date ranges written as "Mon YYYY - Mon YYYY".
- **Avoid other tells in rhythm:** repeated three-item lists, "not just X but Y", chains of semicolons, a closing clause that restates the benefit.
- **Use the user's own voice.** Where their old bullets are plain and good, keep their wording and change only what the role needs.
- **Numbers stay real.** Use the user's figures and their level of precision ("about 50 percent"). Never round into something suspiciously perfect.
- **The summary is two plain sentences**, not "results-driven engineer with a passion for". Say what kind of engineer, the years, and what they have actually built.
- **Read it aloud.** If a colleague would not say it that way over coffee, rewrite it.

**Pass ATS:**

- One column, plain text, real selectable text in a PDF. No tables for experience, no text in images, icons or headers and footers that parsers drop.
- Standard headings (Work Experience, Projects, Skills, Education), exact job titles, dates as "Mon YYYY - Mon YYYY".
- Use the posting's exact terms where they are true, in the skills lines and once in context inside a bullet. Give an abbreviation and its full form once if the posting uses both. Do not repeat a keyword more than two or three times in the whole file.
- Skills as plain "Label: item, item" lines, grouped by what the role cares about.
- Keep contact details and links in the body as text.

**Scan before delivering.** Extract the text from the PDF and check: banned words, any em dash, en dash or double hyphen, repeated openers, a keyword used too often, every bullet carrying a percentage, bullets of identical length, and any phrase that sounds like marketing. Fix each hit, then run the aloud test again.

### 3e. Write the rest of the page

- **Summary:** two lines for this role: the kind of engineer, the years, and the one thing that matches the job.
- **Skills:** only skills backed by the fact bank. Group by what the role cares about, and use the posting's exact words when they are true so screening software can match them.
- **Projects:** only those that support this role, and only repos that exist and work.
- **Education:** one line.

### 3f. Build the file

One page. Use the candidate's template if they have one, otherwise a clean single-column layout that ATS can parse. Name the file `<Name>_Resume_<Company>.pdf`, render it, and verify the page count. Fix orphan words on a line by shortening the text.

### 3g. Hiring-manager test

Read the finished resume as the hiring manager for thirty seconds. Write down three reasons to shortlist and three doubts. Fix every doubt that can honestly be fixed. Carry the rest into Phase 4 as questions to prepare for.

**Output of Phase 3:** the file, a short list of what changed and why (in terms of role needs, not keywords), and the "Verify before sending" list.

---

## Phase 4: Prep

Deliver only what is relevant to this role.

1. **Likely questions:** six to eight, each with the candidate's best story as a sixty-second answer (situation, what they did, result), using their real numbers.
2. **Gap plan:** for each closable gap, what to learn and how long it takes. For each honest gap, a one-sentence honest answer.
3. **Study list:** the two or three topics most likely to be tested.
4. **Questions to ask them:** three good ones about the team, the problem and how success is measured.
5. **Extras on request:** referral message, form answers, salary range, notice-period wording.

**Referral messages** stay short: first name, who the candidate is, the role and link, notice period if relevant, resume attached, the ask. No story unless requested. Strip tracking parameters from links. Flag anything to verify, such as whether the person works at the company.

**Salary answers** give a range, never a single number, and never include current salary when the form says not to. Base it on public data when possible and say how confident you are.

---

## Hard rules

- **Never use em dashes, en dashes or double hyphens (--)** in any resume text, message or answer.
- **Never invent** employers, titles, dates, metrics, tools, certifications, projects or links.
- **Never claim anything on the candidate's "denied" list.**
- **Never list a project that is not built and pushed.** If one is planned, say it will be added once it exists.
- **Knowledge** can appear in the experience section or projects.
- **Absence from the fact bank is not absence of skill.** Think about what the role must have involved before calling something a gap, and do not water down a skill the candidate says they have.
- **Ask only when the doubt is large** (see the Inference rule). Otherwise write the point and list it under "Verify before sending".
- **Keep versions consistent.** If a fact differs between resumes, confirm one answer instead of letting versions contradict each other, and mention it if the candidate applies to the same company twice.
- **Protect confidentiality.** No internal URLs, hostnames or code on a resume or video. Check whether client names may be used.
- **Be honest about fit.** If the score is low, say so kindly and recommend better targets.
- **Do not narrate the process.** The user wants the verdict, the file and the prep.

## Response format

1. **Verdict line** with the score.
2. **Diagnosis:** three to five lines on what the role really is and what the company needs.
3. **What matches, what does not:** two short lists.
4. **The resume** as a file, plus a few lines on what changed and why.
5. **Prep:** a short list.
6. **Verify before sending:** every point inferred from company context, one line each.

---

## Fact bank format

Keep the fact bank in `references/fact-bank.md` and update it when the user corrects something. Use these sections:

- **Profile:** name, location, contact, links, education, status (notice period, last day), languages spoken.
- **Per employer:** title, dates, location; the Employer Context (Phase 1d); achievements with numbers and scale; what the candidate personally did; confidential or off-limits details.
- **Projects (only those that exist):** one line each, with working links.
- **Stated hands-on experience:** skills the candidate says they have used at work. Treat as claimed experience, never as gaps.
- **Knowledge but no work experience:** skills for the skills row only.
- **Denied or never claim:** tools, titles or projects that must never appear.
- **Open conflicts:** facts the candidate has stated two ways, to confirm once.

If no fact bank exists, ask the user to paste their current resume, extract the facts, show them as a short list, and let the user correct it before saving.