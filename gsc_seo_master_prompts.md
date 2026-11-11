# Google Search Console SEO Opportunity & Page Optimisation Workflow

This workflow uses Google Search Console (GSC) query data to uncover
customer questions, identify content and search-intent gaps, and improve
existing website pages using genuine business information.

It contains two prompts:

1.  **Prompt 1: RE2 Regex Generator** -- creates a GSC-compatible regex
    to filter informational and question-based queries.
2.  **Prompt 2: SEO Master Analysis & Page Optimisation** -- analyses
    the exported query data, gathers business-specific information from
    the user, and produces evidence-led recommendations and an improved
    page structure.

------------------------------------------------------------------------

## How to use this workflow

1.  Open ChatGPT and run Prompt 1.
2.  Copy the generated regex into Google Search Console: **Performance →
    Search results → Queries → Add filter → Query → Custom (regex)**.
3.  Review the matching queries and export the data as CSV or Excel.
4.  Start a new ChatGPT conversation, upload the export, and run Prompt
    2.
5.  Answer the business-context questions Prompt 2 asks. The questions
    should be based on the actual queries and opportunities found in the
    uploaded data.
6.  Review the recommendations and provide any further business facts or
    source material requested before asking for revised page content.

**Important:** GSC query data shows what people searched for and how the
website performed. It does not, by itself, prove what a business offers,
its processes, credentials, service areas, guarantees, experience or
unique selling points. Those facts must come from the business owner or
reliable material supplied by the user.

------------------------------------------------------------------------

# Prompt 1: Google Search Console RE2 Regex Generator

Copy and use the prompt below:

> Act as an expert SEO analyst who understands Google Search Console
> regex filters and the RE2 regex engine.
>
> Generate a Google Search Console-compatible RE2 regular expression
> that filters informational, question-based search queries. Include
> common question words and variations, such as:
>
> -   who
> -   what
> -   why
> -   when
> -   where
> -   how
> -   which
> -   can
> -   does
> -   do
> -   is
> -   are
> -   should
> -   could
> -   would
> -   will
> -   have
> -   has
>
> Include sensible variations and phrases that indicate a question or an
> informational search intent. Make the expression suitable for the
> **Queries → Custom (regex)** filter in Google Search Console.
>
> Requirements:
>
> 1.  Use RE2-compatible syntax only. Do not use unsupported features
>     such as lookahead, lookbehind or backreferences.
> 2.  Make the expression case-insensitive where supported by Google
>     Search Console.
> 3.  Avoid matching every query simply because it contains a short
>     character sequence inside an unrelated word. Prefer question terms
>     at the beginning of a query or as separate words where practical.
> 4.  Include a brief explanation of what the regex is designed to match
>     and any limitations.
> 5.  Return the final regex in a single copyable code block.
> 6.  If useful, provide a second, broader version that captures more
>     conversational and long-tail question queries, clearly labelled as
>     broader.
>
> Do not claim that the regex captures every informational query. Search
> intent cannot always be identified from wording alone.

------------------------------------------------------------------------

# Prompt 2: SEO Master Prompt -- Search Intent, Content Gaps, E-E-A-T and Page Optimisation

Copy the complete prompt below into a new ChatGPT conversation after
uploading the GSC export.

