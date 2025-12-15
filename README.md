# L10nIssues Dataset (Partial Release)

This repository contains a **partial and evolving release** of the *L10nIssues* dataset, a curated collection of GitHub issues related to internationalization (i18n) and localization (l10n) defects.

The dataset focuses on **real-world issues that include screenshots**, enabling the study of visually observable localization problems such as missing translations, layout breakage, text truncation, and right-to-left (RTL) issues.

⚠️ **Important:**  
This is an *early release*. The dataset is **still under active manual curation**, and its size and content will change as new issues are reviewed and annotated.

---

## Dataset Overview

- Source: Public GitHub repositories
- Time span: 2014–2024
- Issue type: i18n/l10n-related bugs
- Media: All issues include at least one screenshot
- Status: **Partially curated (work in progress)**

Each issue was manually reviewed to ensure relevance to localization or internationalization defects. In some cases, a single issue may be associated with multiple bug types.

---

## Dataset Schema

The CSV file uses the following schema:

| Attribute       | Description |
|-----------------|-------------|
| `issue_id`      | Unique identifier of the issue |
| `repo_full`     | Full repository name (e.g., `owner/repo`) |
| `repo`          | Repository name only |
| `title`         | Issue title |
| `url`           | Direct link to the issue |
| `labels`        | Labels assigned to the issue |
| `image_urls`    | URLs of attached images |
| `bug_types`     | Assigned bug classification(s) |
| `created_at`    | Issue creation timestamp |
| `stars`         | Repository star count |
| `license`       | Declared repository license |
| `platform`      | Affected platform (e.g., web, mobile) |
| `language`      | Target localization language |

---

## Intended Use

This dataset is intended to support:

- Empirical studies on i18n/l10n defects  
- Training and education of QA engineers and testers  
- Development and evaluation of tools for detecting localization issues  
- Multimodal analysis combining text and screenshots  

---

## Current Limitations

- The dataset is **not yet fully curated**
- The number of issues is **not representative of the full population** of i18n/l10n bugs on GitHub
- Bug type labels and metadata may evolve in future releases

A fully curated and expanded version of the dataset will be released in future updates.

