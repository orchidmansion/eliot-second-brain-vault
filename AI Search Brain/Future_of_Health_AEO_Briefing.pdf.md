# Future of Health _ AEO Briefing.pdf

# Citation Gap / Prompt Set Methodology

## Context

R/GA is co-developing The Citation Gap with AthenaHQ as the headline finding inside the Future Vision Health report. Prompts run through the Athena UI across five answer engines, results exported. This brief sets out how the team produces the prompt set at category scale, across eight categories in US health and wellness. 

## Scope

A category-scale measurement exercise.  Geography: US only.  Tier 1 categories (priority depth): 

1. Fitness apps and digital coaching 2. Wearables 3. Gyms and premium fitness clubs 4. Mental health and mindfulness 

 Tier 2 categories (covered, lighter depth): 

5. Nutrition (protein, supplements, RTD) 6. Weight management (GLP-1 medications and support apps) 7. Sleep and recovery 8. Longevity 

 Brand universe: top 10 to 12 brands per category, provided in companion CSV/Google sheet.  Consumers of the output: 

- R/GA strategists, interpreting the export.  Yael Cesarkas - The Future Vision Health report and its launch programme, publishing the findings. 

 Success criteria: a defensible Share of Answer index at category and sub-category level,  with cross-category insight on consumer journey stacking, ready for publication mid-May.  Deliverable 

One master CSV for sharing with Athena, tagged by category and sub category with a cross category flag.   Answer engines Five engines run by Athena across all prompts: 

1. ChatGPT (OpenAI) 2. Gemini (Google) 3. Claude (Anthropic) 

 Optional 

4. Perplexity 5. AI Overviews (Google) 

## Sub-category taxonomy

The unit of analysis is the sub-category. Taxonomy below. Strategists to confirm before lock. 

### Tier 1

Fitness apps and digital coaching - AI personal coaching - Running and endurance - Strength training - Group and streaming classes - General tracking and utility - Sport-specific (cycling, swimming, golf) 

 Wearables 

- Premium smartwatches - Performance and athletic watches - Smart rings - Budget bands - Sleep and recovery focused - Continuous health monitoring (CGMs, blood pressure) 

 Gyms and premium fitness clubs 

- Budget HVLP - Mid-tier full-service - Premium and lifestyle - Ultra-luxury - Boutique and specialty 

- Recovery and social clubs - Community and civic 

 Mental health and mindfulness 

- Meditation and mindfulness - Clinical therapy (text and video) - AI companions - Mood and behaviour tracking - Sleep and relaxation content - Anxiety and depression specific - Workplace and B2B 

### Tier 2

Nutrition - Whey and protein powders - Ready-to-drink shakes - Protein bars - Plant-based - Collagen and wellness - Sports performance 

 Weight management 

- GLP-1 medications - GLP-1 support and tracking apps - Behavioural and CBT programs - Telehealth prescribing - Off-ramp and maintenance 

 Sleep and recovery 

- Sleep tracking and analysis - Sleep aids and supplements - Recovery devices - Recovery clubs and spaces - Breathwork and relaxation 

Longevity - Biomarker testing - Longevity supplements - Longevity clinics and protocols - Hormone optimisation - Cellular health and anti-ageing 

## Cross-category prompt set

Health and wellness is one consumer journey. Cross-category prompts capture how categories stack and where engines co-recommend.  High-value cross-category pairs: 

- Wearables × Fitness apps - Wearables × Sleep and recovery - Wearables × Weight management (CGMs and GLP-1 tracking) - Fitness apps × Nutrition - Mental health × Sleep - Weight management × Nutrition (post-GLP-1 protein support) - Longevity × Wearables × Nutrition (biohacker stacks) - Gyms × Recovery 

 Cross-category slice: ~150 prompts, distributed across the eight pairs.  Example shapes: 

- "What wearables pair well with GLP-1 tracking?" - "Best fitness app and wearable combinations" - "What brands belong in a longevity stack?" - "Gym memberships with strong recovery offerings" 

 These prompts surface co-recommendation patterns that single-category prompts miss. Likely the most quotable findings in the launch programme. 

## The matrix

Every prompt sits at the intersection of four axes. 

1. Query archetype (8): open recommendation, constrained recommendation, comparison, validation, problem-led, outcome-led, switching, information. 

2. Intent stage (3): awareness, consideration, decision. 3. Sub-category: drawn from the taxonomy. 4. Branding state (4): unbranded, need-anchored unbranded, branded comparison, 

branded validation.  Mix per sub-category: 

