# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## Added
* Two new demos: `usage-grid-social-network.py` and `usage-concentric-social-network.py`
* Add Issue and PR templates for Github (located in `.github`)

## Changed
* `usage-*.py` - Modified all the import statements from `import dash_cytoscape` to `import dash_cytoscape as cyto`. Also optimized imports.
* `usage-phylogeny.py` - Clear callback conditional statement
* `CONTRIBUTING.md` - changed `dash-cytoscape-0.0.1` to `dash-cytoscape-x.x.x`. Added a **Code quality & design** section. Changed the **Making a contribution** section and updated title to **Publishing**. Updated **Pre-Release checklist**.
* `npmignore` - Added `venv` to avoid venvs to be included in the npm distribution package, which makes us a large amount of space and many unnecessary files being distributed.

## Removed
* `extract-meta.js`, `extract-meta` - they were moved to the dash component CLI, thus are not needed anymore
* `config.py`, `runtime.txt`, `Procfile`, `index.html` - only needed for hosting `usage-*.py` on DDS, they are now moved to `plotly/dash-cytoscape-demos`.
* `review_checklist.md` -  redundant since all the information is already contained in CONTRIBUTING.md

## [0.0.4] - 2018-01-19

### Added
* Homepage URL for PyPi
* Long Description for PyPi

### Changed
* Cytoscape component docstring for thorough and well-formatted references (#26)
* Refactored code base to match the up-to-date version of `dash-component-boilerplate` (#27)

### Fixed
* Console error where `setProps` gets called even when it is undefined (# 28)
* Incorrect setProps assignment that causes `setProps` to not be properly defined when nested in bigger apps (e.g. `dash-docs`) (#28)

## [0.0.3] - 2018-12-29
### Added
* Detailed usage example for rendering Biopython's Phylo object (phylogeny trees)
into a Cytoscape graph, with interactive features such as highlighting.

### Updated
* React-Cytoscapejs version, from 1.0.1 to 1.1.0 

## [0.0.2] - 2018-11-08
### Added
* Author email and improve description
* Data section of demos readme
* Added the components "dash", "dash-html-components", and "dash-renderer" as explicit package requirements.

### Changed
* Move grid layout data file
* Change App.js react demo data to be local
* Installation steps in readme to use yarn


### Updated
* Cytoscape.js version, correct component import

### Fixed
* Correct unpkg link error
* Markdown formatting for CONTRIBUTING.md


## [0.0.1] - 2018-11-03
### Added
- First pre-release version of dash-cytoscape. Still WIP, so prepare to see it break 🔧
