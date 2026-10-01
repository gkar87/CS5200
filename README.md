# CS5200 · Database Playgrounds

Interactive, self-contained course readers for **CS5200 / CS4600 — Database Theory and Applications**,
prepared by **Dr. Gorkem Kar**.

**Live site:** https://gkar87.github.io/CS5200/

## What this is

Fifteen playgrounds that build from foundations to formal theory. Each one pairs a short reading with
worked examples, a self-check quiz, and practice problems — and **every SQL example runs for real in
your browser**, so you can edit it and see what happens. Nothing needs to be installed and nothing is
simulated: the pages load SQLite compiled to WebAssembly (`sql.js`) and execute your statements against
a live database.

## Contents

| # | Playground |
|---|---|
| 1 | [Why Databases? From Files to DBMS](1_why_databases_playground.html) |
| 2 | [DBMS Architecture and Data Independence](2_dbms_architecture_playground.html) |
| 3 | [SQL Quickstart](3_sql_quickstart_playground.html) |
| 4 | [ER Modeling Basics](4_er_modeling_playground.html) |
| 5 | [Extended ER — Inheritance and Aggregation](5_eer_inheritance_aggregation_playground.html) |
| 6 | [Relational Model and ER-to-Relational Mapping](6_relational_mapping_playground.html) |
| 7 | [Relational Algebra](7_relational_algebra_playground.html) |
| 8 | [DDL, Constraints and Data Types](8_constraint_violation_predictor_playground.html) |
| 9 | [Single-Table SELECT and Set Operations](9_null_trap_detector_playground.html) |
| 10 | [Joins and Subqueries](10_join_pattern_selector_playground.html) |
| 11 | [Aggregation, GROUP BY and HAVING](11_aggregation_playground.html) |
| 12 | [CTEs and Recursive Queries](12_cte_recursive_playground.html) |
| 13 | [Window Functions and Views](13_window_functions_and_views_playground.html) |
| 14 | [Functional Dependencies and Keys](14_fd_keys_playground.html) |
| 15 | [Normal Forms and Decomposition](15_normal_forms_playground.html) |

Start at **[index.html](index.html)** and work down — each page links to the next.

## Notes for students

- Everything runs **entirely in your browser**. No account, no install, no server.
- Your edits stay in the page; reloading resets a cell to its starting query.
- These pages are best read on a laptop or desktop. They work on a phone, but the SQL editors are
  much easier to use on a larger screen.
- The `Run` button executes whatever is in the box, so it is a safe place to make mistakes — that is
  what it is for.

## Technical

- Plain static HTML/CSS/JS — no build step, no dependencies to install.
- SQLite via [`sql.js`](https://github.com/sql-js/sql.js) 1.14.2 (WebAssembly), loaded from cdnjs.
- Typefaces: Source Serif 4 and IBM Plex Mono, loaded from Google Fonts.
- Published with GitHub Pages from the `main` branch, repository root.

Because the pages fetch `sql.js` and the fonts from public CDNs, an internet connection is needed the
first time you open a page.
