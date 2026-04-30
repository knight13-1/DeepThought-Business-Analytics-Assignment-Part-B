# Proposal: 1000 ICP-Qualified Companies in One Month
### Scale-up Strategy — Business Analytics Internship, DeepThought
**Candidate:** Yash Raj Gupta  

---

## 1. Objective
The goal is to build a verified list of 1,000 "Federer" ICP companies (Indian specialty manufacturers, Rs. 50Cr–Rs. 500Cr, promoter-driven, technical decision-makers) within 30 days. 

Based on the preliminary research in the Indore Agri-Tech segment, a **30% yield** is expected. To reach 1,000 verified passes, we must ingest and process a starting universe of **~3,500–4,000 companies**.

---

## 2. Sourcing the Universe (Week 1)
To avoid the "surface-level Google search" trap, we will utilize high-signal technical registries to build our initial 4,000-company pool.

### Primary Sources:
1. **DSIR-Recognized R&D Units:** Department of Scientific and Industrial Research list (~3,000+ technical firms).
2. **Specialty Export Data (Zauba/Volza):** Filtering for niche HS codes (e.g., hybrid seeds, bio-pesticides) to find manufacturers with international technical standards.
3. **PLI Scheme Beneficiaries:** Government lists for Production Linked Incentives in Specialty Chemicals and Agri-inputs.
4. **BSE SME / NSE Emerge:** Small-cap listed entities which provide transparent financial and leadership data for rapid scoring.
5. **Technical Expo Directories:** Exhibitor lists from events like *Agri Intex* or *CPHI India*.
6. **MCA Filings (NIC Codes):** Bulk extraction via Antigravity for specific manufacturing NIC codes within target industrial hubs like Pithampur and Sanwer Road.

---

## 3. Automated Scoring Pipeline (Week 2-3)
Manual research for 4,000 companies is impossible. We will deploy a "Scientific Execution" engine using a Python-AI stack.

### The Stack:
* **Scraper:** Python + Playwright (handles JavaScript-heavy sites) to scrape the Homepage, /About, /Products, and /News sections.
* **Filter:** A programmatic "Hard Filter" to auto-disqualify traders, distributors, or companies with revenue >Rs. 500Cr (via Tofler API).
* **Scoring:** Claude Haiku API for first-pass scoring of the 6-criteria rubric (C1–C6).
* **Deep-Dive:** Claude Sonnet for re-scoring "Borderline" cases (scores between 40-59).

### Speed & Cost Estimate:
* **Scraping:** ~12 hours using 4 parallel workers.
* **AI Scoring:** ~5 hours via API batch processing.
* **Total AI Cost:** ~Rs. 4,000 (Haiku + Sonnet usage).

---

## 4. Human Quality Assurance (Week 3-4)
Human judgment is reserved for high-stakes verification and borderline cases flagged by the AI.

### The QA Workflow:
1. **The Borderline 400:** We will manually review the ~400 companies that the AI flagged with "low confidence" or "borderline scores."
2. **C3/C4 Verification:** Manually verifying PhD/Technical credentials on LinkedIn for the top-priority targets.
3. **Growth Signal Audit:** Spot-checking "C6 Evidence" to ensure news or hiring signals are current (post-2024).
4. **Final Assembly:** Deduplication of the master list and generation of personalization hooks for the top 200 "Strong Federer" targets.

---

## 5. Weekly Execution Roadmap

| Week | Focus | Output |
|:---|:---|:---|
| **Week 1** | **Ingestion** | Raw master list of 4,000 companies across all target manufacturing segments. |
| **Week 2** | **Automation** | Scraper-Scorer loop completed; 1,300 first-pass "Passes" identified. |
| **Week 3** | **Refinement** | Human QA on borderline cases; re-scoring completed for high-priority tiers. |
| **Week 4** | **Packaging** | Final list of 1,000 verified companies + Personalization hooks for the Top 200. |

---

## 6. Risk Mitigation
* **Low Yield:** If the yield drops below 30%, we will expand the sourcing universe to include state-level industrial directories (e.g., MP AKVN or MIDC).
* **Scraper Block:** Using residential proxies and rotating user agents to ensure continuous data extraction without getting blacklisted.
* **Accuracy:** Initial "Calibration Set" of 50 companies will be used to fine-tune the AI scoring prompts before running the full 4,000-company batch.

---
*DeepThought | Building the AI Execution Workspace*
