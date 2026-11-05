# CREATE PERMANENT PROJECT CONTEXT

We are building an Environmental Intelligence & Compliance Management System.



## PROJECT PURPOSE

A connected environmental platform that identifies developing environmental threats, predicts deterioration, communicates warnings and helps authorities investigate and track corrective action.

## ENVIRONMENTAL COVERAGE

1. Air pollution — PRIMARY FOCUS. Advanced PM2.5 forecasting, AQI monitoring, anomaly detection and early warnings.
2. Water pollution — Water-quality measurements, suspected contamination and investigation.
3. Unsafe waste disposal — Illegal dumping, open burning, citizen reports and image analysis.
4. Industrial emissions — Industrial stack emissions, effluent monitoring and compliance concerns.

Do not attempt to implement four equally advanced forecasting systems. Air pollution receives the most advanced ML capabilities.

## USERS

Citizen:
- Register and select preferred locality.
- Receive relevant free environmental warning emails.
- View public environmental conditions.
- Submit photographs and reports.
- Track personal reports.

Environmental authority:
- Access technical monitoring and predictions.
- Receive early-warning and critical emails.
- Review citizen reports and AI evidence.
- Examine environmental standards.
- Assign investigations and corrective actions.
- Track incidents.

Administrator:
- Manage accounts, authorities, monitoring stations, alert settings, data sources and models.

No paid subscriptions, premium plans, billing, paywalls or paid user access tiers.

## CORE COMPONENTS

1. Environmental Command Center.
2. Live Environmental Map and Historical/Future Timeline.
3. Predictive Environmental Intelligence.
4. AI Environmental Analyst.
5. Dual Citizen/Authority Email System.
6. Citizen and Field Evidence Reporting.
7. Central Risk and Alert Engine.
8. Incident and Compliance Center.
9. Simulation and Replay Engine.
10. Administrator and System Health capabilities.

## ML REQUIREMENTS

- XKDR India Air Quality Database for historical air-quality training.
- CPCB/data.gov.in for available current air-quality observations.
- Open-Meteo for meteorological information and forecasts.
- LightGBM PM2.5 regression models for +1h, +3h and +6h.
- Quantile forecasting for uncertainty.
- Calibrated LightGBM classifier for future deterioration probability.
- Robust MAD and Isolation Forest for anomaly detection.
- SHAP for model explanations.
- Pretrained vision model or appropriate YOLO model for visual environmental evidence.
- RAG and structured regulatory rules for compliance interpretation.

Use chronological training/validation/testing. Compare forecasting with a persistence baseline. Never invent evaluation metrics or prediction outputs.

## TECHNICAL STACK

Preferred:
- Next.js, React and TypeScript.
- Tailwind CSS.
- Supabase PostgreSQL, Authentication and Storage.
- PostGIS for geographical queries.
- Python and FastAPI for environmental ML services.
- LightGBM, Scikit-learn and SHAP.
- MapLibre or Leaflet.
- Recharts.
- Resend or another verified transactional email provider.

Inspect the repository before selecting compatible versions or introducing dependencies.

## DESIGN REQUIREMENT — NON-NEGOTIABLE

THE ENTIRE APPLICATION MUST USE A PREMIUM LIGHT THEME.

Use:
- White and soft off-white backgrounds.
- Dark navy/slate typography.
- Restrained teal and blue accents.
- Amber for warnings.
- Red for critical conditions.
- Light map tiles and clean geographical visualizations.
- Subtle borders, shadows and consistent spacing.

Do not build a dark dashboard or mix light and dark component styles.

Avoid excessive gradients, glowing effects, oversized cards and clutter.

## FUNCTIONALITY RULES

- Live data must originate from actual data sources.
- Historical records must be labelled as historical.
- Predictions must come from trained models.
- Simulations must be clearly labelled.
- Citizen photographs must actually be stored and linked to reports.
- Emails must be genuinely sent through the backend.
- Citizens and authorities must have separate permissions and email templates.
- Risk, severity, forecast probability, evidence confidence and regulatory compliance must remain separate.
- Critical alerts require validated observations or approved emergency criteria.
- Predictive alerts must not be presented as confirmed violations.
- Every important incident and authority action must have an audit history.

## DEVELOPMENT RULES

- Preserve existing working code.
- Work in small, independently testable phases.
- Never rewrite the whole application for a small feature.
- Do not create fake backend data or placeholder functionality.
- Do not modify unrelated files.
- Inspect dependencies before installing new packages.
- Run relevant tests after changes.
- Report changed files, tests and remaining problems.
- Use Git checkpoints before major phases.

Treat this file as the permanent specification. All future implementation prompts must follow it.
