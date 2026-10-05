# Repository Instructions

## Purpose

Maintain the KROS newsletter "지식나눔" archive published through the Jekyll site in this repository.

## Newsletter update workflow

When asked to add or update a KROS newsletter entry:

1. Read the latest `README.md` before making changes.
2. Find the requested newsletter on the official [KROS website](https://kros.org/).
3. Verify all metadata against the original KROS pages:
   - publication year and volume number;
   - newsletter title and URL;
   - 지식나눔 title;
   - author names and affiliations;
   - 지식나눔 article URL.
4. Treat the two KROS page types separately:
   - newsletter pages normally use `B_CATE=BBS5`;
   - 지식나눔 article pages normally use `B_CATE=BBS7`;
   - preserve the exact `b_code` belonging to each page.
5. Check for an existing volume, article title, article URL, or `b_code` before adding a row. Do not create duplicates.
6. Add the entry to the existing Markdown table in chronological order using this form:

   `| [YYYY. Vol. N](NEWSLETTER_URL) | [ARTICLE_TITLE](ARTICLE_URL) | AFFILIATION AUTHOR |`

7. Preserve the table headers, surrounding prose, link style, and existing entries unless the user explicitly requests another change.
8. Correct obvious spacing artifacts introduced by the KROS webpage, but do not paraphrase or translate article titles, author names, or affiliations without explicit instruction.
9. Modify only files required by the request. A normal newsletter update should change only `README.md`.
10. After editing, read the changed section again and verify:
    - the new row appears exactly once;
    - year and volume order are correct;
    - Markdown table column counts remain consistent;
    - both URLs point to the intended KROS pages;
    - title, author, and affiliation match the official source.
11. Report the added entry and provide the resulting change or commit link.

## Site styling

- The site uses the `jekyll-theme-primer` theme.
- Preserve responsive behavior when changing desktop layout.
- The custom desktop maximum width is defined in `assets/css/style.scss`.
- Do not alter site styling during a newsletter-content update unless explicitly requested.

## Safety and scope

- Use the official KROS website as the authoritative source.
- If the requested volume is not yet published or its metadata is ambiguous, stop and report what could not be verified.
- Do not invent missing titles, authors, affiliations, URLs, or `b_code` values.
- Do not add a repository-level `SKILL.md`; reusable personal Skills are installed separately from repository instructions.
