# SafeRoad+ — Intelligent Road Safety System

A software engineering term project designing an intelligent road safety system that improves driving safety through real-time traffic alerts and automatic accident detection. Developed using the Incremental Development Model, with full UML documentation from requirements through architecture.

## Overview

SafeRoad+ uses GPS and sensor data to monitor road conditions and driver behavior, identifying potential hazards in real time. When a risk or incident is detected, the system instantly notifies nearby drivers and emergency authorities — aiming to reduce accidents, enhance driver awareness, and support faster emergency response.

**Development Model:** Incremental Development Model — chosen to allow the system to be built step by step, with each increment adding features such as reporting, live maps, automatic detection, and SOS alerts, reducing risk and delivering value early.

## Core Features

- **Report Accident** — manual accident reporting with automatic location capture (GPS or manual fallback)
- **Send SOS Alert** — emergency alert to authorities with driver and vehicle data attached
- **View Live Map** — real-time interactive map showing traffic, hazards, and accident reports
- **Request Safe Route** — route recommendations that avoid hazards, closures, and poor weather conditions
- **Send Road Suggestions / Update Road** — integration endpoints for the Map System to exchange live road data

## Requirements

**Functional (selected):**
- Real-time notification of nearby incidents to drivers
- Live traffic and road condition display on an interactive map
- Alternative safe-route suggestions based on live hazard data

**Non-Functional:**
- **Performance:** alerts processed and delivered within 3 seconds
- **Reliability:** 99% uptime, 24/7 availability
- **Security:** all transmitted data encrypted using secure protocols
- **Usability:** bilingual interface (Arabic and English)

## System Design

The project includes full UML documentation:

- **Context Diagram** — SafeRoad+'s interactions with the Driver, Map System, Weather API, and Emergency Authority System
- **Use-Case Diagram** — 8 use cases covering account management, reporting, alerts, mapping, and routing
- **System Class Diagram** — core classes: `Driver`, `SafeRoadSystem`, `EmergencyAuthoritySystem`, `WeatherAPI`, `MapSystem`, `SOSAlert`, `Route`
- **Sequence Diagrams** — detailed message flows for Report Accident, Send SOS Alert, View Live Map, and Send Road Suggestions
- **Activity Diagrams** — step-by-step logic for key use cases, including error and edge-case paths
- **State Diagram** — state transitions for the accident-reporting lifecycle (Idle → Getting Location → Filling Form → Submitting → Confirmed)
- **Architecture Diagram** — 3-tier structure: UI layer, Authentication & Business Logic layer, and Data/Infrastructure layer

## Tech / Method

- **UML** (context, use-case, class, sequence, activity, and state diagrams)
- **Incremental Development Model**
- External system integrations: Map System, Weather API, Emergency Authority System

## What This Project Demonstrates

- Translating a real-world safety problem into functional and non-functional requirements
- Full software design lifecycle — from context diagram through architecture
- Modeling system behavior under both normal flow and failure conditions (network loss, GPS unavailable, permission denied)
- Applying an incremental development methodology to manage risk and scope

## References

- Larman, C. (2004). *Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development* (3rd ed.). Pearson Education.
- Sommerville, I. (2016). *Software Engineering* (10th ed.). Pearson Education.

## Team

Developed as a group project for the Software Engineering (CS 385) course at Princess Nourah bint Abdulrahman University.
