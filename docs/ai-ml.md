# AI/ML Implementation - Raksha-Gig

Artificial Intelligence is the core of our "No-Manual-Claim" promise.

## 1. Risk Prediction Model

**Objective:** Calculate the dynamic weekly premium based on environmental risks.

- **Algorithm:** Random Forest Regressor.
- **Inputs:**
    - 7-day weather forecast (Rain, Heat, AQI).
    - Historical "Order Volume" dips in the specific zone during similar conditions.
    - Worker density in the zone.
- **Outcome:** A "Risk Score" (0.1 to 1.0) used to multiply the premium buffer.

## 2. Fraud Detection Techniques

To prevent payout manipulation (e.g., workers going offline just to trigger a payout), we use AI verification:

- **GPS Anomaly Detection:** Checks if the worker was actually in the "Impact Zone" during the trigger event.
- **Downtime Verification:** Cross-references "Loss of Income" claims with aggregate downtime reports from other workers in the same cluster. If 90% of workers in the cluster show no uptime during the event, the claim is 95% likely to be valid.

## 3. Threshold Logic (Parametric Engine)

The AI doesn't just look at absolute values; it looks at "Impactful Anomalies":

- **Rainfall:** > 15mm/3-hrs is the base. However, if the zone is prone to waterlogging (determined by historical topography maps), the threshold lowers to 10mm.
- **AQI:** Payouts trigger when AQI > 400 for more than 4 hours, acknowledging that outdoor food delivery is hazardous for the worker.

## Data Sources
- **Training Data:** 3 years of Bengaluru weather data + 1 year of mock delivery volume data.
- **Validation:** Live API feeds from OpenWeatherMap.
