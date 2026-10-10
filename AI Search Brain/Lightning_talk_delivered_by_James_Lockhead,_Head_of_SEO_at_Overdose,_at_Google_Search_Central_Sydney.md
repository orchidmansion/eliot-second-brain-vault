# Lightning talk delivered by James Lockhead, Head of SEO at Overdose, at Google Search Central Sydney 2026.docx

Here is a detailed summary of the lightning talk delivered by James Lockhead, Head of SEO at Overdose, at Google Search Central Sydney. His presentation outlines a highly actionable, template-level strategy for optimizing internal linking structures across large-scale Shopify websites.

The Core Foundation: A Backend Navigation Hierarchy

The entire strategy relies on building a robust, tiered navigation structure directly within the Shopify backend.

**Separate from the Mega Menu:** This backend navigation is explicitly decoupled from the user-facing mega menu.

**Tiered Architecture:** It is designed to map out a logical category architecture across the entire site using a tiered methodology (e.g., Tier 1: Category $\rightarrow$ Tier 2: Sub-collection $\rightarrow$ Tier 3: Sub-sub-collection)  *(visualized in Slide IMG_9438.jpg)*.

**Efficient Scalability:** To prevent this from becoming an overwhelming manual task, SEOs can use the app **Matrixify** to bulk upload the entire hierarchy via a CSV file, reducing the setup time to just 1 or 2 hours.

Step 1: Optimize Collection Pages with Sub-category Links

Once the backend navigation framework is live, developers can use it to dynamically generate contextual internal links on collection templates.

**Above-the-Fold Placement:** The template should output collection-to-collection links high up on the page, specifically above the main product grid or above the fold  *(visualized in Slide IMG_9439.jpg)*.

**Automatic Child-Tier Output:** The system leverages the backend navigation hierarchy to automatically display the sub-categories sitting directly beneath the current category (e.g., navigating to "Dresses" automatically triggers tile links for "Maxi Dresses", "Midi Dresses", etc.).

**Proven Conversion Lift:** An internal split-test conducted by Overdose on a New Zealand client showed that users who clicked these sub-category tile links were roughly 40% more likely to convert.

Step 2: Ensure a Server-Side Rendered (SSR) Product Grid

For internal links within a product grid to pass value to search engines, the product listings must be hardcoded into the page's HTML from the server.

**The Third-Party Filter Flaw:** Many enterprise e-commerce sites use third-party search and filtering apps that rely entirely on client-side JavaScript, rendering a blank grid to search engine crawlers  *(visualized in Slide IMG_9440.jpg)*. James specifically noted that the app *Athos* frequently presents technical SEO hurdles because it lacks an SSR workaround.

**SEO-Friendly Alternatives:** Smaller websites should rely on Shopify’s native, out-of-the-box filtering. For larger sites requiring advanced applications, **Algolia** or **Nosto** are recommended as SEO-compliant, SSR-supporting options.

Step 3: Fix Broken Product Breadcrumbs via Canonical URLs

One of Shopify's most pervasive technical SEO issues is its default tendency to link to non-canonical product URLs from collection pages (e.g., paths containing */collections/collection-name/products/product-name*)  *(visualized in Slide IMG_9441.jpg)*.

**The Breadcrumb Dilemma:** Modifying the store code to point collection grids directly to clean, canonical product URLs (*/products/product-name*) is mandatory for SEO, but doing so inherently breaks Shopify's native product breadcrumb tracking.

**The Nav Piggyback Solution:** By leveraging the custom backend navigation hierarchy created in the initial phase, developers can write a loop that accurately reconstructs an optimized, full-tier breadcrumb path on the canonical product template (e.g., Home $\rightarrow$ Dresses $\rightarrow$ Maxi Dresses $\rightarrow$ White Maxi Dresses)  *(visualized in Slide IMG_9442.jpg)*.

**SEM and Feed Integration:** This clean breadcrumb path can be fed directly into Google Merchant Center as the *product_type* attribute, providing a structured, highly optimized signal for Paid Search teams at scale.

Step 4: Surface Related Categories on Product Pages (PDPs)

While previous steps push crawl equity downwards to products, it is equally important to pass link authority back up to high-value collection pages.

**Contextual Cross-Linking:** By tapping back into the clean navigation list, a product detail template can dynamically display links to every collection that the product is a member of  *(visualized in Slide IMG_9443.jpg)*.

**Bypassing Historical "URL Mess":** This programmatic approach ensures the site links exclusively to primary SEO collection pages, completely bypassing old, low-value promotional URLs created by marketing or email teams over time.

**Massive Scale Impact:** For a store managing over 10,000 SKUs, this instantly builds thousands of contextual, automated internal links pointing directly back to core target landing pages.

Summary of the Workflow Impact

Ultimately, this framework allows an SEO professional to execute about half a day's worth of preparation and mapping independently before passing clear requirements to engineering. Once the developers implement the template logic, a large-scale e-commerce site will automatically maintain an optimized internal link ecosystem across thousands of pages.