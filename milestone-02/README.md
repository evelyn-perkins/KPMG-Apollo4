# Milestone 2: AI Business Intelligence & Process Design
**Project Track:** Track B — AI & Analytics  
**Client:** Wasatch Outfitters Collective (WOC)  

## 1. Current-State Workflow & Operational Bottlenecks
Based on our Milestone 1 exploratory data analysis of `woc_track_b_support.csv`, WOC's customer support operations suffer from severe structural friction due to multi-channel fragmentation:
* **The Asynchronous Lag:** Channels like **Email** (~316 tickets) and **Instagram DM** (~167 tickets) account for the vast majority of inbound volume but trap customers in average response times exceeding **23.5 to 24.6 hours**.
* **Synchronous Advantage:** High-intent channels like **Phone** (~244 tickets) and **Web Form** (~73 tickets) achieve rapid resolution times averaging **~2 hours**, yet lack a unified handoff or tracking mechanism with asynchronous touchpoints.
* **Operational Impact:** Siloed communication leads to lost customer history, agent burnout, and inconsistent policy enforcement (specifically observed in split resolutions for **Late Fee Disputes**).

## 2. Centralized CRM Strategy
To eliminate data silos and establish a single source of truth across all retail locations (Downtown SLC, Sandy, and Park City), WOC must implement a unified CRM architecture:
* **Omnichannel Unified Inbox:** Consolidate Email, Instagram DMs, SMS, and Web Forms into a single shared queue so staff have a complete 360-degree view of member rental history and past inquiries.
* **Cross-Channel Tracking:** Automatically attach customer profiles to incoming inquiries to eliminate redundant questioning when a customer switches from social media to phone support.

## 3. AI-Enabled Triage & Deflection Architecture
To combat the ~24-hour backlog on asynchronous channels, we propose deploying an AI-enabled triage layer at the ingestion point:
* **Automated Intent Classification:** Instantly parse incoming inquiries using Natural Language Processing (NLP) to categorize requests by primary drivers (**Rental Availability**, **Class Registration**, **Gear**, and **Repair Status**).
* **Tier-1 Deflection & Self-Service:** Automatically resolve routine inquiries—such as real-time gear rental availability or ski class schedule lookups—via an automated chatbot or instant email/DM response template.
* **Standardized Policy Enforcement:** Embed WOC business logic directly into the AI knowledge base to ensure uniform handling of edge cases, such as automated validation and consistent decision-making for **Late Fee Waivers**.

## 4. Expected Business Impact
* **Resolution Time Reduction:** Cut asynchronous response times from ~24 hours down to near-instantaneous triage for tier-1 inquiries.
* **Staff Reallocation:** Shift human agents away from repetitive status checks and toward high-value physical retail consultations, gear maintenance, and complex escalations.