- 60% unbranded recommendation (drives Share of Answer) - 20% branded validation and comparison (drives Mention vs Recommendation) - 10% problem-led - 10% information 

 Plus a small negative-prompt slice (~5% of unbranded volume): "what should I avoid in X", "is X overrated", "downsides of X". Brand absence here is signal.  Variation within each cell comes from phrasing and structural variety in the templates, not from consumer segmentation. 

## Volume built up from sub-category

Volume is built from minimum cell sizes, not allocated top-down.  Per sub-category minimums: 

- Unbranded recommendation prompts: 30 (statistical floor for stable Share of Answer) - Branded validation and comparison: 10 - Problem-led: 5 - Information: 5 - Negative / avoidance: 3 - Total per sub-category: ~53 

 Roll-up: 

- Tier 1 (4 categories × ~6.5 sub-categories × 53 prompts): ~1,400 - Tier 2 (4 categories × ~5.5 sub-categories × 40 prompts, lighter depth): ~900 - Cross-category slice: ~150 - Pilot run and buffer: ~250 

Total: ~2,700 prompts  Each prompt runs across 5 engines: ~13,500 LLM responses generated. 

## Worked example: smart rings (sub-category under Wearables)

To make the matrix concrete, here's how one sub-category gets populated.  Brands in scope: Oura, Samsung Galaxy Ring, Ultrahuman Ring AIR, Amazfit Helio, RingConn.  Volume target: 53 prompts.  Coverage breakdown:  

Archetype slice Count Example prompts 

Unbranded recommendation 30 "What's the best smart ring to buy?" / "Most accurate smart ring" / "Top smart rings in 2026" / "Which smart ring should I choose?" 

Branded validation and comparison 

10 "Oura Ring 4 vs Samsung Galaxy Ring" / "Is Ultrahuman worth it over Oura?" / "Which smart ring brand is most reliable?" 

Problem-led 5 "I want to track my sleep better, what tech should I look at?" / "How do I monitor my recovery from training?" 

Information 5 "How do smart rings measure HRV?" / "What do smart rings actually track?" 

Negative / avoidance 3 "Smart rings I should avoid" / "Are smart rings overrated?" 

Every sub-category follows this pattern. Variation in each cell comes from phrasing variety in templates, not from consumer types. 

## Method

### Phase 1: Category framing (per category, parallelised)

- Reverse brief of the category and its sub-categories. - Deep Research per category. US sub-segments, brand landscape, consumer behaviour, 

top intents, pain points, current cultural narrative. - SEMrush keyword pull across the top 5 brands per category, deduplicated to a 

category keyword set. Volume signal informs vocabulary weighting. - Brand alias map per category: misspellings, abbreviations, product line names, parent 

company variants. Required for the prompt set and for Athena's pitch parameter setup. - LLM-assisted vocabulary generation. Feed Deep Research, SEMrush keywords, and 

brand alias map into Claude or Gemini. Generate category and sub-category vocab per category. Strategist reviews and trims. 

### Phase 2: Matrix design (per sub-category)

- Confirm sub-categories against the taxonomy. - Define the brand set in scope per sub-category. - Lock the volume target per sub-category against the 53-prompt floor (40 for Tier 2 

sub-categories). 

### Phase 3: Generation

- Template library: ~20 templates, slot-based. Written once, reused across categories. Each template carries archetype, intent stage, and branding state tags. 

- Vocabulary library: per category, variable values per slot, sourced from Phase 1. - Generation script: permutes templates and variables, applies stratified sampling so 

every archetype × intent × branding state cell hits its minimum. - Cross-category prompts: hand-curated for each high-value pair, ~20 per pair. - Health-specific edge case prompts: hand-curated for mental health, GLP-1, 

supplements, and longevity sub-categories. - Tagging: every prompt carries its full tag set into the final CSV. 

### Phase 4: QA

- Template review (Marc + strategist, half day). If templates are right, prompts are right. - Vocabulary review (lead analyst, half day). Does the vocab match the category. - Cross-category prompt review (Marc + strategist, half day). - 50-prompt pilot upload before committing the full set. Look for prompts that all return 

the same five brands, prompts engines refuse, prompts that don't trigger recommendations, engine guardrail patterns. 

- 5% random sample human read-through on the full set. - Cell completeness check: automated audit that every required cell hits its minimum 

prompt count. 

## Health-specific edge cases (do not skip)

Some sub-categories will hit engine guardrails. This is itself a finding for the study.  

- Mental health crisis prompts: engines respond with hotline information rather than brand recommendations. Test how they handle "I'm anxious every day, what app should I try?" vs "I'm having panic attacks, what should I do?" The shift point is the finding. 

