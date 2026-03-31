# Job Search Workflow Instructions (Interactive Sessions)

## Candidate Profile
- **Name:** Killian Louis Grant
- **Targets:** Engineering Manager, Technical Lead, Lead Engineer, Staff Engineer, Principal Engineer, Senior Engineer, Solutions Architect
- **Level exclusions:** No VP or Director-level roles
- **Location:** Remote US or Denver area
- **Compensation:** Binary pass/fail. Max salary >= $180K = pass, max < $180K = skip. Ranges starting below $180K but extending above are acceptable. NEVER editorialize about salary: no "lower end", "tight", "barely passes", no comparisons between positions, no flagging salary as a concern or gap. This has been corrected multiple times. Stop.
- **Citizenship:** US Citizen

## Exclusions
- Reddit, Meta, Amazon, X, Palantir, Flock Safety, Discord
- Defense/Military contractors
- Crypto/Web3
- Gambling

## Stack Fit (Hard Filter)
**Preferred:** TypeScript, Node.js, React, Next.js, Vue/Nuxt, GraphQL, PostgreSQL, MongoDB, AWS, GCP, Docker, CI/CD, Svelte, Redis, Rust, PHP/Laravel
**Auto-skip ONLY:** Ruby, .NET/C#, Kubernetes, Terraform, C++, Swift
- Python, Java, Go, and other languages are fine. Candidate can adapt.
- For leadership roles (Day A), stack matters less since the candidate won't be extremely hands-on.
- **Infra roles:** OK if focused on Docker, TurboRepo, IDEs, CI/CD, developer tooling. Auto-skip if centered on K8s, Helm, Terraform, SRE, or cloud provisioning.

## Fit Quality Gate
**Every position must pass ALL checks before being added to a daily batch.**
1. **Stack match:** Prefer TypeScript. Auto-skip ONLY if Ruby, .NET/C#, K8s, Terraform, C++, or Swift is mandatory. Everything else is fine.
2. **Role type:** Product/platform/full-stack engineering only. Auto-skip: security-focused, GTM/sales-adjacent, solutions architect (unless explicitly engineering), pure data/ML engineering, pure infra/SRE
3. **Location:** Posting explicitly says "Remote US" or Denver-eligible. Never assume "remote" = US; check for region restrictions
4. **Salary:** Binary pass/fail per Candidate Profile rules above
5. **Skills gap:** If JD requires domain expertise the candidate lacks with no genuine adjacent bridge, skip. "Adjacent" = substantially similar work done (KMP ↔ React Native). NOT "could probably learn" or "vaguely related area"
6. **Dedup:** Check Application Tracker for company+role. Applies to initial picks AND replacements
7. **Title alignment:** Day B (IC+) prioritizes Staff/Principal. Senior OK only if JD scope is clearly staff-level (architecture ownership, mentoring, cross-team influence)
8. **Full JD read:** Read every section: description, requirements, "about you", location, salary, AND the application form/instructions. Extract essay questions or custom prompts before writing anything
9. **Conservative by default:** Not clearly a good fit? Skip. No Stretch-rated positions. 8 strong > 10 with 2 bad. When in doubt, skip.

## Per-Application Workflow (Gated Phases)

### Phase 1: QUALIFICATION
1. **Verify URL is live:** Open in Chrome. Confirm JD text is readable (not 404/redirect/home page). Dead → replace immediately.
2. **Read full JD + application form:** Extract essay questions, custom prompts, Easter eggs. Document before writing.
3. **Run Fit Quality Gate** (all 9 checks above). ANY failure → STOP, find replacement.

### Phase 2: VARIANT GENERATION (only after Phase 1 passes)
4. Fit assessment (Standout, Gaps, Why) → update Application Tracker
5. Extract keywords: Hard Skills, Domain Skills, Leadership Skills from JD
6. Tailor resume per TAILORING_CHECKLIST.md; tailor cover letter (answer all prompts, weave Easter eggs)
7. Verify word counts: resume 475-600w, cover letter 200-300w

### Phase 3: FILE VERIFICATION
8. Run `ls -la variants/` and confirm both files exist with non-zero bytes. Missing → regenerate.

### Phase 4: USER REVIEW
9. Present materials for approval → incorporate feedback → open application tabs

