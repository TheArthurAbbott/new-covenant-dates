# Copilot Instructions for TheArthurAbbott/new-covenant-dates

This document provides onboarding instructions to optimize the use of Copilot within this repository. Follow these guidelines to perform tasks efficiently and accurately.

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
  - `.github/`: Contains workflows. Used for CI setups and file validation.
  - `70-sevens/`: Contains dating of events regarding Daniel's 70 weeks of years.

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

## Copilot-Specific Instructions

### Citation Style: Wikipedia-Style Footnotes

1. **Numerical Citations Only:**
   - In the main body text, citations shall appear as **simple numerical references in square brackets** (e.g., `[1]`, `[2]`, `[3]`).
   - These numbers must be **non-descriptive** and purely sequential.
   - Readers should encounter only the number in the main text without any descriptive text or author names inline.

2. **Footnote Format:**
   - At the end of each document or section, create a footnotes section with the heading `## References` or `## Footnotes`.
   - Each numbered entry must follow this exact format:
     ```
     [1] Article Title. Author Name. URL
     ```
   - Example:
     ```
     [1] The Chronology of the New Testament. John Smith. https://example.com/article
     ```

3. **Dead Link Policy:**
   - **No dead links are permitted.** Before including any source, verify the link is active and accessible.
   - If a source link is dead or inaccessible:
     a. Attempt to locate the original content using **archive.org (Internet Archive Wayback Machine)**.
     b. If an archived version exists and can be reliably accessed, use the archive.org URL instead: `https://web.archive.org/web/[date]/[original-url]`
     c. If the source cannot be found on archive.org or the archived version is incomplete/unreliable, **do not use the source**. Replace it with an alternative source that meets credibility standards.

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
