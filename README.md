# Bosch Rexroth AG 
## Predictive Maintenance Strategy

## Project Overview

This project analyses hydraulic system performance across 10 Bosch Rexroth AG machines (HPU_01 to HPU_10) using multi sensor telemetry, failure logs, maintenance records, and equipment metadata. The objective is to identify failure patterns, evaluate sensor health, assess Remaining Useful Life (RUL), and quantify the financial and operational impact of the current maintenance strategy.

Three dashboards were developed to provide visibility into failure dynamics, sensor behaviour, and cost saving opportunities. The insights support Bosch Rexroth AG’s transition from reactive to predictive maintenance.

## Collaboration and Project Team

This analysis was delivered through a cross functional collaboration involving:
- Business Analysts: defining business questions, aligning KPIs, validating operational relevance
- Data Scientists: modelling RUL, analysing sensor behaviour, identifying anomaly patterns
- Project Management Team: coordinating scope, timelines, stakeholder requirements, and delivery

This multidisciplinary approach ensured that the insights were technically sound, operationally relevant, and strategically aligned with Bosch Rexroth AG’s maintenance objectives.

## Dataset Source

All datasets used in this project were provided directly by Bosch Rexroth AG for internal operational analysis. They include:
- Sensor telemetry
- Failure events and downtime logs
- Maintenance actions and component replacements
- Equipment metadata
- Daily operating hours and anomaly counts

These datasets reflect real machine behaviour and operational conditions.

## Data Quality Validation

Before analysis, all datasets were reviewed to ensure accuracy and consistency. Validation checks confirmed:
- Machine records aligned correctly across telemetry, failure logs, and maintenance history
- Operating hours and anomaly counts followed expected patterns
- Failure events and maintenance actions were complete and correctly attributed
- Sensor telemetry was consistent enough to support RUL estimation and anomaly analysis

These checks ensured that the insights and dashboards were built on reliable, high‑integrity data.

## Tools Used

The analysis and dashboards were developed using:
- PgAdmin (PostgreSQL): for data validation, integration, and time‑series preparation
- Power BI: for dashboard development, KPI modelling, and visual insights

## Dashboards

### Failure and Maintenance Overview Dashboard

Shows failure modes, downtime hours, maintenance frequency, and machine‑level health indicators.

<img width="507" height="284" alt="Screenshot 2026-06-04 162249" src="https://github.com/user-attachments/assets/1df0b06e-b0d1-4bd6-9c92-91610923e8d8" />

### Sensor Health and Predictive Insights Dashboard

Analyses anomaly rates, sensor dropouts, RUL estimates, fluid performance, and blind failure detection.

<img width="501" height="293" alt="Screenshot 2026-06-04 162402" src="https://github.com/user-attachments/assets/cdf9f0b3-4a49-4396-94e0-af50b5c2edaa" />

### Financial and Operational Impact Dashboard

Quantifies cost avoidance, repair cost reduction, spare‑parts optimisation, and asset end‑of‑life risk.

<img width="503" height="286" alt="Screenshot 2026-06-04 162455" src="https://github.com/user-attachments/assets/6c93c4aa-c601-4976-8d84-f82070d04b6d" />

## Exploratory Data Analysis

Financial and Resource Optimisation
- Reducing 106.7 hours of downtime by 30 to 50% yields $133K to $222K in cost avoidance.
- RUL‑based alerts can reclaim 15 to 20% of technician hours ($22K labour savings).
- Emergency spare to parts premiums can be reduced by 25% with ±8‑hour RUL accuracy.

Failure Dynamics and Reliability
- Several machines experienced failures despite showing no anomaly activity → blind failures.
- Each machine recorded 259 sensor dropouts, correlating with unlogged failures.
- Pump wear is the highest cost failure mode.
- Synthetic fluid shows significantly lower anomaly rates than mineral oil.
- Preventive actions consistently extend RUL compared to reactive repairs.

Asset Lifecycle
- HPU_08 has exceeded the end‑of‑life threshold with 24,309 operating hours.
- Other machines (HPU_07, HPU_10) remain within healthy ranges.

## Key Insights

- Pump wear is the most financially critical failure mode.
- HPU_08 is the highest risk asset in the fleet.
- Pressure is the earliest and most reliable early warning sensor.
- Synthetic fluid significantly improves machine reliability.
- Reactive maintenance (30%) exceeds the 20% business target.
- Emergency spare‑parts premiums can be reduced by 25%.
- Predictive maintenance can reduce downtime by 30 to 50%.

## Recommendations

1. Implement pressure based alert thresholds
Pressure degradation provides the earliest indication of failure and should trigger preventive actions.

2. Prioritise HPU_08 for immediate intervention
High operating hours and anomaly activity make it the most critical asset.

3. Expand the use of synthetic fluid
Synthetic fluid demonstrates superior reliability and should be adopted more widely.

4. Reduce reactive maintenance from 30% to 20%
Use RUL predictions to convert reactive events into scheduled interventions.

5. Introduce proactive seal replacement
Seal failures are predictable and ideal for preventive scheduling.

6. Strengthen sensor health monitoring
High dropout rates indicate the need for calibration or firmware updates.

7. Integrate RUL predictions into CMMS workflows
Maintenance teams should receive alerts with at least 10 hours of lead time.

## Business Impact

Implementing these recommendations will enable Bosch Rexroth AG to:
- Reduce downtime by up to 50%
- Improve machine reliability and extend asset life
- Lower emergency repair and spare‑parts costs
- Increase technician productivity
- Strengthen predictive maintenance readiness
- Support long term Industry 4.0 scalability

