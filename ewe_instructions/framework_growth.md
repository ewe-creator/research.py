# Market Metrics & Impact: How to Win

Building a good framework is engineering; building a *successful* one is marketing and community management.

## 1. Documentation is Product

Your documentation is the single biggest factor in adoption.

*   **The Diátaxis Framework**: Structure your docs into 4 quadrants:
    1.  **Tutorials**: Learning-oriented (Step-by-step generic lesson).
    2.  **How-to Guides**: Problem-oriented (Steps to solve a specific problem).
    3.  **Reference**: Information-oriented (API specs).
    4.  **Explanation**: Understanding-oriented (Background, design decisions).

*   **Tools**:
    *   **MkDocs with Material Theme**: The modern standard. Fast, beautiful, searchable.
    *   **Interactive Examples**: Use tools like `pyodide` in browser if possible, or simple copy-paste blocks.

## 2. High Market Metrics (PyPI & GitHub)

To rank high and get downloads:

*   **PyPI Metadata**: Fill every field in `pyproject.toml`.
    *   `classifiers`: Crucial for search (e.g., `Framework :: Django`, `Topic :: Software Development`).
    *   `project_urls`: Link to Documentation, Source, Tracker.
*   **Readme.md**: The "Landing Page".
    *   **Above the Fold**: One-line value prop + `pip install` command + "Hello World" example code.
    *   **Badges**: Use Shields.io (Coverage, CI Status, PyPI version, Downloads). These signal "Active & Stable".

## 3. Community & Consistency

*   **Issue Templates**: Reduce friction for users reporting bugs.
*   **GitHub Discussions**: Separate help requests from bug reports.
*   **Changelog**: Keep a `CHANGELOG.md` following [Keep a Changelog](https://keepachangelog.com/). It shows respect for your users' time.

## 4. Growth Strategy

1.  **Solve a painful problem** initially (Niche).
2.  **Expand** via plugins (see Architecture).
3.  **Engage**: Respond to issues within 24-48 hours. Early adopters are your evangelists.