> ## Role
>
> Act as a senior SEO strategist, search-intent analyst, content
> strategist and website optimisation consultant. Your task is to
> analyse the uploaded Google Search Console data and help improve the
> website's existing pages using evidence from the search data and
> accurate information supplied by the business.
>
> Your goal is not to produce generic SEO copy or automatically add
> keywords to a page. Your goal is to understand what potential
> customers are asking, what the website currently satisfies or misses,
> what the business can genuinely deliver, and how the relevant page
> should be improved.
>
> ## Core objectives
>
> Analyse the uploaded data to identify:
>
> 1.  **Search intent gaps:** Questions and needs that the current
>     landing pages may not answer adequately.
> 2.  **Content gaps:** Important subtopics, explanations, comparisons,
>     processes or supporting details missing from relevant pages.
> 3.  **Keyword and query opportunities:** Relevant queries with
>     impressions, clicks, CTR and average-position opportunities.
> 4.  **Competitor and SERP gaps:** Topics, formats and useful
>     information that competing pages appear to cover better, where
>     competitor or live search evidence is available.
> 5.  **Customer concerns:** Questions that indicate uncertainty,
>     objections, risks, pricing concerns, eligibility, suitability,
>     timing or the need for reassurance.
> 6.  **Topical coverage:** Whether the page gives a clear and
>     sufficiently complete explanation of the subject without
>     unnecessary repetition.
> 7.  **E-E-A-T and entity signals:** Opportunities to demonstrate
>     first-hand experience, expertise, authoritativeness and
>     trustworthiness, and to describe the real business, its people,
>     services, processes, credentials and relevant entities accurately.
> 8.  **Page structure:** Improvements to the existing page's headings,
>     sections, FAQs, supporting content and calls to action.
> 9.  **Internal linking:** Relevant pages on the supplied website that
>     should link to the target page, and relevant pages the target page
>     should link to.
>
> ## Stage 1: Understand and validate the uploaded data
>
> First inspect the uploaded file. Identify the available columns, date
> range, query data, landing-page data (if present), clicks,
> impressions, CTR and average position.
>
> If a field is not present, state that it is unavailable. Do not invent
> metrics or assume that the export contains page-level information when
> it does not.
>
> Clean and group the queries into meaningful themes and customer-intent
> categories. Separate, where possible:
>
> -   Informational questions
> -   Commercial investigation
> -   Transactional or service-seeking queries
> -   Navigational or brand queries
> -   Local or location-based queries
> -   Irrelevant or ambiguous queries
>
> Identify duplicate, closely related and differently worded questions.
> Preserve the original query wording when it provides useful customer
> insight.
>
> Do not assume that every question belongs on the same page. Group
> questions by topic, intent, service and likely destination page.
>
> ## Stage 2: Identify the pages and opportunities
>
> If landing-page data is included, map relevant queries to their
> associated URLs. Identify:
>
> -   Pages receiving impressions for relevant questions
> -   Pages with high impressions but comparatively low CTR
> -   Queries ranking around positions 4--20 that may have realistic
>     improvement potential
> -   Pages attracting queries that do not closely match their apparent
>     purpose
> -   Relevant queries for which no suitable page is evident in the
>     supplied data
> -   Potential keyword cannibalisation or overlapping page intent,
>     where the evidence supports it
>
> Treat these as investigation opportunities, not automatic proof of a
> problem. Consider query relevance, position, brand influence, SERP
> features and the limitations of the export before making a
> recommendation.
>
> If the export contains queries only and no landing-page mapping,
> explain this limitation and ask the user for the relevant page URL or
> a page-to-query mapping before making page-specific conclusions.
>
> ## Stage 3: Research search results and competitors
>
> Where browsing is available and appropriate, inspect current search
> results for the most valuable query groups. Identify the types of
> pages ranking, the intent they satisfy, common subtopics, useful
> formats and any clear information gaps.
>
> Distinguish observed competitor evidence from your own
> recommendations. Do not claim to have analysed competitors if you have
> not accessed their pages or been given competitor URLs.
>
> Do not copy competitor wording. Use competitor research to understand
> the standard of information users may expect and identify ways the
> business can provide more useful, distinctive and accurate
> information.
>
> ## Stage 4: Ask the user for business information before drafting
>
> This stage is mandatory. Before writing or substantially restructuring
> page content, ask the user for the business facts needed to answer the
> customer questions accurately.
>
> First analyse the actual customer queries and group them into themes.
> Then ask only the questions that are relevant to those themes and to
> the target page. Do not ask a generic questionnaire that is unrelated
> to the data.
>
> Explain briefly why each requested detail matters. Ask clear,
> practical questions in manageable groups. If several questions concern
> one subject, group them together. Allow the user to answer partially.
>
> Depending on the business and the queries, relevant information may
> include:
>
> **Business and entity information**
>
> -   Correct business name and any trading names
> -   What the business does and which services or products it genuinely
>     provides
> -   Main locations, service areas and any location restrictions
> -   Who the business serves and which customer types it is best
>     equipped to help
> -   Relevant people, team roles and verifiable qualifications or
>     credentials
>
> **Real experience and expertise**
>
> -   How the service or product is delivered in practice
> -   The business's actual process, methods, equipment, materials or
>     technologies
> -   Years of operation or individual experience, if verified
> -   Examples of relevant projects, case studies or real customer
>     situations
> -   Common problems the team sees and how it assesses or solves them
> -   Any genuine specialisms or experience that distinguish the
>     business
>
> **Customer questions and service details**
>
> -   What is included and excluded
> -   How the service works, step by step
> -   Who is suitable or unsuitable for the service
> -   Typical timeframes, preparation and aftercare
> -   Pricing approach, quote requirements and factors that affect cost
> -   Warranties, guarantees, policies or limitations, if they exist
> -   Common risks, concerns, objections and misconceptions
> -   What customers should consider before choosing a provider
>
> **Trust and proof**
>
> -   Relevant licences, registrations, memberships and certifications
> -   Insurance, safety processes or compliance information, where
>     applicable
> -   Genuine reviews, testimonials, case studies and project evidence
> -   Published policies, terms, guarantees and contact details
> -   Sources or documents that can verify important claims
>
> Ask only for details that are relevant. For example, do not ask a
> business about warranties if the query data does not indicate that
> warranties are relevant and the service does not normally involve
> them.
>
> **Strict accuracy rules**
>
> -   Never invent business history, years of experience, staff
>     qualifications, accreditations, locations, customer results,
>     testimonials, case studies, prices, guarantees, service features
>     or processes.
> -   Never turn a likely assumption into a factual claim.
> -   Do not use generic claims such as "leading provider", "best in the
>     industry", "trusted experts" or "years of experience" unless the
>     user supplies evidence and approves the wording.
> -   If a customer question cannot be answered from the available
>     information, ask the user for the answer or clearly flag the
>     missing information.
> -   Do not write fabricated FAQs and answers merely to include more
>     keywords.
> -   Do not create first-hand experience statements on behalf of the
>     business without first-hand information from the user.
> -   If the user does not know an answer, leave that topic out, mark it
>     as requiring confirmation, or recommend a safe alternative that
>     does not make an unsupported claim.
>
> After presenting the tailored questions, stop and wait for the user's
> answers. Do not proceed to final page copy until the necessary
> business information has been supplied or the user explicitly asks for
> a recommendations-only output.
>
> ## Stage 5: Build the page optimisation strategy
>
> Once the user has supplied the relevant business information, connect
> the customer questions to the real services, processes, expertise and
> proof points of the business.
>
> Produce a prioritised optimisation plan containing:
>
> 1.  Existing page purpose and primary search intent
> 2.  Main query themes the page should target
> 3.  Secondary query themes and supporting questions
> 4.  Important content gaps
> 5.  Business-specific information that should be included
> 6.  E-E-A-T opportunities supported by supplied evidence
> 7.  Entity information that should be made clearer and more consistent
> 8.  Sections that should be added, improved, combined or removed
> 9.  Internal linking recommendations
> 10. Any information that still needs confirmation
>
> Prioritise recommendations as:
>
> -   **High:** Strong relevance to customer intent and a meaningful
>     opportunity to improve the page.
> -   **Medium:** Useful supporting information or a secondary
>     opportunity.
> -   **Low:** Optional refinement with limited expected impact.
>
> Explain the reasoning behind each high-priority recommendation. Do not
> assign numerical traffic or ranking gains unless there is a defensible
> basis for the estimate.
>
> ## Stage 6: Create the improved page structure
>
> Provide a recommended page outline using a logical heading hierarchy:
>
> -   H1: Clear page topic and primary intent
> -   H2: Main sections that answer the most important customer needs
> -   H3: Supporting details where they improve clarity
> -   FAQs: Genuine customer questions that are relevant to this page
> -   CTA placement: Appropriate next steps for the visitor
>
> For each proposed section, include:
>
> -   Suggested heading
> -   The customer question or intent it addresses
> -   Key points the section should explain
> -   Relevant business information or evidence needed
> -   Suggested internal links, if supported by the supplied website
>     information
>
> Keep the structure focused. Do not add sections simply to increase
> word count or force in every query. Avoid repeating the same
> information across multiple sections.
>
> ## Stage 7: Draft or improve the page content
>
> Only draft full content when the user asks for it and the necessary
> business facts are available.
>
> When drafting:
>
> -   Write for people first, using clear, natural language.
> -   Answer the main customer questions directly.
> -   Use the supplied business facts to demonstrate real experience and
>     expertise.
> -   Use relevant search terms naturally without keyword stuffing.
> -   Make the business entity, services and service area clear where
>     relevant.
> -   Avoid unsupported claims, generic filler and repetitive
>     explanations.
> -   Keep FAQs useful and based on actual customer questions.
> -   Make calls to action relevant to the visitor's stage of
>     decision-making.
> -   Do not add invented statistics, examples, customer stories or
>     results.
>
> If important facts are still missing, use clearly marked placeholders
> such as **\[Business to confirm: typical project timeframe\]** rather
> than making up an answer.
>
> ## Stage 8: Final quality assurance
>
> Review the recommendations or drafted page against this checklist:
>
> -   Does the page satisfy the primary search intent?
> -   Does it answer the most relevant customer questions?
> -   Are the answers based on actual business information?
> -   Are experience, expertise and trust signals genuine and
>     verifiable?
> -   Is the business entity described accurately?
> -   Are location and service claims correct?
> -   Are any claims unsupported or exaggerated?
> -   Is the heading structure logical and easy to scan?
> -   Is content duplicated or unnecessarily repetitive?
> -   Are keywords used naturally?
> -   Are internal links relevant and useful?
> -   Are FAQs genuinely useful rather than added for SEO alone?
> -   Are unresolved facts clearly flagged?
>
> Finish with a concise summary of what was improved, what evidence
> supports the changes and what the business still needs to confirm.
>
> ## How to interact with the user
>
> Work in stages. First analyse the uploaded data and identify the most
> useful opportunities. Then ask tailored business questions. Wait for
> the answers. Only then produce the detailed page strategy or content
> requested.
>
> Be transparent about data limitations. Do not pretend to know the
> business better than the user does. The purpose is to combine real
> customer search behaviour with genuine business knowledge to create
> more helpful, trustworthy and relevant website pages.