## Mandatory Resources
- **TAILORING_CHECKLIST.md** (in /Claude): Read and follow for every variant. Document fit assessment before writing, final check after.
- **Job Search Resources.md:** Update when finding new career pages, boards, or exhausting a company.
- **Application Tracker.md** (in /Claude): Update at every status change (Ready → In Progress → Applied → Phone Screen, etc.). Include: Fit rating, Standout, Gaps, Why This Role.
- **dedup.txt** (in /Claude): Append "Company | Role" when marking anything Applied. The scheduled agent checks this before opening JD tabs to avoid re-surfacing completed roles.
- **Master resumes** (in /masters): Always review for accurate dates, titles, experience. Never fabricate.
- **role-context-and-stories.md** (in /Claude): Narrative context for cover letters and SA applications.

## Resume Variant Rules
Research-backed: 475-600 word resumes get ~2x interview rate; over 600 words sees 43% drop in callbacks.

### Structure
H1 Name > H3 Headline > Contact > --- > Intro (2-3 sentences) > --- > ## Experience > ### Company, *Title* | Dates > --- > ## Skills > --- > ## Education

Experience before Skills (recruiter F-pattern scan). Skills at bottom (ATS keyword index).

### Density
- **475-600 words total.** Over 600 → cut.
- 3 bullets max per recent role, 2 for older roles (8+ years) unless directly relevant
- 15-20 total experience bullets
- Each bullet: 1 line, 180-200 chars max, action verb, metric/outcome where possible
- Intro: 2-3 sentences max

### Measurable Results
Intro and most recent role are scanned first. These MUST contain time-based statements AND improvement metrics.
- **DrWell exception:** Team laid off before product shipped. No outcome metrics. Emphasize scope, architecture, technical leadership. Compensate with extra TheKey metrics.

### Skills Section
Two subsections: `#### Hard` and `#### Soft`, each a flat comma-separated list. 10-15 keywords total mirroring JD language. Include both technical and leadership terms for ATS.

### Cover Letter
Same header as resume. No emdashes. 3-4 paragraphs, 200-300 words. Tone mirrors JD voice. First paragraph: why this company specifically. Middle: map experience to JD with examples. Close: brief, confident.
- **No anecdotes.** Do not tell stories with narrative arcs (setup, incident, resolution). State qualifications and relevant experience directly. Anecdotes are saved for behavioral interviews, not cover letters.
- **No editorializing.** Do not add commentary, color, or framing beyond what's needed to connect experience to the role. Say what you did and why it's relevant. Stop.
- **Answer ALL application-specific prompts** from the apply form
- **Scan for Easter eggs** in JD; weave naturally into letter. Easter eggs are deliberate puzzles or hidden instructions that test whether a candidate read carefully: e.g., a required API call before applying, an acronym puzzle with an exact word-count constraint, a specific phrase to include. They are NOT: standard consent disclosures, legal notices, form boilerplate, interview logistics ("we record interviews"), or any information that any reader would casually notice. If it requires no effort to find and no judgment to respond to, it is not an Easter egg. Do not acknowledge it.

### Keyword Threading
Identify JD's core theme. Rewrite every bullet to echo that theme using JD language, as long as underlying work is truthful. Never fabricate; only reframe.

### What to Cut from Master
Reduce to 3 bullets per role (pick most relevant to THIS JD). Trim/remove 8+ year old roles. Compress intro. Trim skills to 10-15 most relevant.

## Anti-Patterns

### Resume Anti-Patterns (from LifeShack/Teal Analysis)
- **Keyword clause appending:** No "demonstrating experience with X" tacked onto bullets
- **Metric stripping:** Never remove real metrics for keyword stuffing
- **Fabricating AI into old roles:** No "AI/ML" on 2015 work unless it actually used it
- **Identical skills sections:** Must be tailored per application
- **Excessive length:** Not more than 600 words. 3 bullets max per role.
- **Excessive skill categories:** Stick to Hard/Soft split only
- **Shoehorning JD theme:** Only reframe where work genuinely connects

