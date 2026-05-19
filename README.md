# region_id

# Q2 2026 ML Forecasting Project

This repository is for standardizing forecasting for Wise WFM across Business Units.
The immediate goal is to evaluate how existing forecasting approaches can be reused or adapted for KYC, then extend the same operating model to other Business Units where forecasting is not yet standardized.

## Scope

- Short-term forecasting (intraday)
- Mid-term forecasting
- Workload forecasting
- Staffing forecasting

## Business Units

- CS
- KYC
- FinCrime
- Payment Ops
- Customer Advocacy

## Current Operating Assumptions

- CS already has an existing forecast model.
- Payment Ops already has an existing forecast model.
- KYC is the first priority area for extension and validation.
- Demand Management is the primary stakeholder.
- SS Tooling Team owns the Calabrio WFM system.
- Data is sourced from Snowflake, persisted in Snowflake, orchestrated with Airflow, and managed in GitHub.

## Repository Layout

- `thinking/`: Japanese-first exploratory notes, assumptions, investigations, and open questions
- `decisions/`: English decision records and final judgments
- `docs/`: English project documentation for review and reuse
- `data_contracts/`: input and output definitions across Snowflake and Calabrio boundaries
- `configs/`: common and Business Unit-specific configuration
- `sql/`: Snowflake extraction and transformation queries
- `src/`: implementation code and future shared modules
- `reference_implementations/`: imported reference assets from existing Business Unit forecasting implementations
- `tests/`: automated validation and regression checks
- `notebooks/`: exploratory analysis and model evaluation notebooks
- `outputs/`: output samples and interface examples
- `runbooks/`: Airflow and operational procedures

## Language Rules

- Use Japanese for exploratory thinking and temporary internal notes.
- Use English for documents that are intended for review, reuse, handover, or stakeholder communication.

See `AGENT.md` for repository operating rules.
