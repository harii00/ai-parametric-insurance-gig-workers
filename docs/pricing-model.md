# Pricing Model - Raksha-Gig (Weekly Micro-Premium)

Raksha-Gig operates on a dynamic, data-driven pricing model designed for the financial reality of Indian gig workers.

## Weekly Logic

Traditional insurance uses monthly or annual premiums, which are ill-suited for' gig workers with fluctuating income. Our model is **Weekly**, aligning with delivery platform payout cycles.

### Premium Components

1. **Base Premium (₹30):** Fixed cost for system maintenance and base risk coverage.
2. **Dynamic Risk Factor (₹0 - ₹25):** 
    - **Weather:** Forecasted precipitation for the worker's zone.
    - **Traffic:** Historically high congestion periods.
    - **Platform stability:** Known maintenance windows for delivery partner apps.
3. **Worker Loyalty Discount (-₹5):** For workers with 4+ consecutive weeks of protection.

## Dynamic Pricing Calculation

The AI engine runs a weekly prediction:

```text
Premium = Base + (WeatherRisk * 0.4) + (CongestionRisk * 0.3) + (PlatformRisk * 0.3)
```

## Example Calculations (Begaluru)

### Scenario A: Dry Season (Low Risk)
- Base: ₹30
- Weather Forecast: 0% rain probability
- Traffic: Normal
- **Weekly Premium: ₹30**

### Scenario B: Monsoon Season (High Risk)
- Base: ₹30
- Weather Forecast: 80% heavy rain probability
- Traffic: High (Waterlogging impact)
- **Weekly Premium: ₹48**

## Claim Payout Structure

- **Daily Protected Payout:** ₹400 per event.
- **Weekly Cap:** ₹2,000 (Up to 5 events per week).
- **Payout Basis:** Minimum of 4 hours of "Loss of Income" window.