### Execution Anti-Patterns (corrected multiple times; do not repeat)
- **Opening tab ≠ verification:** Read the page. Confirm JD text visible, apply form loads.
- **Skipping application instructions:** Essay questions must be documented before writing
- **Rationalizing hard skill gaps:** "Could learn" is not credible for security, networking, legal, ML research, or mobile-native roles
- **"Remote" ≠ "Remote US":** Verify region. Check sidebar/fine print.
- **Skipping dedup on replacements:** Every replacement gets dedup-checked
- **"Variant generated" without file check:** Run `ls` and confirm non-zero bytes
- **Leaving "Ready" backlog:** Every "Ready" entry must get materials generated before task is done. No exceptions.
- **Using WebSearch instead of Chrome for boards:** ZenSearch, BuiltIn, etc. must be browsed in Chrome. WebSearch returns stale/incomplete results for dynamic boards.
- **Stopping at 3-4 when target is 5-6:** 4 is the minimum before giving up, not the target. Keep searching if boards remain.
- **Not toggling ZenSearch filters:** ZenSearch profile may be configured for a different day type. Toggle filters to match today's rotation.
- **Calling standard disclosures Easter eggs:** Consent notices, recording disclosures, legal boilerplate, and interview logistics are not Easter eggs. Do not flag them, do not mention them in cover letters, do not document them as special findings. Read the JD; the information you need is there.
- **Closing JD tabs without confirmation:** NEVER close a candidate's JD tab unless the user explicitly confirms they have applied. Tabs persist until the user says so. This applies to both interactive sessions and the scheduled agent.
- **Creating new tabs instead of reusing existing ones:** CAPTCHA/bot detection triggers more often when creating fresh tabs. Reuse existing tabs in the tab group by navigating them to new URLs. If the user has a site open outside the tab group, ask them to add it rather than opening a duplicate.

## Positioning & Differentiators
- **People-focused leader first;** only emphasize hands-on if JD requires it
- **Team scaling:** 5→50 at Spire, 35-person cross-functional at Fruition
- **AI/LLM:** TheKey production ML (88% reduction), agentic workflows
- **Ordering platforms:** Codelab303 restaurant, DrWell fulfillment, Kin+Carta B2B
- **Mobile:** Codelab303 KMP health app; TheKey backend powering 3 mobile apps
- **Healthcare/regulated:** DrWell compliance, audit logging, RBAC
- **SaaS modernization:** Monigle legacy DAM to multi-tenant SaaS

## Daily Search

### Schedule Rotation
A → B → C → repeat. Check most recent job-feed entry for previous day type.
- **A (Leadership):** Engineering Manager, Technical Lead, Lead Engineer, Head of Engineering
- **B (IC+):** Staff Engineer, Principal Engineer, Staff Software Engineer
- **C (IC):** Senior Engineer, Solutions Architect, Senior Software Engineer

### Process
1. Browse boards in Chrome (not WebSearch): ZenSearch, BuiltIn, HiringCafe, WellFound, TrueUp. Check HN Who's Hiring if recent.
   - ZenSearch: toggle role/keyword filters to match today's day rotation. Browse 2+ pages.
   - BuiltIn: search by role title AND stack keywords. Browse 2+ pages.
2. For each candidate found, complete the FULL pipeline before moving to the next:
   a. Verify URL is live in Chrome (not 404/redirect/closed)
   b. Read full JD + application form
   c. Run Fit Quality Gate. ANY failure → skip, move to next
   d. Generate tailored resume (475-600w) + cover letter (200-300w)
   e. Verify files exist with non-zero bytes
   f. Update Application Tracker
   g. Keep JD tab open for the user
3. Use WebSearch ONLY to find direct ATS URLs after identifying candidates. Not as a substitute for browsing.
4. Target 5-6 fully completed (with materials). Never pad with weak candidates. If 4 after all boards exhausted, proceed. If <4 and boards remain, keep searching.
5. Ensure domain diversity: mix of platform, healthcare, devtools, commerce, AI. No >50% in one domain.
6. Zero "Ready" backlog when done. Every candidate either has materials or was dropped with a reason.

### Technical Notes
- WebFetch is BLOCKED for ATS domains (Lever, Greenhouse, Ashby); use WebSearch or Chrome
- WebSearch does NOT work well for dynamic job boards. Always use Chrome for ZenSearch, BuiltIn, HiringCafe, WellFound, TrueUp.
- Never present a URL without confirming it resolves to a live posting
- Workspace folder may take seconds to mount. If `ls` returns empty, wait 5-10s and retry twice before concluding.
- Scheduled task and interactive sessions share the same Application Tracker
- Scheduled task must complete ALL phases: collect, validate, output, AND generate materials. Finding jobs without producing materials is a failed run.

### File Naming Convention
`Killian Louis Grant - [Company] - [Short Role Title].md` (and `- Cover Letter.md`)

### Titles Must Stay Accurate
Never change job titles to match JD. Only reframe bullet content, not titles.

### No Emdashes
Use colons or semicolons instead, in all documents.
