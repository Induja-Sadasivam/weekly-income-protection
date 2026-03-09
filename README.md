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
## Fraud Detection and Prevention

Since the system provides automated payouts, fraud prevention is essential.

The platform analyzes worker activity, GPS location, device usage, and historical behavior to detect suspicious patterns.

A fraud risk score is calculated for each worker during disruption events.

Fraud Score = 
(w1 × Activity Consistency Risk) +
(w2 × Location Authenticity Risk) +
(w3 × Device Integrity Risk) +
(w4 × Historical Behavior Risk)

If the fraud score exceeds a predefined threshold, the payout may be flagged for verification or temporarily blocked.
## Business Viability of Weekly Insurance Model

The weekly parametric insurance model is designed to match the income cycle of gig workers such as food delivery riders.

Since delivery workers earn income daily and plan expenses weekly, a small weekly premium makes insurance affordable and accessible.

The system maintains sustainability through:

• Affordable weekly premiums  
• Controlled maximum payout limits  
• Automated parametric triggers based on environmental data  

This model ensures that gig workers receive fast income protection during disruption events while maintaining financial stability for the platform.
## Automated Claim Process

The system automatically detects disruption events using a scheduler-based monitoring engine.

Environmental data is continuously retrieved from weather APIs and processed by the AI risk scoring model.

When the calculated risk score exceeds predefined thresholds, the parametric trigger engine automatically activates the payout process.

The payment system then transfers compensation to affected delivery workers and sends real-time notifications through the platform.
