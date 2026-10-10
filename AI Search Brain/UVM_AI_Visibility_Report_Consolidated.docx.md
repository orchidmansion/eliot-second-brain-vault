# UVM_AI_Visibility_Report_Consolidated.docx

**TOYOTA USED VEHICLES MARKETPLACE (UVM) — AUSTRALIA**

**AI Visibility Report: Cross-Persona Findings**

*City SUV Upgrader (RAV4)  ·  Practical Ute Buyer (HiLux)  ·  Seller / Trade-In (Instant Valuation)*

Prepared: 20 July 2026

Data window: 15–20 July 2026  ·  390 AI responses across ChatGPT, Gemini, Google AI Overview

**Executive Summary**

UVM dominates AI answers when someone is buying a used Toyota — and nearly disappears when the same person is selling one.

Buying: UVM leads decisively on both RAV4 (63% visibility, position 1.5) and HiLux (67%, position 2.0) searches, well ahead of Carsales.

Selling: on Trade-In queries, Carsales leads at 45% visibility and position 1.7; UVM sits at 5% and position 10 — with a measurement caveat below that this number likely understates UVM.

One mechanism explains the buying-side gap, and it replicates across two unrelated vehicle categories: mention “Certified”/TCPO or Toyota as a purchase channel, and UVM appears 73–100% of the time. Leave it out — even in a Toyota-branded query — and visibility drops to 0–33%.

Cars24’s apparent presence in HiLux data is a query-framing artifact: it's mentioned only in the one prompt that names it, never independently.

The Trade-In numbers carry a real caveat: AI answers describe Toyota’s Instant Valuation tool in 53% of responses, but brand-tracking only credits 5% of those as a UVM mention — flagged for the team to resolve, not treated as settled fact here.

|   |

| --- |

**Methodology**

Three tracked personas, each with its own chat export (individual AI responses), prompts export (aggregate visibility/position/sentiment per prompt, with branding and intent tags), and Top Brands export (competitive set for that persona).

City SUV Upgrader / RAV4: 120 responses, 10 prompts, 16–17 July.

Practical Ute Buyer / HiLux: 150 responses, 10 prompts, 15–17 July.

Seller / Trade-In: 120 responses, 10 prompts, 15–20 July.

Top Brands exports are scoped to each persona's own tracked prompt set, not a single global aggregate — competitive-set numbers should be compared within a persona, not across personas. Load-bearing external claims (Toyota warranty terms, HiLux market position, product announcements) were verified by web search before inclusion; see the Fact-Check appendix.

**1. The Cross-Persona Mechanism: What Actually Drives a Mention**

Both buying personas were tested against the same hypothesis: does the query invoke Toyota's own Certified Pre-Owned program (“certified,” “TCPO”) or name Toyota explicitly as a purchase channel (“Toyota dealer,” “through Toyota”)? The split is stark and consistent in both datasets.

|   |   |   |   |   |

| --- | --- | --- | --- | --- |

|   |   |   |   |   |

|   |   |   |   |   |

The one-off exceptions in each dataset (RAV4's 33%, HiLux's 7%) are both “asking about a specific vehicle/stock without naming the program” — consistent with the pattern, not contradicting it. This held regardless of whether the underlying query was transactional (“find me a HiLux”) or advisory (“is a Certified HiLux the best option”) — an earlier “advice vs. transactional” hypothesis didn't survive testing and was dropped in favour of this one.

|   |

| --- |

**2. City SUV Upgrader / RAV4**

**2.1 Competitive landscape**

|   |   |   |   |   |

| --- | --- | --- | --- | --- |

|   |   |   |   |   |

|   |   |   |   |   |

|   |   |   |   |   |

**2.2 The funnel gap**

81% mention rate on transactional/bottom-funnel prompts (stock, warranty, dealer vs. private) vs. 0% on top-funnel research prompts (“best SUV for a family,” “best RAV4 model year”) — even when the research prompt names the RAV4 directly. Superseded by the sharper “Certified” finding in Chapter 1, but the underlying data holds.

**2.3 Citation mechanism and platform gap**

Citing toyota.com.au as a source → 91% UVM mention rate. Not citing it → 13%.

Google AI Overview cites toyota.com.au in only 43% of relevant answers, vs. 70% (ChatGPT) and 55% (Gemini) — the weakest surface, and likely the highest-reach one for early research.

**The only two explicit toyota.com.au deep links found in any answer are both facet/category pages (/used-vehicles/search/Toyota/RAV4, /used-vehicles) — never a VIN-level listing. Carsales' one explicit link is the same shape (/cars/suv-bodystyle/). Category pages, not product listings, are what gets cited.**

**2.4 What to do**

Build facet/category URLs matching the losing intents (best-by-model-year, hybrid-vs-petrol, family-SUV cross-model), with live-inventory-backed answer copy on the page itself — not a separate blog.

Audit indexability of those facets before writing copy; marketplaces routinely noindex deep filter combinations.

Move schema investment (ItemList, FAQPage) from PDPs to category pages.

Prioritise Google AI Overview — treat its gap as a technical/indexability fix, not a content gap.

**3. Practical Ute Buyer / HiLux**

**3.1 Competitive landscape**

