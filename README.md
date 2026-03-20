# 🛡️ Raksha-Gig: AI-Powered Parametric Insurance for Indian Gig Workers

### "Securing Every Delivery, One Drop at a Time"

---

## 📌 Problem Statement
The Indian gig economy, led by food delivery platforms like **Zomato** and **Swiggy**, employs over 7.7 million workers. These delivery partners face significant financial vulnerability due to **Loss of Income** caused by unpredictable external factors like extreme weather, server outages, or traffic congestion. Current insurance products are either too expensive, complex, or slow to payout.

## 👤 Persona Description
**Meet Rajesh:** A 28-year-old Swiggy delivery partner in Bengaluru. He supports a family of four. If it rains heavily or the app goes down, he loses his daily earnings (~₹800). He cannot afford a monthly ₹1,000 premium, but he can spare ₹50 a week for peace of mind.

## 💡 Solution Overview
**Raksha-Gig** is a parametric insurance platform that automatically triggers payouts when specific "Loss of Income" events occur. 
- **No manual claims:** Data feeds trigger payments.
- **Weekly micro-premiums:** Scaled for the gig worker's wallet.
- **AI-driven risk assessment:** Personalized pricing based on location and historical trends.

## 🚀 Key Features
- **Automated Payouts:** Instant transfer to worker's wallet upon event confirmation.
- **Dynamic Weekly Pricing:** Premiums adjust based on forecasted weather and city-specific traffic risks.
- **Low Friction Onboarding:** One-click integration with delivery partner apps.
- **Transparency:** Real-time tracking of triggers and policy status.

## 🔄 Workflow
1. **Onboarding:** Rajesh links his Swiggy/Zomato ID to Raksha-Gig.
2. **Weekly Subscription:** ₹45 is deducted from his weekly earnings on Monday.
3. **Monitoring:** Our AI monitor tracks weather (Rainfall > 20mm) and server status.
4. **Trigger Event:** On Thursday, Bengaluru experiences a sudden cloudburst.
5. **Auto-Payout:** AI confirms Rajesh was online but couldn't deliver. ₹400 (50% of daily average) is credited to his account by Friday morning.

## 💰 Weekly Pricing Model
*Example Scenario (Phase 1):*
- **Base Premium:** ₹30/week
- **Weather Surcharge (Monsoon):** +₹15/week
- **Total:** ₹45/week
- **Maximum Payout:** ₹2,000 per week for identified "Loss of Income" days.

## ⚡ Parametric Triggers
1. **Rainfall Threshold:** Precipitation > 15mm in a 3-hour window.
2. **Extreme Temperature:** Heatwaves (> 42°C) or extreme cold.
3. **Platform Server Outage:** Documented downtime of Swiggy/Zomato partner apps > 2 hours.
4. **AQI (Air Quality):** AQI > 400 (Hazardous), restricting safe outdoor movement.

## 🧠 AI/ML Integration
- **Risk Predictive Model:** Predicts high-risk weeks using historical weather data to adjust premiums.
- **Fraud Detection:** Cross-references GPS logs with reported "Loss of Income" triggers to ensure the worker was actually active.

## 🏗️ System Architecture
- **Frontend:** Next.js Dashboard for workers.
- **Backend:** Node.js/Express API handling subscriptions and logic.
- **Data Engine:** Python service consuming Weather (OpenWeather) and Traffic APIs.
- **Smart Payouts:** Automated ledger for instant claim settlement.

## 🛠️ Tech Stack
- **Frontend:** React, Tailwind CSS
- **Backend:** Node.js, MongoDB
- **AI/ML:** Python (Scikit-learn, Pandas)
- **APIs:** Razorpay (Payments), OpenWeatherMap, Google Maps (Traffic)

## 📅 Development Roadmap (6 Weeks)
- **Week 1:** Data collection & Persona validation.
- **Week 2:** Parametric engine logic development.
- **Week 3:** AI Risk model training (Mock data).
- **Week 4:** Frontend worker dashboard.
- **Week 5:** API integrations & Backend stress testing.
- **Week 6:** Pilot launch & Demo video.

## 🌟 Innovation Highlights
- **Zero-Claim Interface:** Eliminates the mental burden of paperwork for workers.
- **Hyper-Local:** District-level triggers using geo-fencing.
- **Financial Inclusion:** Targeted specifically at the "under-insured" gig worker segment.

## 📽️ Demo Video
[Link to Demo Video coming soon...]

## 👥 Team Details
- **Lead Architect:** [Your Name/Team Name]
- **AI Engineer:** [Placeholder]
- **Frontend Guru:** [Placeholder]