- GLP-1 side effect prompts: engines hedge medical claims. Test how they recommend within those guardrails. 

- Supplement and longevity claims: engines vary widely in how they handle unverified efficacy claims. This drives citation patterns. 

- Pricing and accessibility prompts: insurance, cash-pay, and budget framing.  Include a deliberate guardrail-aware prompt set (~5 per sensitive sub-category) so the export captures these patterns. 

## Deliverable format

Eight category CSVs (one per category, mapping to one Athena pitch each) plus one cross-category CSV.  Per-category CSV columns:  prompt_id, sub_category, archetype, intent_stage, branding_state, prompt_text  Cross-category CSV adds:  category_a, category_b  Within each CSV, sorted by sub_category then prompt_id.  File naming: {category}_prompts_v1.csv (e.g., wearables_prompts_v1.csv).  Companion documents:  

- Brand alias map (single CSV across all categories). - Template library (versioned, for re-runs). - Vocabulary library per category (versioned). - Methodology summary (1 to 2 pages, feeds the published transparency commitment). 

 Tags travel with the prompts so the response export comes back tagged. Analysis slices by any axis without recoding. 

## Task list for the team

# Task Owner Output 

1 Confirm sub-category taxonomy 

Marc + strategist Locked taxonomy doc 

2 Reverse brief per category (8 total) 

Strategist 8 reverse briefs 

3 Deep Research per category (8 total) 

Lead analyst 8 Deep Research docs 

4 SEMrush keyword pull per category, dedupe 

Data analyst Category keyword sets 

5 Brand alias map across all categories 

Lead analyst Single brand alias CSV 

6 Vocabulary generation per category (LLM-assisted) 

Lead analyst Vocab library 

7 Strategist vocabulary review and trim 

Strategist Approved vocab library 

8 Template library design (~20 templates) 

Strategist + data analyst 

Versioned template library 

# Task Owner Output 

9 Generation script Data analyst Script + generated prompt set 

10 Cross-category prompt drafting (~150 prompts) 

Strategist Cross-category CSV 

11 Health-specific edge case prompt set (~40 prompts) 

Strategist Edge case prompts integrated 

12 Cell completeness check 

Data analyst Pass / fail audit log 

13 50-prompt pilot upload 

Marc Pilot response data 

14 Pilot review and adjustments 

Marc + strategist Locked final set 

15 5% sample audit on full set 

Lead analyst Audit log 

16 Final CSVs + companion docs to Athena 

Marc Delivered 

17 Methodology summary doc 

Strategist 1 to 2 page transparency doc 

## Ownership

- Marc: framework sign-off, Athena interface, pilot review, final delivery. - Lead analyst: Phase 1 grounding (Deep Research, SEMrush, brand aliases, vocab). - Strategist: Phase 2 matrix design, templates, cross-category prompts, methodology 

doc. - Data analyst: Phase 3 generation script, Phase 4 audits. - Eliot or Nico: delivery oversight. 

## Timeline

Working back from Athena upload date.  

- Day 1: framework and taxonomy lock. Phase 1 kicks off across all 8 categories in parallel. 

- Days 2 to 4: Phase 1 outputs complete. Deep Research, SEMrush, brand aliases, vocab. 

- Day 5: Phase 2 sub-category and brand set selection. - Days 6 to 7: Phase 3 templates, vocabulary library, generation script, prompt set 

generated. - Day 8: Cross-category and health edge case prompts drafted. - Day 9: Phase 4 pilot, audits, adjustments. - Day 10: Final CSVs and companion docs delivered. 

 ~10 working days end to end. ~6 to 7 person-days of effort. Re-runnable for free after. 

## Cost estimate

Item Cost 

Athena UI compute (Path A, 5 engines, ~2,700 prompts) 

Bundled in partnership 

Anthropic / Gemini API for Deep Research and vocab generation 

~$50 to $80 

SEMrush On contract 

Total external spend ~$80 

 Team time: ~6 to 7 person-days. 

## Out of scope

Scoring framework, Share of Answer index logic, dashboard, brand-level recommendations. All come after the data lands. 

## Open for working team

- Personas. Marc's recommendation is to operate at the broad category level, no 

personas, no granular use cases. Trade-off: cleaner category-level Share of Answer signal, less coverage of long-tail consumer-specific brand citations. Team to weigh in before lock. 

- Sub-category taxonomy. Proposed above. Strategists to confirm. - Brand alias generation. Manually per brand list, or extracted from SEMrush data? - Cross-category prompt distribution. Proposed ~20 per pair. Strategist input on 

priority.   