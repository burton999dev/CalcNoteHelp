# Gemini Project Context: CalcNote Help

## Project Overview
This repository contains the online documentation and help resources for **CalcNote**, a notepad calculator application for Android. The project serves static content via GitHub Pages, with documentation available in English and Japanese.

## Directory Structure
*   **`documents/`**: Contains the main documentation source files in Markdown.
    *   `ja/`: Japanese documentation.
    *   `en/`: English documentation.
    *   `all/`: Shared documents like privacy policy and terms.
*   **`docs/`**: The public-facing directory served by GitHub Pages. Contains HTML files, stylesheets, and localized privacy policies/terms.
*   **`images/`**: Stores images and screenshots used in the documentation, organized by language (`ja`, `en`, `all`).
*   **`AGENTS.md`**: Specific guidelines for AI agents and contributors regarding repository structure and conventions.

## Key Files
*   **`README.md`**: The entry point for the repository, containing links to the main help indexes (`documents/ja/index.md` and `documents/en/index.md`).
*   **`documents/{lang}/index.md`**: The table of contents for the documentation in each language.
*   **`docs/index.html`**: The main landing page for the GitHub Pages site.
*   **`docs/params.json`**: Configuration file for the GitHub Pages generator.

## Development Workflow
Since this is a static documentation site without a build process:
1.  **Editing**: Modify the Markdown files in `documents/`. Ensure changes are reflected in both English and Japanese directories if applicable.
2.  **Previewing**: Use a Markdown previewer or run a local server (e.g., `python -m http.server`) inside the `docs/` directory to check HTML files, although the core content is in `documents/`.
3.  **Images**: Place new images in the `images/` directory.

## Conventions
*   **Markdown Style**:
    *   Use ATX headers (`#`).
    *   Use `-` for unordered lists with 2-space indentation.
    *   Prioritize relative links.
*   **Naming**: Use lowercase snake_case for filenames (e.g., `custom_extension.md`).
*   **Localization**: Maintain parity between English and Japanese documentation where possible.
*   **Commit Messages**: Use concise Japanese summaries explaining *why* the change was made (e.g., "FAQを更新").

## Build & Test
*   **No Build Step**: There are no build scripts or package managers (`package.json`, `Makefile`, etc.).
*   **Manual Verification**: Check for broken links and correct image rendering manually before committing.
