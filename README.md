# RubiCon Media Tool – README
Day 2 in the starting of the prosject
![RubiCon Media Tool Screenshot](https://www.rubiconmedia.no/Skjermbilde%202025-07-18%20045255.png)
## Introduction

RubiCon Media Tool is a next-generation, modular Windows application for creative production powered by advanced artificial intelligence. The platform enables creators, developers, and designers to work seamlessly across image, video, 3D, code, website, and game modules—each managed independently for maximum flexibility and scalability.

Users interact with Rubi AI Chat, an intelligent language model that interprets commands and executes tasks directly within the application. The system is designed for professional workflows, supporting rapid prototyping, content generation, and collaborative development.

**Project Ownership:**
Developed and maintained by Cell Magic Limited (RubiCon Media).
Lead Developer & Company Owner: Tobias Hillstrand Østen
Contact: Tobias@rubiconmedia.no
Website: [www.rubiconmedia.no](https://www.rubiconmedia.no)

day 2 of the prosject
![RubiCon Media Tool Screenshot](https://www.rubiconmedia.no/Skjermbilde%202025-07-17%20234927.png)

# Join the Team & Help Launch RubiCon Media Studio AS
I’m looking for passionate developers to help build RubiCon Media Tool. Those who contribute and remain committed until the project's launch will be invited to co-found the new company: RubiCon Media Studio AS.

Founding Contributors Will Receive:
- Equity Ownership: The founder retains a majority stake, with the remaining portion fairly distributed among team members based on contribution and long-term commitment.
- Leadership Roles: Eligible for board membership, voting rights, and signature authority.
- Influence and Responsibility: A meaningful role in shaping the company’s future and recognition for your efforts.
  
My goal is to build a collaborative team where everyone is valued and has a real stake in what we create together.


If you are interested in joining, please contact support@rubiconmedia.no
![RubiCon Media Tool Screenshot](https://www.rubiconmedia.no/devteam.jpg)
---

## Project Structure

RubiConProject/
├── AI-Orchestrator/          # Interprets and distributes AI commands
├── Modules/                  # Functional tools (see below)
├── UserInterface/            # WPF GUI + Chat panel
├── Assets/                   # Local projects, databases, and files
└── README.md                 # This file

---
## Modules and Agents

Each module has its own folder and is managed by specialized agents:

- `RubiCode` → Generates, debugs, and documents source code
- `ImageGenerator` → Creates and edits images from text descriptions
- `ThreeDBuilder` → Models 3D objects with rigging and animation
- `WebsiteBuilder` → Builds frontend/backend code and layouts
- `GameEngine` → Designs game mechanics and logic with AI-driven NPCs

Each module includes:
## Rubi AI Chat

- Fetches module metadata
- Returns results to the GUI with explanations

The chat log also contains change history and a preview button for all commands.

---
- Each module has a defined file structure and lookup via `metadata.json`
- Rubi reads metadata before editing – never direct file writing
- Users can override AI choices by manually selecting files in the GUI

---
## Change Log and Version Tracking
This makes all work traceable and reversible.

## Compilation and Running

**Requirements:**

**Running:**

cd RubiConProject
python AI-Orchestrator/ai_router.py
dotnet build UserInterface/

## Update 2025-07-17
AI-Orchestrator and Theme-dev have been removed from the project. Use AI_Orchestrator for all backend.
See progress_status.md and logs/command_log.json for details about cleanup.
