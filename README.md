# Weekly Income Protection System

## Problem Statement
## Selected Persona
Peak-Hour Dependent Urban Food Delivery Rider (Bike-Based, Tier-2 City)
## Income Loss Model
## Parametric Trigger Model
## Peak-Hour Optimization Logic
## System Architecture (Initial)
The system collects environmental data from weather APIs, air quality APIs, and flood alert systems.

This data is processed by an AI risk scoring engine to evaluate the probability of delivery disruption.

If the risk crosses a predefined threshold, the parametric trigger engine automatically activates a payout.

The delivery worker receives compensation through the platform without submitting a manual claim.
## Initial System Flow

See diagrams in /diagrams folder:

- User Journey Diagram
- Problem Flow Diagram
## Weekly Pricing Model

The system uses a micro-insurance weekly premium designed for gig workers.

Base Premium: ₹100 per week

Risk Multiplier:
Low Risk → ₹100  
Medium Risk → ₹130  
High Risk → ₹160

Weekly Premium Formula:

Weekly Premium = Base Premium × Risk Multiplier

Example:
Low Risk Week = ₹100 × 1.0 = ₹100
High Risk Week = ₹100 × 1.6 = ₹160

Maximum payout per disruption event: ₹500
## AI Risk Scoring Model

The system evaluates environmental risk using multiple indicators.

Risk Score =
(w1 × Rainfall Severity) +
(w2 × Temperature Severity) +
(w3 × Pollution Severity) +
(w4 × Flood Alert Indicator)

Risk Score Levels

Low Risk → Normal operations  
Moderate Risk → Possible disruption  
High Risk → Significant disruption  
Critical Risk → Automatic payout triggered
