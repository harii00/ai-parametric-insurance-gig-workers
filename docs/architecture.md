# System Architecture - Raksha-Gig

This document outlines the high-level architecture of the Raksha-Gig parametric insurance platform.

## Architecture Overview

Raksha-Gig uses a **decoupled, event-driven architecture** to monitor real-time environmental data and trigger automated insurance payouts.

### 1. Architectural Components

- **User Layer (Frontend):** A Next.js-based web app for gig workers. Features include policy management, real-time trigger status, and digital wallet integration.
- **Service Layer (Backend):** A Node.js/Express REST API that manages user authentication (Linked with Swiggy/Zomato), subscription handling, and policy lifecycle.
- **Data & Intelligence (AI Engine):** A Python-based service responsible for:
    - Ingesting weather, traffic, and platform status data.
    - Running risk prediction models for premiums.
    - Executing fraud detection algorithms on claims.
- **Oracle Layer:** A bridge between external APIs (Weather, GPS, Traffic) and the core parametric engine. This layer ensures that for every "trigger event," there is multiple-source validation.
- **Payout Engine:** An automated financial settlement service integrated with Razorpay/Stripe for near-instant disbursement.

## Data Flow

1. **Ingestion:** The Python service polls weather and traffic APIs every 30 minutes for specific worker clusters.
2. **Analysis:** The AI engine determines if any "Loss of Income" thresholds are met (e.g., Rainfall > 20mm).
3. **Validation:** If a threshold is hit, the system cross-references the GPS logs of active workers in that cluster.
4. **Trigger:** The parametric logic confirms an eligible event.
5. **Payout:** The Backend instructs the Payout Engine to release funds into the validated worker's wallet.

## Integration Points

- **Authentication:** OAuth for Swiggy/Zomato partner IDs.
- **Data Sources:** OpenWeatherMap API, Google Maps Traffic API.
- **Finance:** Razorpay Payouts API.
