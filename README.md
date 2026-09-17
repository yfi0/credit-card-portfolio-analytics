# Credit Card Portfolio Analytics

An evolving analytics portfolio project focused on credit-card portfolio monitoring, consumer-credit behavior, and credit-risk analysis using synthetic data.

## Project objective

Build a reproducible credit-card portfolio dataset and analytics workflow that can support portfolio KPIs, utilization and delinquency monitoring, customer segmentation, and later extensions such as roll-rate and vintage analysis.

## Current version: V0.1 — Portfolio foundation

V0.1 establishes the data model, synthetic-data generator, validation controls, data dictionary, and initial SQL analytics layer. The first BI presentation layer will be built in Tableau, with a later Power BI/DAX rebuild planned as an extension.

## Planned architecture

`Synthetic Data → Python / SQL Analytics → Tableau → later Power BI`

The project separates relatively stable account characteristics from monthly account performance so behavior can be analyzed over time rather than only as a current snapshot.

## Planned repository structure

```text
credit-card-portfolio-analytics/
├── README.md
├── data/
├── python/
├── sql/
├── docs/
└── dashboard/
```

## Data transparency

All customer and account records in this repository are synthetic. Simulated distributions and relationships are project assumptions created for analytical practice and do not represent a real financial institution or claim to reproduce industry portfolio benchmarks.

The synthetic-data design will favor probabilistic relationships rather than deterministic rules. For example, higher utilization or lower FICO may be associated with higher simulated credit risk, but neither will automatically determine a customer's outcome.

## Development approach

This repository will be developed through meaningful versions rather than waiting for the entire roadmap to be complete:

- **V0.1:** portfolio foundation and reproducible synthetic data
- **V0.2:** validation and core portfolio KPI / SQL layer
- **V0.3:** Tableau portfolio dashboard
- **V0.4:** delinquency migration, roll-rate, and vintage analysis
- **Later:** underwriting strategy, Power BI/DAX migration, and optional data-engineering or predictive extensions

Documentation will distinguish assumptions from findings and will be updated as the implementation evolves.
