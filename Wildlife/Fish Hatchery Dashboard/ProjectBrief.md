# 🐟 Project Brief: Fish Hatchery Dashboard
| Key Detail | Information | 
| :---------: | :-------- | 
| Status |  Discovery / Research Phase | 
| Area of Interest | Wildlife & Environment |
| Lead AoI Commission | [Open / Seeking Leads] |

1. **Executive Summary:**
Managing a fish hatchery involves tracking a massive amount of moving parts: water chemistry, feed schedules, growth rates, and regulatory compliance. Currently, much of this is done via paper logs or fragmented spreadsheets.
The Fish Hatchery Dashboard is an open-source, centralized platform designed to help hatchery managers and staff visualize their data in real-time and automate the process of generating weekly and annual permit-compliance reports.
2. **The Problem**
 * Data Silos: Information on water flow, feed, and fish mortality is often kept in different places, making it hard to see the "big picture."
 * Manual Reporting: Staff spend hours every month manually compiling data to meet Idaho Department of Environmental Quality (DEQ) or EPA requirements.
 * Risk Management: Without real-time visualization, it’s harder to spot trends (like a slow drop in oxygen) before they become a crisis.
3. **Core Features (The MVP)**
To get this off the ground, we are focusing on three main Pillars:
* A | The Data Entry Hub
    * Simple mobile-friendly forms for technicians to log daily water temps, dissolved oxygen (DO), and pH.
    * Feed tracking (logging how many pounds of which feed type went into which raceway).
* B | Analytics & Visualization
    * A "Health at a Glance" dashboard showing current conditions across all raceways.
    * Growth charts comparing actual fish growth vs. projected growth models.
* C | The "Magic Report" Button
    * Automated generation of discharge monitoring reports (DMRs) based on logged data, formatted to meet standard regulatory templates.
   
4. **Technical Architecture**
We aim for a "Modular Monolith" approach so hobbyists of all levels can contribute to different parts of the stack.
 * Frontend: React or Vue.js (Focus on clean, high-contrast UI for outdoor/tablet use).
 * Backend: Python (FastAPI or Flask) — ideal for the heavy data processing and math required for aquaculture.
 * Database: PostgreSQL (to handle relational data like Species -> Raceway -> Feed Log).
 * Calculations: Implementation of aquaculture-specific math like Lindeberg’s Growth Model and FCR (Feed Conversion Ratio).
5. **User Personas**
 * The Technician: Needs to input data quickly with wet hands on a tablet. Speed and "fat-finger" friendly UI are key.
 * The Manager: Needs to see trends over the last 30 days and export reports for the front office.
 * The Biologist: Needs to analyze mortality rates and feed efficiency to optimize fish health.
6. **Success Metrics**
 * Reduction in Paper: Does this replace at least two physical logbooks?
 * Time Saved: Does the monthly reporting time drop from 4 hours to 10 minutes?
 * Accuracy: Does the software accurately predict when a raceway will hit its "carrying capacity"?
7. **How to Help**
Check the #aoi-wildlife channel in Discord! We currently need:
 * Researchers: To find specific Idaho DEQ reporting templates.
 * UI/UX Designers: To wireframe the "Daily Log" mobile view.
 * Backend Devs: To help architect the database schema for raceways and batches.

# 🐟 Project: Fish Hatchery Dashboard
## Issue #1: Research - Local Hatchery Directory
 * Difficulty: Beginner (Non-coding)
 * The Task: We need a comprehensive list of Idaho-based fish hatcheries (state, federal, and private) to use as our "customer" personas.
 * Deliverable: Create a Markdown file in /research/hatcheries.md listing the name, location, and types of fish raised at at least 10 Idaho hatcheries.
 * Why it matters: This helps us understand who will actually use the dashboard.
## Issue #2: Design - Feed Conversion Formula Docs
 * Difficulty: Intermediate (Math/Logic)
 * The Task: Research and document the standard formulas for "Feed Conversion Ratio" (FCR) used in aquaculture.
 * Deliverable: Add a section to /design/logic.md explaining the math. Use LaTeX if possible, e.g., FCR = \frac{\text{Total Feed Fed}}{\text{Weight Gained}}.
 * Why it matters: Our developers need the math before they can write the code.
## Issue #3: Frontend - Dashboard "Mockup" (HTML/CSS)
 * Difficulty: Beginner/Intermediate (Coding)
 * The Task: Create a simple, static HTML page that shows what a "Hatchery Overview" might look like. Include placeholders for "Water Temperature," "Oxygen Levels," and "Current Biomass."
 * Deliverable: A single index.html file in /src/ui-prototype.
 * Why it matters: It gives the team something visual to get excited about!