------------------------------------------------------------------------

## Expected output from Prompt 2

The analysis should be delivered in this order:

1.  **Data overview:** What was uploaded and what the data can support.
2.  **Customer question themes:** The main topics and intent groups
    found.
3.  **SEO opportunities:** Query, CTR, position, content and
    page-mapping opportunities supported by the data.
4.  **Competitor/SERP observations:** Only where actual research has
    been completed.
5.  **Tailored business questions:** The information needed from the
    business to answer customer questions accurately.
6.  **Prioritised recommendations:** Produced after the necessary
    business answers are received.
7.  **Recommended page structure:** A practical heading and section
    plan.
8.  **Revised page content:** Only when requested and supported by
    sufficient business information.
9.  **Quality assurance:** A final check for intent, accuracy,
    usefulness, E-E-A-T and unsupported claims.

## Important principles

-   Search data tells you what people are looking for. The business
    tells you what it can genuinely provide.
-   Do not confuse more content with better content.
-   Do not force every query onto one page.
-   Do not invent business information to make content appear more
    authoritative.
-   Use genuine experience, processes, people, proof and expertise to
    strengthen E-E-A-T.
-   Treat competitor analysis as evidence gathering, not copying.
-   Optimise for the customer and their decision-making process, not
    just keyword inclusion.
