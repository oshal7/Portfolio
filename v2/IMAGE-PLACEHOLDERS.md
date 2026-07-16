# Image placeholder index

Every image slot across the three case studies, with a stable ID. When a picture
is ready, just tell me the **ID** (e.g. "here's COH-01") and I'll drop it in — or
do it yourself using the two-step process at the bottom.

Naming: `REC` = Recovery Readiness · `COH` = Cohesity · `TAI` = TalentAI · `AXB` = Axis Bank.

---

## Recovery Readiness — `case-study-recovery-readiness.html`

| ID | Ratio | Where | What to put there |
|----|-------|-------|-------------------|
| **REC-01** | 21:9 banner | 00 / overview | Hero — recovery readiness dashboard with a live readiness score |
| **REC-02** | 16:9 | 01 / context | The passive protection loop — backups run, recovery never rehearsed |
| **REC-03** | 16:9 | 03 / design approach | Readiness framework — dimensions, score model, drill loop |
| **REC-04** | 16:9 | 04 / final solution (left) | Readiness score & drill scheduler |
| **REC-05** | 16:9 | 04 / final solution (right) | Recovery drill report — actual vs. promised RTO |

---

## Cohesity — `case-study-cohesity.html`

| ID | Ratio | Where | What to put there |
|----|-------|-------|-------------------|
| **COH-01** | 21:9 banner | 00 / overview | Hero — the integrated MongoDB protection dashboard in DataProtect |
| **COH-02** | 16:9 | 01 / the problem | Before-state map — DBAs juggling Cohesity + Ops Manager + manual scripts |
| **COH-03** | 16:9 | 03 / design process | Sprint artifacts — journey maps, the five high-impact moments |
| **COH-04** | 16:9 | 04 / final solution (left) | Topology-aware replica-set visualisation |
| **COH-05** | 16:9 | 04 / final solution (right) | Point-in-time recovery timeline scrubber |

## TalentAI — `case-study-talent-ai.html`

| ID | Ratio | Where | What to put there |
|----|-------|-------|-------------------|
| **TAI-01** | 21:9 banner | 00 / overview | Context hero — TalentAI inside a familiar WhatsApp thread |
| **TAI-02** | 16:9 | 03 / design process | Conversation flow map — 11 core flows in FigJam |
| **TAI-03** | 9:18 phone | 04 / final solution (left) | Resume review flow |
| **TAI-04** | 9:18 phone | 04 / final solution (right) | Skill-gap analysis flow |

_(The WhatsApp chat mockup in section 01 is real CSS, not a placeholder — no image needed.)_

## Axis Bank — `case-study-axis-bank.html`

| ID | Ratio | Where | What to put there |
|----|-------|-------|-------------------|
| **AXB-01** | 21:9 banner | 00 / overview | Hero — Axis Bank app framed by accessibility affordances |
| **AXB-02** | 1:1 square | 01 / the environment | Axis Design Labs (ADL) badge |
| **AXB-03** | 16:9 | 02 / scope of work | Scope illustration — design system × research intersection |
| **AXB-04** | 16:9 | 04 / other contributions | Slider component for the Subzero design system |

---

## How to replace a placeholder yourself

1. **Add the image file.** Create an `assets/` folder next to the HTML page and
   save the picture as the ID in lowercase, e.g. `assets/coh-01.png`
   (`.jpg` / `.webp` are fine too — just match the filename in step 2).

2. **Swap the placeholder for an `<img>`.** In the HTML, find the slot by its ID.
   Each one already has the exact tag to paste, in a comment right above it:

   ```html
   <!-- COH-01 · replace with: <img src="assets/coh-01.png" alt="..."> -->
   <figure class="shot">
     <div class="ph banner"><span class="ph-id">COH-01</span> … </div>   ← delete this line
     <figcaption><b>Fig 01.</b> One pane of glass for every MongoDB source.</figcaption>
   </figure>
   ```

   Replace the `<div class="ph …">…</div>` line with:

   ```html
   <img src="assets/coh-01.png" alt="Integrated MongoDB protection dashboard">
   ```

   Keep the `<figure>` wrapper and the `<figcaption>` — the image inherits the
   rounded corners, spacing, and caption styling automatically.

That's it. Ratios are fixed by the placeholder, so nothing shifts when you swap in
the real image — as long as your file roughly matches the listed aspect ratio.
