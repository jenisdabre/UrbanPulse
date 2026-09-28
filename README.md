# UrbanPulse

**Smart India Hackathon (SIH) 2026**

UrbanPulse is a real-time city intelligence platform for Mumbai. City buses act as mobile witnesses, citizens confirm what they see, and AI turns both into verified, actionable insight for road safety, traffic and civic repair, while keeping raw data private through edge AI and federated learning.

## Problem Statement

* **Problem Statement ID:** 26124
* **Title:** AI-Powered Mobile Urban Intelligence Platform Using Public Transport Fleet
* **Organization:** Bharat Electronics Limited (BEL)
* **Category:** Software
* **Theme:** Smart Automation

Public transport buses travel almost every major road in a city every day, and many are already fitted with front, rear, side and cabin cameras. Yet those cameras are used only for recording, while city authorities still depend on fixed CCTV, manual inspections and citizen complaints. This leads to delayed response, incomplete situational awareness and inefficient maintenance planning.

UrbanPulse turns the bus fleet into a mobile urban sensing network. Edge AI on each bus detects road defects, estimates traffic density, flags vulnerable pedestrian situations and tracks offending vehicles, while a central platform aggregates everything on a GIS map with congestion heat maps, origin-destination analysis and route-delay insights for transport authorities. Detection is closed out with citizen confirmation and repair verification.

## Key Features

### AI-Powered Mobile Urban Sensing

- Public transport buses act as mobile sensing units using onboard cameras
- Continuous city-wide monitoring without relying only on fixed CCTV infrastructure

### Road Hazard Detection

- Detects potholes, damaged roads, missing road dividers, faded zebra crossings
- Identifies damaged or missing traffic signboards, waterlogging, and other road hazards

### Traffic Monitoring and Analytics

- Vehicle detection, classification, and counting
- Traffic density estimation and congestion hotspot identification
- Route delay estimation and traffic bottleneck analysis

### Vulnerable Pedestrian Safety

- Detects high-risk pedestrian situations
- Special focus on school zones and pedestrian crossings

### Incident Detection and Vehicle Tracking

- Detects rash driving and hit-and-run incidents
- Tracks offending vehicles across multiple observations
- Extracts vehicle registration numbers using OCR with confidence scores

### GIS-Based Urban Intelligence Dashboard

- Visualizes incidents, hazards, and traffic events on an interactive GIS map
- Generates congestion heatmaps and road condition maps

### Infrastructure Deficiency Monitoring

- Identifies missing or damaged public infrastructure
- Supports proactive maintenance planning for city authorities

### Fleet-Wide Data Aggregation

- Combines observations from multiple buses across the city
- Provides a comprehensive and continuously updated urban view

### Actionable Decision Support

- Generates alerts, reports, and insights for transport authorities
- Enables evidence-based traffic management and urban planning

## Unique Selling Propositions (USP)

### Bus as a Witness

- Multiple independent bus camera observations of the same incident
- Timeline, vehicle/event tracking, and registration/OCR information

### Repair Verification

- Full lifecycle tracking: Detected → Reported → Repaired → Re-observed → Verified
- Passing buses automatically verify completed repairs

### Citizen Reporting (See It, Report It)

- GPS-enabled reporting with photos and issue categorization
- Automatic duplicate detection and issue consolidation

### Ask the City

- Natural language city analytics queries
- Hindi and Marathi language support
- Voice-based interaction

### AI, Privacy and Federated Learning

- Edge AI processing directly on buses
- Privacy-first architecture
- Federated learning improves models without transferring raw data


## Tech Stack

**Frontend:** React, TypeScript, Vite, Tailwind CSS, Leaflet / React-Leaflet, Recharts

**Backend:** Node.js, Express, Drizzle ORM

**Tooling:** pnpm workspaces (monorepo)

## Project Structure

```
artifacts/
  urbanpulse/       # Main frontend app (Vite + React)
  api-server/       # Backend API (Express)
  mockup-sandbox/   # Design/prototyping sandbox
lib/                # Shared libraries
scripts/            # Workspace scripts
```

## Installation

**Prerequisites:** Node.js (LTS) and pnpm (`npm install -g pnpm`)

```bash
# 1. Clone the repository
git clone https://github.com/YOUR-USERNAME/UrbanPulse.git
cd UrbanPulse

# 2. Install dependencies
pnpm install
```

> \\\*\\\*Windows users:\\\*\\\* if `pnpm install` fails on the `preinstall` script (`'sh' is not recognized`), use Git Bash, or run `pnpm install --ignore-scripts`.

### Run the frontend

```bash
cd artifacts/urbanpulse
```

Set the required environment variables, then start the dev server:

**macOS / Linux / Git Bash**

```bash
PORT=5173 BASE\\\_PATH=/ pnpm dev
```

**Windows PowerShell**

```powershell
$env:PORT=5173
$env:BASE\\\_PATH="/"
pnpm dev
```

Open http://localhost:5173/

### Run the backend (optional)

See `.env.example` for required variables (such as database URL), then:

```bash
cd artifacts/api-server
pnpm dev
```

## Team UrbanPulse

* Trisha Deshmukh
* Sanika Mane
* Shravani Joshi
* Bliss Gonsalves
* Shravani Kolekar
* Jenis Dabre



## Institution

St. Francis Institute of Technology (SFIT), Mumbai

## Hackathon

Smart India Hackathon (SIH) 2026

> "Turning every bus, citizen and road into a sensor for a safer city."



