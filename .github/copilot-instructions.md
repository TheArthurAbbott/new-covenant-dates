# AI Instructions for TheArthurAbbott/new-covenant-dates

This document provides onboarding instructions to optimize the use of an AI like Copilot within this repository. Follow these guidelines to perform tasks efficiently and accurately.

---

## Repository Summary

### Purpose
This repository focuses on dating significant scriptural events, such as Daniel's 70 weeks, using both Biblical and extra-Biblical historical sources. It emphasizes unbiased research, academic rigor, and clear documentation of sources for verifiable historical analysis.

### Key Details
- **Language:** Markdown and any parsing language for managing historical data processing.
- **Frameworks/Targets:** This project primarily uses Markdown for documenting research. There are minimal runtime dependencies.
- **Size:** Small to medium-sized files, primarily research documentation.

---

## Build and Validation Instructions

### Instructions for Bootstrap, Validation, and Changes
1. **Always Sync with 'Practice' branch:**
   - This repository uses the `practice` branch as the primary working branch for updates.
2. **Environment Setup:**
   - No complex setups or dependencies required.
   - Ensure Markdown preview tools are in place for reviewing `.md` files.
3. **Testing Research Accuracy:**
   - Any claims must include citations. Cross-reference Biblical sources with **two extra-Biblical sources.**
   - Validate sources with high credibility levels (peer-reviewed research, museum publications, etc.).
   - Links are mandatory for every footnote.
4. **Best Practices for Edits:**
   - Use summary tables to present comparative data concisely.
   - Prioritize clear section structures for each research sub-question.
   - Cite key sources for claims but ensure scriptural references are cross-dated by **historical records.**
5. **Formatting and Linting:**
   - Never use unverifiable or "soft" links (e.g., blogs without institutional authors). Wikipedia is acceptable only if tracing through its citations to primary or secondary trusted sources.

---

## Project Layout

### Guidance for Copilot

#### Root-level Files
- **README.md:** General project introduction. Refer here first for context.
- **Key Directories:**
  - `.github/`: Contains workflows, copilot instructions, and the article summary template.
  - `70-sevens/`: Contains dating of events regarding Daniel's 70 weeks of years.
  - `article-summaries/`: Contains structured summaries of external articles relevant to New Covenant dating.

#### Validation Pipelines
- Validate Markdown (`.md`) syntax and content structure regularly to ensure proper rendering and hyperlink functionality.
- Review GitHub Actions workflows to understand automated processes linked to file updates and validations.

#### Common Patterns
- **Citations Expectations:**
  - Use **footnotes** for all citations explicitly.
  - Provide **direct links** to high-quality sources. All sources listed must:
    a. Reference factual historical data.
    b. Enhance the credibility of scriptural dating where applicable.

### Checks Prior to a Pull Request
- Test Markdown rendering.
- Confirm that all sources include links.
- Reassess summary tables for clarity and correctness.
- Ensure alignment with the repository theme—**accurate cross-dating of scriptural events.**

---

## AI-Specific Instructions

### Citation Style: Wikipedia-Style Footnotes

1. **Numerical Citations Only:**
   - In the main body text, citations shall appear as **simple numerical references in square brackets** (e.g., `[1]`, `[2]`, `[3]`).
   - These numbers must be **non-descriptive** and purely sequential.
   - Readers should encounter only the number in the main text without any descriptive text or author names inline.

2. **Footnote Format:**
   - At the end of each document or section, create a footnotes section with the heading `## References` or `## Footnotes`.
   - Each numbered entry must follow this exact format:
     ```
     [1] Source Title. Institution/Publisher. URL
     > "A sizable, representative quotation from the source document that
     > provides the reader with the key passage or evidence being cited,
     > so they can evaluate the claim without needing to visit the link."
     ```
   - **Source Quotation Requirement:** Every footnote **must** include a direct quotation from the source material, formatted as a Markdown blockquote (`>`). The quotation should:
     a. Be **sizable and representative** — not a single phrase, but a full sentence or short paragraph that conveys the source's argument or evidence in context.
     b. Contain the **specific passage** that supports the claim being made in the main text.
     c. Be **faithfully reproduced** from the source. Use `[...]` to indicate omitted portions if trimming for length, but do not alter the meaning.
     d. For non-English sources (e.g., ancient inscriptions, cuneiform translations), quote the **English translation** provided by the source, and note the translator or translation edition if available.
   - Example:
     ```
     [1] Babylonian Chronicle (ABC 5, Jerusalem Chronicle). Livius.org. https://www.livius.org/sources/content/mesopotamian-chronicles-content/abc-5-jerusalem-chronicle/
     > "In the seventh year, in the month of Kislev, the king of Akkad
     > mustered his troops, marched to the Hatti-land, and encamped
     > against the city of Judah and on the second day of the month of
     > Adar he seized the city and captured the king. He appointed there
     > a king of his own choice, received its heavy tribute and sent
     > them to Babylon."
     ```
     ```
     [2] Cyrus Cylinder. The British Museum. https://www.britishmuseum.org/collection/object/W_1880-0617-1941
     > "I returned the images of the gods, who had resided there, to
     > their places and I let them dwell in eternal abodes. I gathered
     > all their inhabitants and returned to them their dwellings. [...]
     > I collected together all of their people and returned them to
     > their settlements."
     ```

