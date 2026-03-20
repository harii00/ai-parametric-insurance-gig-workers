# API Integrations - Raksha-Gig

This document describes the external services required for the Raksha-Gig platform.

## 1. Weather Data (Live Trigger)
- **API:** [OpenWeatherMap - One Call API 3.0](https://openweathermap.org/api/one-call-3)
- **Used for:** Real-time rainfall measurement, temperature alerts, and 7-day forecasts for premium calculation.
- **Critical Threshold:** Precipitation (Rain/Snow) > 15mm in 3 hours.

## 2. Traffic & Geospatial Data
- **API:** [Google Maps Roads API](https://developers.google.com/maps/documentation/roads/overview) / [MapmyIndia API](https://www.mapmyindia.com/api/)
- **Used for:** Detecting zone-level congestion. If congestion > 200% of baseline, "Loss of Income" is validated for workers stuck in traffic.

## 3. Delivery Platform (Mock Integration)
- **Service:** Swiggy/Zomato Partner Webhooks (Mocked for Hackathon)
- **Used for:** Verifying the worker was logged "Online" but received "0 Orders" during the impact window.

## 4. Payment Gateway
- **API:** [Razorpay Payouts](https://razorpay.com/payouts/)
- **Used for:** 
    - Collecting weekly premiums via UPI/Auto-debit.
    - Releasing instant insurance payouts to bank accounts or digital wallets.

## 5. Air Quality Index (AQI)
- **API:** [AQICN (World Air Quality Index)](https://aqicn.org/api/)
- **Used for:** Monitoring extreme pollution levels in cities like Delhi/NCR to trigger "Hazardous Environment" protection.
