# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository purpose

This is Mohammad Sekandar Hossain's personal portfolio repository, showcasing projects in Artificial Intelligence, Environmental Science, GIS, Python, and Data Analysis. It is **not a software application** — there is no build system, package manifest, linter, or test suite. Content is primarily Markdown READMEs, one Jupyter notebook, and image assets (map screenshots, chart outputs). Treat changes here as documentation/content edits, not software engineering changes requiring build/lint/test verification.

## Structure

Each top-level directory is a self-contained project category with its own `README.md` describing objectives, tools used, and findings:

- `ai-projects/` — AI/ML projects. Has both a category-level `README.md` and a nested `air-quality-prediction/` project with its own README and `Untitled0.ipynb` notebook (UCI Air Quality dataset; compares Linear Regression vs. Random Forest to predict CO concentration).
- `data-analysis/` — category overview of EDA, visualization, and environmental data analysis work (no sub-projects yet, description only).
- `gis-projects/` — QGIS-based urban facilities accessibility analysis; README plus numbered screenshot PNGs (`01_project_overview.png` through `07_final_map_layout.png`) documenting the QGIS workflow step by step. Contains a nested `urban-utility-network/` project scaffold (`data/`, `data/layers/`, `maps/`, `outputs/`, `screenshots/`) that is currently empty aside from `.gitkeep` placeholders and an empty `README.md` — this is a work-in-progress project skeleton, not yet documented.
- `gis-project/` (singular, distinct from `gis-projects/`) — currently just holds a placeholder `GIS_TEST_MAP.png`.
- `python-projects/` — category overview of Python-based data analysis and geospatial projects (no sub-project folders yet, description only).
- `powerbi-financial-sales-analysis` — currently a stray near-empty file (not a directory); likely a placeholder for an upcoming Power BI project.
- `README.md` (root) — the main portfolio landing page: bio, technical skills table, links to project categories, education, and contact info. Keep this in sync when adding or renaming project categories.

## Conventions to follow

- Each project/category README follows a consistent emoji-header Markdown structure: Project Overview, Objectives, Technologies/Tools, Dataset/Methods, Results/Key Findings, and (for completed projects) a "Project Structure" code block and "How to Run" section. Match this structure when adding new project READMEs.
- New completed projects should be linked from both their category README and the root `README.md`.
- Numbered screenshots (e.g. `gis-projects/01_...png` through `07_...png`) represent a sequential workflow — preserve the numbering order if adding more.
- `.gitkeep` files mark placeholder directories reserved for future project output (data, maps, outputs, screenshots) — do not remove them unless replacing with real content.
- Notebook work lives directly in the project folder alongside its README and referenced dataset (see `ai-projects/air-quality-prediction/`); there is no separate `notebooks/` or `src/` convention yet.