### Dead Link Verification & Replacement Protocol

**Critical Rule:** No dead links are permitted in any document. All URLs must be tested and verified as active before inclusion.

1. **Link Verification Process:**
   - Before finalizing any source, verify the link is active and accessible.
   - Test links by attempting to access the full page/resource and confirm it contains the expected information.
   - Check that the content matches the citation's description (e.g., if citing a museum artifact, confirm the URL contains museum collection records, not unrelated pages).

2. **When a Link is Dead or Inaccessible:**
   - **Step 1 - Search for Alternatives:**
     - Identify the primary source institution (museum, archive, academic publisher, etc.).
     - Search for the source on that institution's official website using their search function.
     - If the direct institutional link is unavailable, proceed to Step 2.
   
   - **Step 2 - Use Archive.org (Internet Archive Wayback Machine):**
     - Visit https://web.archive.org and search for the original dead URL.
     - If archived snapshots exist, review them to confirm they contain the source material and are complete/readable.
     - Use the archived URL if the snapshot quality is reliable: `https://web.archive.org/web/[YYYYMMDD]/[original-url]`
     - Only use archive.org links if the captured content is legible and substantially complete.
   
   - **Step 3 - Seek Reliable Alternative Sources:**
     - If archive.org has no useful snapshots, search for the same source on established academic platforms:
       - **For Mesopotamian texts/chronicles:** Livius.org (established ancient history resource with peer-reviewed translations)
       - **For classical texts:** Perseus Digital Library (Scaife Viewer), Project Gutenberg (for public domain texts)
       - **For museum collections:** Direct links to institution's official collection database
       - **For academic publications:** Internet Archive Scholar, Google Scholar, institutional repositories
     - The replacement source must provide equivalent or superior information and credibility to the original.
     - Prioritize sources that offer translations, scholarly commentary, or direct museum/institutional curation.
   
   - **Step 4 - If No Suitable Alternative Exists:**
     - Do not use the source.
     - Locate a different, verified source that covers the same historical material.
     - If multiple attempts fail to find a working link for a critical source, flag the citation in a comment and work with repository maintainers to find a solution.

3. **Best Practices for Link Reliability:**
   - Prefer **direct institutional sources** (museum collections, university libraries, government archives) over secondary aggregators.
   - Verify that URLs use consistent naming conventions across the institution's website (some sites update URL structures, causing old links to break).
   - Test variations of URLs if initial links fail (e.g., if `/content/` returns 404, try removing it: `/mesopotamian-chronicles/`).
   - Keep links concise and avoid overly specific URLs that include session IDs or temporary parameters.
   - When citing a specific work (e.g., Book XI of Josephus' Antiquities), ensure the URL links directly to that section, not just the homepage.

4. **Documentation & Auditing:**
   - If a link replacement was necessary, note the reason briefly in a commit message or comment (e.g., "Replace broken CDLI link with Livius.org source for better accessibility").
   - Periodically audit links in documents (especially those citing online-only sources) to identify and fix dead links before they propagate.

### Article Summary Format

When creating article summaries in the `article-summaries/` directory, follow the template at **`.github/article-summary-template.md`**. Key conventions:
- **Section headings** use the format `## Event Name: Date BC/AD`.
- For date ranges, use `## Event Name: Date-Date BC/AD`.
- Each event section must include a **blockquote** from the article and a **commentary** paragraph.
- End with a **Summary** table and a closing commentary on significance to other New Covenant events.
- Note any known biases in the author's interpretation in the opening summary.

### Dating Principles

1. Always cross-reference **Biblical sources** with at least two **extra-Biblical historical sources** where possible. Avoid unverifiable data.
2. **Bias-Free Interpretation:** Be rigorous in presenting unbiased interpretations. Ensure analysis represents multiple datasets, outlining disagreements clearly.
3. **Source Validation:** Every citation requires a direct, verified link. Prioritize **direct access sources** like museum artifacts, journal-level historical timelines, or highly accredited archives.
4. **Preferred Outputs:**
   - Summary tables for organizing dated events.
   - Sectioned narratives explaining each data point prior to table inclusion.
5. **Content Limitations:**
   - Avoid speculative data without corroborating sources.
   - Focus solely on providing useful, repeatable observations.

---

This file should only be updated to fix inaccuracies, add steps, or improve clarity for better repository handling.
