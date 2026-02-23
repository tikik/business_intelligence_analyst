## Ethos-Aligned Institutional Analytics Prototype

Governance-First Integration • Certified Metrics • Decision Support

---

### Executive Overview

This repository presents a governance-aligned institutional analytics prototype designed to demonstrate:

- Multi-system integration (Banner, Navigate, Ad Astra via Ethos)

- Certified metric construction using SQL views

- Census-aligned cohort logic

- FERPA-aware aggregation and small-cell suppression

- Role-based dashboard delivery in Power BI

The goal of this prototype is to illustrate how institutional data can move from reactive reporting toward proactive, repeatable decision support — while maintaining data governance standards.

This repository contains synthetic data only. No real student information is included.

---

### Strategic Purpose

Institutions frequently encounter:

- Conflicting definitions across systems

- Manual reporting workflows

- Inconsistent cohort logic

- Capacity planning blind spots

- Graduation and credential capture gaps

This prototype addresses those challenges by introducing a layered architecture:

- Integration & Validation

- Certified Metric Views

- Role-Based Dashboard Delivery

Dashboards do not query transactional tables directly. All reporting logic flows through certified SQL views.

#### What This Prototype Demonstrates

1. Certified Definitions

Cohort logic, graduation metrics, and credit velocity thresholds are defined in reusable SQL views. This prevents silent definition drift across reports.

2. Census-Aligned Cohort Logic

Entry term cohorts are defined at census freeze, ensuring consistent graduation and retention tracking.

3. Privacy-by-Design

Small-cell suppression (<5) is applied to protect student confidentiality in aggregate reporting.

4. Capacity & Momentum Modeling

Analytics support questions such as:

Are students on pace for 15 credits?

Where are scheduling bottlenecks constraining growth?

Which programs drive retention stability?

Are certificate completions being captured before transfer?

### Architecture Overview

- Layer 1–3: Integration & Validation

Ethos API staging

Orphan record checks

Term alignment verification

Canonical ID mapping

- Layer 4: Certified Views

Graduation rate by entry cohort

Retention (Fall → Spring persistence)

Credit velocity modeling

Section fill rate & demand metrics

Credential capture tracking

These views serve as the institutional “single source of truth.”

- Layer 5: Delivery

Power BI dashboards provide:

Executive aggregate view

Dean/program-level analytics

Student-success operational insights (role-based access)

Governance Principles Applied

No reporting logic embedded directly in dashboards

All calculations reproducible via SQL

Separation of staging logic from presentation layer

Small-cell suppression applied before publication

Metric definitions documented and version-controlled

---

Repository Structure
/docs
  Executive_Overview_Page1.docx
  Ethos_Architecture.pdf
  PowerBI_Dashboard_Summary.pdf

/sql
  certified_views.sql
  cohort_logic.sql
  retention_model.sql
  validation_checks.sql

/notebooks
  synthetic_data_generator.ipynb
Intended Audience

This prototype is structured for:

Institutional Research leadership

Academic Deans

IT Data Integration teams

Executive decision-makers

The emphasis is on governance maturity, definition clarity, and repeatable reporting structures.

---

### Closing Note

This repository is not intended to represent production institutional data. It is a structured demonstration of how higher education analytics can be implemented in a governed, sustainable, and decision-ready framework.
