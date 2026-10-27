# SCAE Web Preview

Public **synthetic-data-only** web preview for the Walking Comet Security Control Assessment Engine (SCAE).

**Source of truth:** The private `pdomoney/security-control-assessment-engine` repository. This public repository is solely for static frontend output and **must not** receive private engine source code, client evidence, database files, credentials, API tokens, assessor records, or actual security assessment reports.

## Publishing

The private repository's reviewed GitHub Actions workflow builds and tests the React/TypeScript frontend, then copies **only** its compiled static output into `docs/` in this public repository.

GitHub Pages should be configured as:

- **Source:** Deploy from a branch
- **Branch:** `main`
- **Folder:** `/docs`

After the first successful static publication, the development preview address will be:

https://pdomoney.github.io/scae-web-preview/

No live assessment backend, Microsoft tenant collection, LLM processing, or persistent customer data connection is provided by the public preview.

## Safety notice

Everything on this site is public. **Never upload actual evidence, credentials, sensitive client records, or assessment artifacts.** The preview uses fictional fixtures solely for UI development and browser testing.