|   |   |   |   |   |

| --- | --- | --- | --- | --- |

|   |   |   |   |   |

|   |   |   |   |   |

|   |   |   |   |   |

|   |   |   |   |   |

UVM's own average position (2.00) is softer here than on RAV4 (1.50) — driven by the one three-way comparison prompt below, not a broad weakness.

**3.2 Cars24: real competitor or framing artifact?**

Artifact. Cars24 is mentioned in exactly one of ten prompts — the one that literally names it in the question (“…through Toyota vs Carsales or Cars24”) — and never once independently of Carsales (0 of 15 co-occurrences broken). cars24.com.au is barely cited as a source anywhere else. The Top Brands jump from 0% (RAV4 period) to 12% (HiLux period) reflects the tracked prompt set including a Cars24-naming prompt, not Cars24 gaining real ground.

**3.3 Fact-check: claims worth verifying before they inform strategy**

C1 — “TCPO covers HiLux/commercial vehicles; the extended warranty is void only for commercial use (rideshare, taxi, goods-for-payment), not for the vehicle being a ute.” ✅ Verified against toyota.com.au's own TCPO warranty terms. A tradie using their own ute for their own work is not excluded.

C2 — Toyota announced a factory-fitted GVM upgrade for the HiLux (from $4,000, arriving August 2026, retains full 5-year warranty — unlike aftermarket kits, which can void it). ✅ Verified (CarExpert, The Beep, Torquecafe, June 2026). This postdates the data collection window — a live, narrow, low-competition content opportunity, not yet saturated by third-party sites.

C3 — AI answers describe HiLux as “one of Australia's best-selling vehicles” without claiming #1. ✅ Verified and accurately hedged — Ford Ranger holds the top spot (VFACTS, third year running); HiLux is consistently #2. No correction needed.

**3.4 What to do**

Apply the Chapter 1 mechanism directly: build “Certified HiLux”-anchored facet pages for the exact losing intents (which-year-for-towing, commercial-use checklist).

Fast-track a GVM-upgrade content page ahead of the August 2026 factory launch — timing matters here.

Don't over-invest defensively against Cars24 based on the Top Brands trend line; it's a measurement artifact of prompt composition, not a market signal.

**4. Seller / Trade-In Motivated**

**4.1 Competitive landscape**

|   |   |   |   |   |

| --- | --- | --- | --- | --- |

|   |   |   |   |   |

|   |   |   |   |   |

|   |   |   |   |   |

|   |   |   |   |   |

A near-total reversal of the buying-persona pattern. Carsales leads on both frequency and position; UVM is rarely named and, when it is, buried near the bottom of the list (position 10, vs. ~1.1–2.0 elsewhere in this report).

**4.2 Read this number with a caveat**

|   |

| --- |

What isn't in question: Carsales' 45% is measured the same way throughout this report, and it's a real, large lead — independent of how the UVM number resolves.

**4.3 What to do**

Resolve the tracking-scope question first. If Instant Valuation should count as UVM and isn't being credited, this may be a measurement fix, not a content fix — cheaper and faster than either.

Assume the Chapter 1 mechanism won't transfer as-is: there's no “certified” equivalent in a selling journey. The likely analogue is naming “Toyota Instant Valuation” explicitly — worth testing once the tracking question is settled, rather than porting the buying-side playbook wholesale.

Regardless of the UVM number, Carsales' lead here is real and should be treated as the primary competitive gap for this persona.

**5. Recommendations, in priority order**

Build “Certified”-anchored facet/category pages for RAV4 and HiLux, targeting the specific losing query intents identified in each chapter, with live-inventory copy on the page itself.

Audit facet indexability before writing new copy — likely faster and cheaper than a content program, and a prerequisite for it to matter.

Move schema investment from PDPs to category pages (ItemList, FAQPage); the citation evidence points there, not to listings.

Prioritise Google AI Overview specifically — lowest toyota.com.au citation rate on the buying side, likely highest reach for early research.

Ship HiLux GVM-upgrade content ahead of the August 2026 factory launch.

Resolve the Instant Valuation tracking-scope question before committing budget against the Trade-In persona's 5% figure.

Once resolved, treat Trade-In as its own strategy — test whether naming “Toyota Instant Valuation” explicitly does for selling what “Certified” does for buying, rather than assuming the mechanism transfers.

Re-run tracking after changes. Watch specifically whether Cars24 stays confined to named comparisons (artifact, as now) or starts appearing independently (a real shift worth re-assessing).

**Appendix: Fact-Check Summary**

|   |   |   |

| --- | --- | --- |

|   |   |   |

|   |   |   |

|   |   |   |

**Appendix: Methodology Notes and Limitations**

“Mention” = brand name appears in the AI response's tagged mentions field. “Position” = rank among mentioned brands within that answer (1 = first-named).

Top Brands figures are scoped to each persona's own tracked prompt set — don't compare raw visibility percentages across personas as if drawn from the same competitive universe.

The Trade-In persona's UVM visibility figure (5%) may understate real presence; see §4.2. Treated as flagged, not resolved, throughout this report.

“Cites toyota.com.au” includes the root domain and Toyota dealer subdomains appearing in a response's listed sources.