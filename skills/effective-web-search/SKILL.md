---
name: effective-web-search
description: Guides the agent on how to formulate precise web search queries, evaluate sources, and synthesize information into structured, highly readable, and accurate responses. Use this when answering questions that require up-to-date information, factual verification, or aggregating data from multiple sources.
---

# Effective Web Search

This skill teaches you how to maximize the value of web search tools, ensuring you retrieve high-quality information and present it in a clear, authoritative, and user-friendly format.

## When to Use This Skill

Apply these guidelines whenever the user's prompt requires external search, specifically when:

*   **Seeking current events:** News, sports scores, stock prices, or recent releases.
*   **Troubleshooting:** Niche bugs, fresh error codes, or undocumented software issues.
*   **Requesting comparisons:** Product reviews, market alternatives, or software benchmarking.
*   **Verifying facts:** Debunking claims, checking statistics, or finding primary sources.
*   **Aggregating data:** Gathering disparate pieces of information (e.g., "What are the top 5 highest-grossing movies of 2025 and their budgets?").

---

## Step-by-Step Search Workflow

### Step 1: Formulate Precise Queries

Do not simply pass the user's natural language question into the search tool. Translate their intent into highly optimized keyword strings.

1.  **Extract Core Entities:** Remove filler words (who, what, where, why). Focus on nouns, proper names, and specific verbs.
2.  **Use Search Operators:**
    *   `site:reddit.com` or `site:github.com` for community discussions and developer issues.
    *   `"exact phrase"` for specific error logs or quotes.
    *   `filetype:pdf` for academic papers or official reports.
3.  **Run Parallel Searches:** Always fire multiple, diverse queries simultaneously rather than waiting to refine sequentially. Issuing 3-4 varied queries at once saves time and gathers a broader context instantly.

*Example:*
*   **User:** "Why is my Next.js app throwing a hydration error after I updated to version 15?"
*   **Bad Query:** `Why is my Next.js app throwing a hydration error after I updated to version 15?`
*   **Good Parallel Queries:** `next.js v15 hydration error`, `site:github.com/vercel/next.js "hydration failed" v15`, `next.js 15 breaking changes hydration`

### Step 2: Evaluate and Refine

**Do not accept the first set of results blindly.** Evaluate the snippets:

1.  **Authority:** Prioritize official documentation, reputable news outlets, and primary sources over content farms or SEO-spam blogs.
2.  **Recency:** Check dates in snippets to ensure the information isn't outdated (especially for tech, law, and news).
3.  **Refinement:** If the initial parallel results completely missed the mark, run a fast follow-up batch with adjusted keywords, narrower scope, or exclusion operators (e.g., `-spamword`).

### Step 3: Synthesize Information

Never just regurgitate search snippets. Process the information:

1.  **Cross-Reference:** If a claim is bold or controversial, ensure multiple independent sources corroborate it.
2.  **Resolve Conflicts:** If sources disagree (e.g., different specs for a phone), note the discrepancy for the user.
3.  **Extract the Signal:** Cut through the noise. Identify the exact answer the user needs without the fluff of a blog post recipe.

### Step 4: Present the Results Effectively

How you format the answer is just as important as the information itself. Follow the **BLUF** principle (Bottom Line Up Front).

1.  **Direct Answer First:** Start with a concise summary answering the core question.
2.  **Structured Hierarchy:** Use Markdown headings (`###`), bullet points, and numbered lists to make the content scannable.
3.  **Use Tables for Comparisons:** If the user asks to compare items, data, or specs, always use a Markdown table.
4.  **Cite Your Sources Inline:** Embed links naturally in the text using clean Markdown formats like `[Source Name](https://example.com)`. Avoid dumping naked URLs at the bottom unless specifically requested, as inline citations make the results cleaner and easier to verify in context.

**Example of a Good Presentation:**

> ### The Bottom Line
> The error `ERR_MODULE_NOT_FOUND` in your Node.js project is likely occurring because you are using ES Modules (`"type": "module"`) but missing the `.js` extension in your local import statements.
>
> ### How to Fix It
> 1. **Update Imports:** Ensure all relative imports include the file extension.
>    * *Change:* `import { helper } from './helper'`
>    * *To:* `import { helper } from './helper.js'`
> 2. **Check package.json:** Verify that `"type": "module"` is correctly set.
>
> ### Why this happens
> According to the [official Node.js documentation](https://nodejs.org/api/esm.html), ES module resolution strictly requires file extensions for relative paths, unlike CommonJS.

---

## Common Query Strategies

Use these patterns to optimize searches across different domains:

| Domain | Strategy | Example Parallel Queries |
| :--- | :--- | :--- |
| **Tech/Coding** | Target official docs, GitHub issues, and StackOverflow. | `site:github.com "TypeError: fetch failed" node 20`, `node 20 fetch failed stackoverflow` |
| **News/Events** | Use specific dates, names, and locations. | `Federal Reserve interest rate decision January 2026`, `FED rate hike news Jan 2026` |
| **Reviews** | Target aggregator sites or specific communities. | `best mechanical keyboard 2026 site:reddit.com/r/MechanicalKeyboards`, `rtings mechanical keyboard review 2026` |
| **Academia** | Focus on domain extensions (`.edu`, `.gov`) or specific hubs. | `impact of microplastics on marine life site:ncbi.nlm.nih.gov`, `microplastics ocean ecosystems filetype:pdf` |

---

## Handling Search Failures

If you run parallel searches and cannot find a reliable answer:

1.  **Be Transparent:** Explicitly state that you searched the web but could not find current or verifiable information on the topic.
2.  **Avoid Hallucination:** Do not invent facts to fill the gap.
3.  **Offer Alternatives:** Provide the closest related factual information you *did* find, or suggest alternative ways the user might phrase their question or find the data.

**Example Response for Failure:**
> I searched the web for recent benchmarks comparing the "UltraChip X9" to the "MegaProcessor 5000," but it appears no reputable tech outlets have published independent reviews yet. The chips were only announced yesterday. 
> 
> However, based on the manufacturer's press release, the UltraChip X9 claims a 20% efficiency boost. Would you like me to summarize the official spec sheet instead?
