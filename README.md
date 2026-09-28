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

### City Overview

* Live Mumbai GIS map with active buses, incidents, road hazards, congestion and pedestrian safety
* Live alerts and clickable incident markers

### Incident Detection and Details

* Location, severity, timestamp and detection information for each incident
* Community confirmation (for example: 30 citizens + 4 buses confirmed this)

### Bus as a Witness

* Multiple independent bus camera observations of the same incident
* Timeline, vehicle/event tracking and registration/OCR information

### Repair Verification

* Full lifecycle: Detected, Reported, Repaired, Re-observed, Verified
* Re-observation by passing buses confirms repairs without manual follow-up

### Citizen Reporting (See It, Report It)

* GPS capture, issue category and photo-based reporting
* Duplicate matching and consolidation with existing issues

### Ask the City

* Natural-language questions such as "Which areas currently have the highest number of road hazards?"
* Hindi and Marathi support and voice interaction

### City Intelligence

* Traffic analytics, congestion, road conditions, route delays
* Origin-Destination (OD) analysis and heatmaps

### AI, Privacy and Federated Learning

* Edge AI for on-device processing
* Privacy-first design
* Federated learning: models improve across the city without raw data leaving local devices

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



