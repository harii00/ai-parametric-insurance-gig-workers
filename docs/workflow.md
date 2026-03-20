# User Workflow & Journey - Raksha-Gig

This document details the end-to-end journey of a gig worker using Raksha-Gig.

## Journey Flow

### 1. Discovery & Onboarding
- **Sign-up:** Worker downloads the Raksha-Gig app or discovers it via the Swiggy/Zomato partner dashboard.
- **KYC & Linking:** Worker links their delivery ID. AI-verified profile is created.
- **Notification:** Worker receives a "Welcome Protection" notification.

### 2. Subscription Cycle
- **Monday Morning:** The weekly premium (e.g., ₹45) is calculated by the AI engine based on the weekly weather forecast.
- **Deduction:** The premium is deducted from the worker's weekend earnings or paid via UPI.
- **Active Status:** Policy becomes active for the week (Mon-Sun).

### 3. Real-time Monitoring
- **Trigger Check:** The system continuously monitors external APIs for the worker's registered zone.
- **Alerts:** If a high-risk event (e.g., heavy rain alert) is predicted, the worker receives a notification to exercise caution.

### 4. Trigger Event & Claim Settlement
- **Event Occurs:** A "Loss of Income" event is recorded (e.g., Cloudburst in North Delhi).
- **Auto-Verification:**
    - AI confirms the worker was "active" (online) during the event.
    - AI confirms Rainfall > threshold.
- **Instant Claim:** Notification: *"A Loss of Income event was detected in your zone. Your claim of ₹400 is being processed."*
- **Payout:** Funds hit the wallet within 24 hours.

### 5. Review & Renewal
- **Weekly Report:** Worker receives a summary of their protection and payouts at the end of the week.
- **Renewal:** One-click renewal for the next week.
