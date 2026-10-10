# Lightning talk delivered by Jing, Technical SEO realestate.com.au at Google Search Central Sydney 2026.docx

The Core Problem: The Danger of Uncontrolled Crawling

Jing opened by addressing a common anxiety among technical SEOs looking at their Index Coverage reports. She shared a cautionary truth originally stated by Google's Gary Illyes:

"Once Googlebot discovers a set of URLs, it cannot decide whether that URL space is good or not, unless it crawls a large chunk of it. By then, it's too late."

Failing to control this crawl behavior poses severe risks:

**Server Overload:** Unchecked bot traffic can overload hosting servers and potentially bring an entire website down.

**Protracted Recovery:** Recovering from major site-wide crawling and indexation errors can take a massive amount of time.

**Wasted Potential:** SEMrush identifies poor crawlability and unmanaged crawl budget as one of the single biggest operational mistakes a large website can make.

The Mindset Shift & Proof of Concept

To tackle this on an enterprise scale, Jing's team adopted a radical mindset shift: **Instead of focusing on how to get valuable pages indexed, they focused first on preventing the crawl and indexation of "the waste."**

They proved this concept on their sister site, *property.com.au*, which originally had a broken crawl budget structure that left 60% of its most valuable pages completely unindexed. By starving out the waste, they achieved exceptional growth:

**Indexation Rate:** Shot up from an initial 38% to an optimal 90%+ indexation efficiency.

**Organic Performance:** Yielded a 200% increase in daily organic SEO traffic, expanding daily clicks from 100,000 to 300,000.

1. Classifying the Site Hierarchy (The 3 Tiers)

E-commerce and marketplace search result structures are staggeringly complex, generating millions of potential filter combinations. To decide which URLs Googlebot should access, realestate.com.au categorizes all pages into three distinct tiers based on target search volume and traffic potential:

**Tier 1 (Must Index):** Pages exhibiting high user intent, delivering high user value, and matching high-to-medium search volumes.

**Tier 2 (Should Index):** Pages with meaningful user intent and good user value, but tied to relatively low search volumes.

**Tier 3 (Must NOT Index):** Pages with very low to zero search volume that exist solely for internal tracking or internal, on-site refinement.

2. Starving the Waste: Eliminating 3 Massive Crawl Traps

Jing highlighted three specific areas where large sites unintentionally hemorrhage crawl budget, along with the precise technical solutions her team executed:

A. Tracking Parameters

Marketing teams often append tracking parameters directly to links to monitor click paths. From an SEO perspective, this creates millions of duplicate URLs that decimate crawl budgets and break clean indexation.

**The Solution:** Realestate.com.au completely stripped tracking parameters from standard internal links. Instead, they transitioned to using client-side **browser local storage** to retain and track user pathing data without altering the URL strings.

B. Multiple Filter Combinations

Exposing crawlable links for every combination of multi-location or feature filters creates an infinite web of zero-search-volume URLs.

**The Solution:** The team explicitly avoided using standard <a href> links for individual sidebar filters. Instead, they implemented a **pop-up filter container**. Users select their options within a closed UI and click a dedicated "Search" button to transition to the results. This keeps millions of low-value, parameter-heavy URLs entirely hidden from Googlebot's discovery mechanisms.

C. Soft 404s (Empty Search Results)

While a clean site can return a hard HTTP 404 status code for permanently dead pages, dynamic marketplaces handle highly volatile inventory where a page may have zero listings today but regain them tomorrow.

**The Solution:** Serve a true HTTP 404 status code *only* for pages that consistently yield no search results. For pages experiencing temporary out-of-stock or zero-listing phases, programmatically **enrich the page content** by injecting results from surrounding suburbs. This satisfies user intent while preserving the URL structure under the principle: *"We build for the user, not just for the bot."*

3. Engineering a "GPS" to Guide the Crawler

A site's search bar is the primary way human users surface specific listings, but search crawlers cannot interact with search inputs to discover deeper pages. To ensure Googlebot naturally discovers the entire, clean site hierarchy, the team engineered a comprehensive architectural framework:

**Top Navigation:** Strictly reserved for directing equity to globally important, high-tier site sections.

**Breadcrumbs:** Used explicitly to display a clear, rigid vertical site hierarchy for search spiders.

**Comprehensive Footers:** Functions as an explicit, highly structured HTML link matrix that serves as a crawlable "GPS" for bots, allowing them to map out tier-down and sibling page relationships natively.

**XML Sitemaps:** Populated exclusively with core indexable target pages; however, Jing emphasized that these URLs must still be backed up by clean, crawlable frontend links to ensure Googlebot finds them naturally.

4. Why Server-Side Rendering (SSR) is Non-Negotiable

To support this massive structural cleanup, having an optimized technical foundation is paramount. Jing stated that SSR is absolutely mandatory for enterprise-scale crawl efficiency, drawing a sharp contrast with Client-Side Rendering (CSR):

|   |   |   |

| --- | --- | --- |

|   |   |   |

|   |   |   |

|   |   |   |

Jing contextualized this with a striking analogy: SSR gives an AI model a piece of **finished furniture**, whereas CSR hands it a **locked IKEA box with instructions** and assumes it has the capacity to build it.

Strategic Takeaways

Ultimately, maximizing crawl efficiency at scale successfully focused Realestate.com.au's index footprint—allowing them to block **315 million low-value URLs** from wasting bot attention, and consolidating equity into **52.8 million highly optimized, indexed target pages**.

Jing concluded by noting that modern technical SEO is no longer just a chase for standard search engine keyword rankings. Its true purpose is providing a thoroughly reliable, deeply authoritative, and instantly understandable source of clean data that search engines can easily parse today, and the AI search models can successfully digest tomorrow.