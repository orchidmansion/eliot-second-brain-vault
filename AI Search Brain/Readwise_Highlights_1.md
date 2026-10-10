# Readwise Highlights 1

- Tab 1

April 29, 2026 “https://www.theanalystacademy.com/designing-readability-effective-slides/”  (None, Quick Passages, pg None)

April 29, 2026 “Two versions in one document. The Quick Scan is a tiered 20-point field guide for any AI Search audit - each item includes the exact check to run and what a fail means for citation rate. The Deep Audit covers the same items with full context, tools, and fixes.

  This checklist is built around what actually drives citation rate in practice - including the checks most practitioners miss entirely.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “AI Search Technical Checklist

  [

  JC

  ](https://community.searchleaders.ai/u/1f2b9e14)

 [ Jeremy Cabra](https://community.searchleaders.ai/u/1f2b9e14)l

  Admin🏅Founding Member

 [ 5](https://community.searchleaders.ai/c/tools-resources/aeo-technical-checklist)d

  Founder of AI Search Leaders

  Two versions in one document. The Quick Scan is a tiered 20-point field guide for any AI Search audit - each item includes the exact check to run and what a fail means for citation rate. The Deep Audit covers the same items with full context, tools, and fixes.

  This checklist is built around what actually drives citation rate in practice - including the checks most practitioners miss entirely.

 ** Part 1: Quick Sca**n

 * *  *

  Run in under 5 minutes. Each item tells you exactly how to check it. Items marked [DEV] need developer involvement to fix.

  Tier 1: Critical Blockers

  If any of these fail, everything else is secondary. These prevent citation regardless of content quality.

 ** 1. Run "Describe [brand] in one paragraph" on Claude, ChatGPT, and Perplexity**. This is the most important check in the audit and most practitioners skip it entirely. Read each output carefully. Compare it to how the brand actually describes itself. The gap between those two things is your entire AI Search problem statement - and it tells you where to start. Failing means: You are optimizing without knowing what you are optimizing against.

 ** 2. AI crawlers not blocked in robots.txt - and verified in server logs**. Check: Go to [domain]/robots.txt. Search for GPTBot, PerplexityBot, anthropic-ai, Bytespider, CCBot, Meta-ExternalAgent, and Applebot-Extended. None should be followed by Disallow: /. Then verify in Cloudflare, server logs, or a crawler analytics tool that these bots are actually visiting - robots.txt compliance is not guaranteed. Failing means: The content cannot be indexed or cited by the platforms you are optimizing for, regardless of how good it is.

 ** 3. Key content renders without JavaScript**. [DEV] Check: Open a core content page. In Chrome, go to DevTools > Settigs > Disable JavaScript. Reload. Is the main body content - headings, paragraphs, the actual information - still visible without JS executing? Failing means: AI crawlers that do not run JavaScript see an empty shell. This is the most underdiagnosed AI Search blocker because it is invisible to human visitors.

 ** 4. Search the brand on Perplexity and check which domains appear as citations**. Check: Run 5 to 10 core category queries on Perplexity. Note which domains appear as cited sources in the responses. Is the brand's domain among them? Which competitor domains appear most frequently? Failing means: You now know exactly which sites LLMs trust in this category - and whether yours is one of them. This is your citation gap map.

 ** 5. Check if the brand's content appears in Common Crawl**. Check: Go to[ commoncrawl.or](http://commoncrawl.org/)g and use the index search to check whether the brand's domain appears in recent crawl data. Common Crawl is one of the primary training data sources for most LLMs. Failing means: If the domain is not in Common Crawl, it is likely absent or underrepresented in LLM training data entirely - which means no amount of on-page optimization will close the gap without increasing crawl accessibility.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “Tier 2: Citation Rate Drivers

  These are the factors that determine whether a site gets cited as a source, not just mentioned by brand name. Mention rate and citation rate are different metrics. Most brands optimize for mentions. Citations are what drive conversion.

 ** 6. The brand has at least one named framework or methodology**. Check: Does the brand own a specific, named concept - a framework, a model, a methodology - that is referenced by its name? Not just a product feature, but a named way of thinking about a problem. Why it matters: LLMs disproportionately cite named frameworks because they are unambiguous reference points. "The LLMO Content Pyramid" gets cited more than "how to structure content for LLM citation." If the brand does not have one, that is the highest-leverage content investment available.

 ** 7. Quotable paragraph audit on key pages**. Check: Read the first 200 words of each key page. Identify any sentence that could be extracted and cited verbatim without context - a specific claim, a clear definition, a data point with attribution. Count how many quotable sentences exist. Why it matters: LLMs pull short, self-contained statements. Pages written in flowing editorial prose are harder to cite than pages with clear, extractable claims. Most brand content fails this test badly.

 ** 8. Original data published and confirmed cited by others**. Check: Does the brand have at least one piece of content presenting data no one else has? Then check: is that data being cited by third-party publications and practitioners? Use Perplexity to search for the data point and see if it surfaces with the brand as the source. Why it matters: Citation rate for original data is 5 to 10 times higher than for content that aggregates others' research. Being the source is the only way to become a default reference in LLM responses.

 ** 9. Brand mentioned in Wikipedia articles about the category - not just having its own Wikipedia page**. Check: Search Wikipedia for the category (e.g. "AI search optimization," "answer engine optimization," the relevant product category). Is the brand mentioned within those articles? Why it matters: Wikipedia is one of the heaviest-weighted sources in LLM training. Being referenced within a Wikipedia article about your category is a stronger entity signal than having your own Wikipedia page. Most brands focus on getting their own page and miss this.

 ** 10. Google AI Overviews appearing for core category queries**. Check: Search 5 to 10 primary category queries in Google. Does an AI Overview appear? Is the brand referenced? Which competitor brands appear? Why it matters: Google's AI Overviews draw from similar authority signals to other LLMs. A brand that does not appear in AI Overviews is likely struggling across all AI search platforms. Appearing in AI Overviews is a strong leading indicator of broader LLM citation presence.

 ** 11. FAQ content sourced from real user queries, not internal guesses**. Check: Compare the FAQ questions on key pages against the People Also Ask results on Google for the same topic. Do they match? Or are the FAQs written from the brand's perspective rather than the user's? Why it matters: FAQs written to match how users actually ask questions get extracted more reliably. Internally-generated FAQs that do not match real query language are nearly invisible to LLMs.

 ** 12. Measure citation rate, not just mention rate**. Check: Run 20 queries across ChatGPT, Perplexity, Claude, and Gemini. For each response that mentions the brand, check whether the brand's URL is cited as a source (in Perplexity this is visible; in ChatGPT and Claude you may need to ask the LLM to cite sources). Calculate: of responses mentioning the brand, what percentage also cite the brand's URL? Why it matters: A brand can have 70% mention rate and 5% citation rate. That means LLMs know the brand exists but do not consider their content authoritative enough to reference directly. Mention rate feels good. Citation rate is what drives traffic and trust.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “Tier 3: Entity Authority

  These build the underlying entity model that LLMs use to understand and frame the brand. Slower to change but foundational.

 ** 13. Entity consistency audit across all external profiles**. Check: Compare the brand description across: Organization schema on homepage, LinkedIn company page, Crunchbase, G2 or Capterra (if applicable), Wikipedia (if it exists), and the About page. Are they describing the same company in the same terms? Note any contradictions in founding year, employee count, product description, or market positioning. Why it matters: LLMs build entity models by aggregating signals across sources. Conflicting descriptions create uncertainty. The LLM averages them into a muddier, less confident description of the brand - which reduces citation confidence.

 ** 14. Organization schema sameAs links to every official profile**. Check: Inspect Organization schema on homepage. Does sameAs include LinkedIn, Crunchbase, Wikipedia (if applicable), official social profiles, and any relevant industry directories? Are all URLs live and pointing to the correct pages? Why it matters: sameAs links are how LLMs confirm entity identity across sources. Missing links mean the LLM cannot fully consolidate its entity model. Every official profile not listed is a missed authority signal.

 ** 15. Author Person schema linked from content and connected to verifiable external profiles**. Check: Click the author byline on a key piece of content. Does it link to a bio page with Person schema? Does that schema include sameAs links to LinkedIn and any published work? Is the same author entity used consistently across the site? Why it matters: Content authored by identifiable, verifiable experts is given higher credibility weight. The connection between a piece of content and a credible human identity is a key AI Search signal that most brands implement partially or inconsistently.

 ** 16. dateModified in Article schema is actually updating when content is edited**. Check: Find a piece of content and note the dateModified in its Article schema (use View Source or Google's Rich Results Test). Ask: when was this page last meaningfully edited? Do the dates match? Many CMS implementations set dateModified once at publication and never update it automatically. Why it matters: Stale dateModified signals tell LLMs the content is old even if it was updated last week. This is a common and easy-to-miss implementation error.

 ** 17. Internal linking creates topical clusters around the brand's highest-priority AI Search pages**. Check: Go to the page the brand most wants to be cited for. How many internal links point to it from relevant pages? Is it the authoritative center of a topic cluster, or is it an orphan that receives no internal link support? Why it matters: LLMs infer topical authority partly from how a site organizes itself. A page that is heavily linked internally signals that the site considers it authoritative. An isolated page - even if the content is excellent - has weaker signals.

 ** 18. Heading structure mirrors how users actually ask questions**. Check: Extract all H2 and H3 headings from a key page. Search each one on Google and check if a similar phrase appears in People Also Ask results. If headings are internal labels ("Our Approach," "Key Considerations") rather than natural language queries or answer summaries, they are not doing AI Search work. Why it matters: LLMs use heading structure to match page sections to query intent. A heading that sounds like a user's question is more likely to be surfaced as an answer to that question.

 ** 19. Content structure passes the inverted pyramid test**. Check: Read only the first paragraph of a key page. After that one paragraph, can a reader extract a clear, complete answer to the page's primary question? Test this by showing the first paragraph to someone unfamiliar with the brand and asking what the page is about. Why it matters: LLMs prioritize extracting answers from content that leads with the answer. Pages that build context before reaching the point are less citable than pages that answer first and elaborate second.

 ** 20. The brand's position in LLM responses tracked over time - not just whether it appears, but where**. Check: In your monthly query testing, record not just whether the brand appears but its position in the response - first brand named, named alongside others, named late, or not named. Track this monthly. Is the brand moving earlier in responses over time? Why it matters: Being named fifth in a list of six tools is categorically different from being named first. Most AI Search measurement tracks presence. The practitioners who track position have a fundamentally more accurate picture of how AI search is shifting - and can catch momentum changes before they show up in traffic data.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “Part 2: Deep Audit

 * *  *

  Same 20 items with full context - what it is, why it matters, how to check it properly, and how to fix it.

  Tier 1: Critical Blockers1. Run "Describe [brand] in one paragraph" on Claude, ChatGPT, and Perplexity

 ** What it is**: A direct audit of how the three most-used AI search platforms currently understand and describe the brand - pulled straight from the source.

 ** Why it matters for AI Search**: Most AI Search audits start with robots.txt and schema. This one starts by reading what the LLM actually thinks, because that is the ground truth you are trying to shift. Every other check in this audit is in service of changing this output. If you do not run this check first, you are optimizing without knowing what you are optimizing against.

  The outputs often reveal things brands do not expect. Common findings: the LLM describes a brand in terms of a product they launched five years ago and have since pivoted from. The LLM associates the brand with a competitor more prominent in its training data. The LLM knows the brand name but has thin knowledge of what it actually does. The LLM describes the brand's positioning accurately but not in the language the brand uses - which means the brand is winning in AI search but not getting credit for it in client conversations.

 ** How to check**: Open a fresh conversation in each platform. Paste: "Describe [brand name] in one paragraph, based on what you know from your training data. Be honest about what you know and do not know." Compare the three outputs. Note where they agree, where they diverge, and where they contradict the brand's actual positioning. Use the diagnosis categories from the Brand Intelligence Audit to categorize the problem.

 ** How to fix**: This check is diagnostic, not directly fixable. The fixes come from everything else in this checklist. But the output of this check should become the brief for all AI Search content work - specifically, the gap between the current LLM description and the desired description is what needs to close.

  2. AI crawlers not blocked - and verified in server logs

 ** What it is**: A full audit of which AI crawlers are allowed to index the site, verified both in robots.txt and in actual server log data.

 ** Why it matters for AI Search**: robots.txt compliance is not guaranteed. Some crawlers respect it; others do not. More importantly, many brands have wildcard disallow rules (User-agent: * / Disallow: /) that block AI crawlers by default, then add selective allow rules for Googlebot - but never explicitly allow AI crawlers. The result is a site that appears accessible in robots.txt review but blocks every major AI crawler in practice.

  The full list of AI crawlers to allow (as of 2025): GPTBot (OpenAI), PerplexityBot (Perplexity), anthropic-ai (Anthropic/Claude), Google-Extended (Gemini), Bytespider (ByteDance), CCBot (Common Crawl), Meta-ExternalAgent (Meta AI), Applebot-Extended (Apple), Diffbot, and Amazonbot. Most checklists only mention GPTBot. That leaves most of the major platforms unaddressed.

 ** How to check**: Step 1 - Go to [domain]/robots.txt. For each crawler in the list above, check: is there an explicit allow rule? Is there any disallow rule that would catch it? Look for wildcard User-agent: * rules with broad disallow paths.

  Step 2 - Verify actual crawl activity in server logs or Cloudflare analytics. Filter by user agent strings for each major AI crawler. Are they making requests? How frequently? Which pages are they hitting?

 ** How to fix**: Add explicit allow rules for each AI crawler you want to permit. Place them above any wildcard rules to ensure they take precedence. If the team has concerns about content scraping, consider allowing crawlers selectively by path rather than blanket blocking. Review this quarterly - AI crawler user agent strings change as platforms update.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “3. Key content renders without JavaScript

 ** What it is**: A test to confirm that the primary body content of key pages is present in the initial HTML response, before any JavaScript executes.

 ** Why it matters for AI Search**: Single-page application frameworks (React, Vue, Next.js without SSR, Angular) often deliver a minimal HTML shell on the first request and then populate content via JavaScript. AI crawlers that do not execute JavaScript - including some configurations of GPTBot and most secondary crawlers - receive only the shell. The crawl shows pages as blank or near-blank, even though human visitors see full content.

  This is the most underdiagnosed AI Search technical blocker. It is invisible to anyone auditing the site as a human visitor. It requires deliberate testing to catch.

 ** How to check**: Open a key content page in Chrome. Open DevTools (Cmd+Option+I or F12). Click the gear icon for Settings. Under Preferences, check "Disable JavaScript." Close Settings. Reload the page. The content visible in this state is what most AI crawlers see. Repeat for 5 to 10 key pages. Pay particular attention to: the main body text, headings, and any FAQs or structured content.

  Also: use curl to fetch the page and inspect the raw HTML. Run: curl -s [URL] | grep -c "[a-z]" to get a rough word count of the initial HTML. Compare to the visible word count on the page. A large discrepancy indicates JavaScript-dependent content.

 ** How to fix**: Implement server-side rendering (SSR) or static site generation (SSG) for content pages. The fix ensures the full content is included in the initial HTML response. Next.js (React), Nuxt.js (Vue), and SvelteKit all support SSR natively. This is a developer-level change that may require architectural decisions about the site. Prioritize content pages - blog, resources, product documentation - over app or dashboard pages.

  4. Search the brand on Perplexity and map which domains get cited

 ** What it is**: A live audit of which sources Perplexity cites when answering questions in the brand's category - and whether the brand's domain is among them.

 ** Why it matters for AI Search**: Perplexity shows its citations visibly, which makes it the most transparent window into which sites LLMs actually trust in a given category. The domains that appear as Perplexity citations are the sites LLMs have established as authoritative references. If the brand's domain is not appearing there, the problem is not visibility - it is authority.

  This check also reveals the competitive citation landscape: which competitor domains are being cited most? What types of content are getting cited (blog posts, research reports, product pages, press coverage)? This tells you exactly what kind of content you need to produce to enter the citation set.

 ** How to check**: Open Perplexity. Run 10 queries that cover: 2 problem-aware queries, 2 category queries, 2 comparison queries, 2 expert recommendation queries, and 2 queries that name the brand directly. For each response, note: which domains appear as citations, what type of content they are, and whether the brand's domain appears. Build a simple table: Query | Citations | Brand domain cited (Y/N).

 ** How to fix**: This check is diagnostic. The output tells you which content types to prioritize. If competitor blogs are being cited, build a blog with deeper content. If research reports are being cited, produce original research. If press coverage is driving citations, prioritize PR in the publications appearing. The goal is to match the content profile of the sites already in the citation set.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “5. Check if the brand's content appears in Common Crawl

 ** What it is**: A check to verify whether the brand's domain appears in Common Crawl - one of the largest open-source web crawl datasets and a primary training data source for most major LLMs.

 ** Why it matters for AI Search**: If a brand's content is not in Common Crawl, it is likely absent or significantly underrepresented in LLM training data. This explains cases where a brand has good content, no crawler blocks, and strong on-page signals - but still does not appear in LLM responses. The content simply was not in the data the model was trained on.

  Common Crawl is not a crawl you can directly influence in real time, but checking for presence gives important diagnostic signal, particularly for newer domains or domains that have recently launched significant content.

 ** How to check**: Go to[ index.commoncrawl.org/collinfo.jso](http://index.commoncrawl.org/collinfo.json)n to find recent crawl indices. Use the Common Crawl Index Server to query a specific domain:[ http://index.commoncrawl.org/CC-MAIN-[CRAWL-ID]-index?url=[domain]&output=jso](http://index.commoncrawl.org/CC-MAIN-%5BCRAWL-ID%5D-index?url=%5Bdomain%5D&output=json)n. Check the most recent 3 to 4 crawls. Note how many pages from the domain appear and which pages specifically.

  Alternatively, use third-party tools like CDX Toolkit or the Common Crawl search interface to check domain presence without direct API queries.

 ** How to fix**: Ensure the domain is crawlable (no crawler blocks, no JS dependency issues, fast page speed, valid sitemap submitted). Common Crawl runs periodic large-scale crawls - improving crawlability increases the likelihood of inclusion in the next crawl cycle. For new domains or domains with recent major content additions, this lag between publishing and LLM training data inclusion is expected. The fix is patience plus crawlability.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “Tier 2: Citation Rate Drivers6. The brand has at least one named framework or methodology

 ** What it is**: A proprietary, named concept - a framework, a model, a methodology, a named approach - that is attributed to the brand and referenced by that specific name.

 ** Why it matters for AI Search**: LLMs disproportionately cite named frameworks because they are unambiguous reference points. "The Inbound Marketing methodology" gets cited as attributed to HubSpot. "The Jobs to be Done framework" gets cited as attributed to Clayton Christensen. "The Flywheel" gets cited as attributed to Amazon. Generic content about "how to do content marketing" does not accumulate citations in the same way.

  A named framework is a high leverage AI Search content investment for most brands, because it creates a citation anchor that is uniquely associated with the brand by name. Every time an LLM mentions the framework, it mentions the brand.

 ** How to check**: Ask: does the brand have any named frameworks, models, or methodologies that practitioners in the category use and reference by name? Search the brand name plus "framework" or "methodology" on Perplexity. Does anything come up? Search the framework name on its own - does the brand appear as the originator?

 ** How to fix**: Identify a genuine insight the brand has that is not yet named. It should be: non-obvious, specific to the brand's area of expertise, and useful enough that practitioners would want to reference it. Name it. Write a definitive piece of content introducing and explaining it. Distribute it aggressively. The goal is for practitioners to start referencing it by name - which then enters LLM training data as an attributed concept.

  7. Quotable paragraph audit

 ** What it is**: An assessment of whether key pages contain self-contained, extractable sentences that an LLM can cite without surrounding context.

 ** Why it matters for AI Search**: LLMs pull short, specific statements when building their responses. "According to [Brand], the primary reason AI Search fails is that brands optimize for mentions rather than citations" is citable. A paragraph that spends 80 words establishing context before making a point is not. Most brand content fails this test because it is written for human readers who have context - not for LLMs that need self-contained claims.

  The specific pattern to look for: does each key page have at least 3 sentences in the first 300 words that could be extracted and cited in isolation, without any surrounding context?

 ** How to check**: Read the first 300 words of each key page. For each sentence, ask: if this sentence appeared alone in an LLM response attributed to [brand], would it make complete sense? Would it be useful? Would it be credible? Count how many sentences pass. A page with 0 to 1 quotable sentences in the opening has a serious AI Search problem regardless of overall content quality.

 ** How to fix**: Rewrite key pages to front-load quotable claims. Useful formats: specific statistics ("Brands with original research are cited X times more often than brands that aggregate data from others"), named definitions ("[Term] is [clear, specific definition in one sentence]"), contrarian insights ("[Common belief] is wrong - here is what the data actually shows"), and named frameworks with specific explanations. Every key page should have at least 3 immediately citable sentences in the opening.

  8. Original data published and confirmed cited by others

 ** What it is**: Original research or proprietary data that the brand has published AND that has been cited by third-party publications, practitioners, or other sites.

 ** Why it matters for AI Search**: Publishing original data is necessary but not sufficient. The data needs to be cited by others to enter LLM training data as an attributed fact. A survey published on a brand's blog that no one links to or references has limited AI Search value. The same survey, cited in ten industry publications, becomes a persistent reference point in LLM responses.

 ** How to check**: Step 1 - Does the brand have any original data published? Step 2 - Search for specific data points from that research on Perplexity. Is the brand cited as the source? Step 3 - Check backlinks to the research piece using Ahrefs or similar. How many external sites link to it? What publications? Step 4 - Run the data point as a query in ChatGPT. Does the model know the statistic? Does it attribute it to the brand?

 ** How to fix**: If no original data exists, commission a survey. If data exists but is not cited, the distribution strategy failed - re-launch the research as a PR asset, pitch it to relevant publications, send it to practitioners who might reference it, and brief it to relevant journalists. The goal is to get the specific data point attributed to the brand in at least 10 to 15 external publications. That is the threshold at which it starts appearing reliably in LLM training data.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “9. Brand mentioned within Wikipedia articles about the category

 ** What it is**: A check for whether the brand appears as a reference within existing Wikipedia articles covering the relevant category, industry, or topic area.

 ** Why it matters for AI Search**: Most people think of Wikipedia AI Search as "does the brand have its own Wikipedia page." The more important question is: is the brand mentioned within the Wikipedia articles that LLMs draw from when understanding the category? Wikipedia is one of the most heavily weighted sources in LLM training. A brand mentioned in the Wikipedia article on "answer engine optimization" or "search engine marketing" is signaling category relevance to LLMs in a way that the brand's own website cannot replicate.

 ** How to check**: Search Wikipedia for the primary category, adjacent categories, and any named methodologies the brand is associated with. Open each relevant article. Use Ctrl+F to search for the brand name. Is it there? How is it described? Is the description accurate?

 ** How to fix**: If the brand is not mentioned where it reasonably should be, contribute to the Wikipedia article. Wikipedia contributions must follow neutral point of view guidelines - adding the brand as an example where it genuinely belongs is appropriate. Adding promotional language is not. If the brand's absence from a Wikipedia article is due to low notability in that category, the fix is building more third-party coverage until the notability threshold is met.

  10. Google AI Overviews appearing for core category queries

 ** What it is**: A check for whether the brand appears in Google's AI Overviews (formerly Search Generative Experience) for primary category and comparison queries.

 ** Why it matters for AI Search**: Google AI Overviews draw from similar authority signals to other LLMs - E-E-A-T, structured data, cited third-party content, and original expertise. A brand that appears in AI Overviews is demonstrating the same signals that drive citation in ChatGPT, Perplexity, and Claude. Conversely, a brand absent from AI Overviews will almost certainly be absent or weak across other AI search platforms. This makes AI Overviews a fast, accessible proxy for broader AI Search health.

 ** How to check**: Search 10 category and comparison queries in Google (use a logged-out browser to avoid personalization). Record: does an AI Overview appear? Is the brand named in it? Which competitor brands appear? Which sources are cited in the "Learn more" section? Do this monthly - AI Overview appearance is volatile and tracking changes tells you whether your AI Search signals are improving.

 ** How to fix**: AI Overview appearance is driven by the same signals as all other AI Search: authoritative content, strong entity signals, cited sources, and structured data. There is no specific Google AI Overviews optimization separate from general AI Search. If the brand is not appearing, prioritize the Tier 1 and Tier 2 items in this checklist.

  11. FAQ content sourced from real user queries

 ** What it is**: An audit of whether FAQ content on key pages uses the same language real users use when asking questions - or whether it is written from the brand's internal perspective.

 ** Why it matters for AI Search**: LLMs match FAQ content to queries based on language similarity. An FAQ question written as "What are the key differentiators of our platform?" will not match a user query of "how is this different from competitors?" An FAQ question written as "How does [brand] compare to [competitor]?" will. The source of FAQ questions matters as much as the format.

 ** How to check**: Copy the FAQ questions from a key page. Search the same page topic on Google and check the People Also Ask section. Do the FAQ questions match the PAA questions? Run the FAQ questions as queries in Perplexity - do they surface as natural queries? Compare FAQ language to actual customer support tickets or sales call recordings if accessible.

 ** How to fix**: Replace internally-generated FAQ questions with questions sourced from: People Also Ask results on Google, actual customer support questions, sales call transcripts, Reddit threads in relevant subreddits, and Quora questions in the relevant category. The questions should sound like something a real person would type or say - not something a product manager would write.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “12. Measure citation rate, not just mention rate

 ** What it is**: A monthly measurement of what percentage of LLM responses that mention the brand also cite the brand's URL as a source - rather than just tracking whether the brand name appears in responses.

 ** Why it matters for AI Search**: Mention rate and citation rate are different metrics that tell different stories. A brand with 70% mention rate and 8% citation rate is well-known but not trusted as a source - LLMs know the brand exists but do not consider its content authoritative enough to reference directly. A brand with 40% mention rate and 35% citation rate has a content trust problem (not enough awareness) but strong source authority for the audience it does reach. The distinction shapes the entire AI Search strategy.

  Most AI Search measurement focuses on mention rate because it is easy to track. Citation rate requires checking whether URLs appear in responses - which is visible in Perplexity (citations are shown) and can be tested in ChatGPT by asking the model to cite sources.

 ** How to check**: In your monthly query set, for every response that mentions the brand, check: does the response also include a URL from the brand's domain as a cited source? In Perplexity, this is visible in the sidebar. In ChatGPT, add "Please cite your sources with URLs" to each query. In Claude, sources are not always shown but can be requested. Calculate: (responses citing brand URL) divided by (responses mentioning brand name) = citation rate.

 ** How to fix**: Citation rate improves through: original data that has been distributed and cited by third parties, named frameworks referenced by practitioners, content that appears in authoritative publications (which then becomes a training data signal), and FAQ schema that enables direct content extraction. If mention rate is high and citation rate is low, the content quality and authority signals are the bottleneck - not awareness.”  (AI Search Leaders, AI Search Technical Checklist)

April 29, 2026 “Tier 3: Entity Authority13. Entity consistency audit across all external profiles

 ** What it is**: A comparison of how the brand describes itself across all major external profiles to identify conflicting signals that create LLM uncertainty.

 ** How to check**: Pull the brand description from: Organization schema on homepage, LinkedIn company page About section, Crunchbase overview, G2 or Capterra profile, Wikipedia article if it exists, and the About page. Note any differences in: founding year, employee count range, core product description, target market, and geographic focus.

 ** How to fix**: Standardize descriptions across all profiles. Agree on the canonical one-paragraph brand description and update every profile to use it (or a close version). Ensure founding year, employee count, and other facts are consistent. Assign someone to audit external profiles quarterly.

  14. Organization schema sameAs links to every official profile

 ** What it is**: The sameAs property in Organization schema linking the brand entity to all official external profiles, enabling LLMs to consolidate entity identity across sources.

 ** How to check**: Inspect Organization schema on the homepage (View Source or Rich Results Test). Does sameAs include: LinkedIn, Crunchbase, Wikipedia (if applicable), official social profiles, and industry-specific directories relevant to the category? Are all URLs live?

 ** How to fix**: Add all official profiles to the sameAs array. Verify every URL is live and points to the correct page. Review this when new official profiles are created. Remove any URLs that redirect or return errors.

  15. Author Person schema connected to verifiable external profiles

 ** What it is**: Structured data connecting content to identifiable authors with verifiable credentials, implemented consistently across all content pages.

 ** How to check**: Click the author byline on a key content page. Does it link to a bio page? Does that bio page have Person schema with a sameAs array linking to LinkedIn and other published work? Is the same Person entity referenced consistently across all content from that author?

 ** How to fix**: Create bio pages for every content contributor with Person schema. Include sameAs links to LinkedIn at minimum, plus any academic profiles, industry publications, or other published work. Ensure the Article schema on each content page links to the correct Person entity rather than using a plain text author name.

  16. dateModified in Article schema is actually updating when content is edited

 ** What it is**: A verification that the dateModified field in Article schema reflects the actual date of the last substantive content edit - not the original publication date or a static value set at launch.

 ** How to check**: Identify a piece of content that was recently edited. Use View Source or Rich Results Test to check the dateModified field. Does it match the actual edit date? Then check a piece of content that has not been edited in 12 months - is dateModified still stuck at the original publication date?

 ** How to fix**: Configure the CMS to automatically update dateModified whenever content is saved with substantive changes. Define what counts as a substantive change (updated statistics, new sections, revised conclusions - not typo fixes or formatting). Test the implementation after making a content edit to confirm the date updates.

  17. Internal linking creates topical clusters around highest-priority AI Search pages

 ** What it is**: An assessment of whether the site's internal linking structure reinforces the authority of the pages most important for AI Search.

 ** How to check**: Identify the 5 pages most important for AI Search (the pages you most want cited). For each page: how many internal links point to it from relevant pages? Are those linking pages topically related? Or is the key page effectively an orphan?

 ** How to fix**: Build topical clusters around key pages. Every related piece of content on the site should link to the central authoritative page on that topic. Create a hub-and-spoke structure where the most important pages sit at the hub with multiple relevant spokes linking in. Use descriptive anchor text that reflects the topic of the destination page.

  18. Heading structure mirrors how users actually ask questions

 ** What it is**: An audit of whether H2 and H3 headings on content pages use natural language that matches real user queries.

 ** How to check**: Extract all H2 and H3 headings from a key page. Search each heading as a query on Google. Does a similar phrase appear in People Also Ask? Does the heading read like a natural question or answer? Or like an internal section label?

 ** How to fix**: Rewrite headings using one of two patterns: question format matching real queries ("How do you measure AI search visibility?") or direct answer summaries that use the vocabulary of the query ("Measuring AI search visibility: the three metrics that matter"). Avoid: "Overview," "Background," "Introduction," "Key Considerations," and other internal labels that carry no query signal.

  19. Content structure passes the inverted pyramid test

 ** What it is**: A verification that the most important information on each key page appears in the first paragraph, rather than building toward it through context-setting or background.

 ** How to check**: Show only the first paragraph of a key page to someone unfamiliar with the brand or topic. Ask them: what is this page about? What is the main answer or point? If they cannot answer confidently from the first paragraph alone, the page fails.

 ** How to fix**: Rewrite page openings using the inverted pyramid structure. The core answer goes first. Supporting evidence, context, and nuance follow. This applies to articles, guides, comparison pages, and product pages. The only exception is content structured as a narrative - but even then, an answer-first summary or key takeaway at the top improves AI Search performance.

  20. Track brand position in LLM responses over time - not just presence

 ** What it is**: A monthly measurement of where in LLM responses the brand appears - first, alongside peers, or late - rather than simply whether it appears.

 ** How to check**: In monthly query testing, for every response where the brand appears, record its position: first brand named, named alongside others in the first sentence, named in a list, named late in the response after others, or named only in response to a direct brand query. Track this data in a spreadsheet month over month.

 ** How to fix**: Position in response is a lagging indicator of entity authority and content quality. Improving it requires the full stack of AI Search work - stronger entity signals, more cited content, named frameworks, and original data. But tracking it gives you a more sensitive signal than mention rate alone. Brands often see position improving before they see mention rate improving, which means position tracking gives you earlier evidence that the AI Search strategy is working.”  (AI Search Leaders, AI Search Technical Checklist)

May 17, 2026 “• 0.50 onions • 5 pieces green onion • 4 oz bean sprouts 1 tbsp dark soy sauce 1 tbsp light soy sauce Cantonese Fried Noodles ( gulled m • 1 tbsp oyster sauce 2 tsp sugar • 1 tbsp water • 1 tsp sesame oil ( to taste )

  • 3 tbsp corn oil Step 1 - Steam noodles, drain, cool↑ Jump to details Here's a quick run-down of the types of HK-style noodles you can buy:

  • fresh, unsteamed • fresh, steamed ⚫ dried In the video, we demonstrate how to cook with fresh, unsteamed noodles (which is my dad's preference). This takes a little bit of extra work but is worth it.

  Here's what you do:

  • Place your steamer rack in a wok on high heat. Pour enough water so that the top of the rack isn't submerged, and start boiling water.

  • Take the rack out, separate and lay out noodles (12 oz) on top of the rack.

  • Once boiling, set the steamer rack + noodles back in the wok and cover for 10 minutes. Leave the stove on high heat.

  • If you're using a steamer rack without holes (i.e. steaming on a plate where the steam can't easily access the bottom, steam for 2-3 extra minutes.)

  • Once the 10 minutes is up, quickly dump the noodles in the water for 15-30 seconds.

  • Drain noodles through a colander, and spend about 1-2 minutes fluffing and separating the noodles with a chopstick.

  • Let it cool for 3-5 minutes.

  ttps://www.printfriendly.com/p/g/NWC3Lq 2/5/21, 5:24 pm Page”  (None, Quick Passages, pg None)

    **Note:** Cantonese fried noodles

May 17, 2026 “If you're using fresh, steamed noodles, you can skip the steaming step.

  Instead dunk the noodles in boiling water for about 2 minutes before draining.

  If you're using dried noodles, it's somewhat similar to cooking instant ramen. Cook according to the package's instructions, erring on the more al-dente side, and rinse with cold water afterwards to stop the cooking.

  Step 2-Chop vegetables Jump to details We'll wash and chop our vegetables:

  onion (5 pieces) - cut into about 1.5 inch pieces. Separate green the roots and the Shoots, as we'll be cooking the roots first.

  onion (0.50) - cut in half, and then julienne (see video for example)

  ⚫ bean sprouts (4 oz) you can leave these as is. Some traditional restaurants will remove the beans and the tips, which is A LOT of work.. but feel free.

  Step 3 - Create sauce↑ Jump to details Mix dark soy sauce (1 tbsp), light soy sauce (1 tbsp), oyster sauce (1 tbsp), sugar (2 tsp), water (1 tbsp) in a bowl until the sugar dissolves.

  We'll be adding the sesame oil later.

  Step 4 - Heat wok, start cooking↑ Jump to details We'll start by heating our wok to around 350-400°F (176-204°C).

  Depending on your stove, this should take around 2-3 minutes.

  AFTER the wok is hot, we'll add corn oil (0.99 tbsp) and heat that to 350-400°F. As a visual cue, it should be "shimmering" - rippling, but not smoking. If it's started smoking, the wok is too hot.

  Then, we'll start cooking our green onion roots and onions for right around 1 minute, and set them on a plate for later.

  Heat the wok again and add more corn oil (0.99 tbsp). Once the oil is shimmering, add the noodles.

  We want to be really gentle with the noodles. DO NOT flip them yet, and only occasionally move the noodles around. Let the bottom get nice and crispy for about 3 minutes.

  https://www.printfriendly.com/p/g/NWC3Lq 2/5/21”  (None, Quick Passages, pg None)

May 17, 2026 “heat inside to help them cook more evenly and quickly.

  • Let the bean sprouts cook underneath the noodles for 30-45 seconds.

  Add the green onions (everything, the cooked roots + raw shoots) and onions, and cook for about 1-2 minutes. Continue separating the noodles with chopsticks and a spatula.

  Pour in the sauce mix, and”  (None, Quick Passages, pg None)
