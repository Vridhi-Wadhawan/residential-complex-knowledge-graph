# Design Approach, Scope, and Assumptions

This document outlines the **design rationale, scope boundaries, and modeling assumptions** used while creating the Residential Complex Digital Twin knowledge graph.

The focus is on **schema-level ontology design** for a modern residential complex, with emphasis on **automation, predictive maintenance, security, and community facilities**.

---

## Design Approach

### A. Brainstorming and Scope Definition

The design process began by identifying the core dimensions required to represent a realistic residential complex as a digital twin:

- **Building hierarchy:** residential complex, towers, floors, flats, rooms, zones
- **Automation and predictive maintenance:** equipment, sensors, alerts, maintenance tasks
- **Security and access management:** residents, visitors, security desk, access records
- **Facilities and amenities:** clubhouse, sports areas, marketplace, lawns

Clear scope boundaries were defined early to ensure the ontology remained **practical, interpretable, and extensible**, without unnecessary over-modeling.

---

### B. Preliminary Sketching

Before formal modeling, **paper-based sketches** were created to explore:

- Entity groupings and abstraction levels
- Relationship directions and hierarchy
- Whether facilities should exist at tower level or complex level

This step enabled rapid iteration and refinement before committing to a structured ontology model.

> Early-stage paper sketches were used to explore entity grouping and relationship direction before formalizing the ontology. Selected sketches are included in the repository as design artifacts, not finalized models.

---

### C. Reference Architecture Study

To ensure real-world alignment, publicly available **building automation and smart infrastructure reference architectures** were reviewed, with focus on:

- Intelligent lighting management systems
- HVAC and automated ventilation networks
- Elevator and pump room monitoring
- Fire safety, biometric access, and surveillance systems

These references helped validate that the ontology reflects **modern IoT-enabled Building Automation Systems (BAS)** commonly deployed in large residential complexes.

---

## Scope Definition

### In Scope

#### 1. Building Hierarchy
- Residential Complex → Buildings → Floors → Flats → Rooms → Zones
- Four towers with multi-storey layouts
- Common and tower-specific reception areas
- Multi-level parking facilities

#### 2. Automation & Predictive Maintenance
- Equipment: elevators, air conditioners, lighting systems, pumps, electrical panels
- Sensors: temperature, motion, energy, smoke, CCTV
- Alerts and maintenance tasks supporting predictive maintenance
- Intelligent lighting, HVAC control, and elevator management systems

#### 3. Security & Access Management
- Residents (owners or tenants)
- Visitors (maids, delivery personnel, guests)
- Security desk and access records
- Biometric access, surveillance, and fire safety systems
- Conceptual integration with a community access management app

#### 4. Facilities & Amenities
- Clubhouse, gym, library, banquet hall, lawns
- Indoor and outdoor sports facilities
- Marketplace with essential shops
- Facilities connected to relevant equipment and sensors

---

### Out of Scope

- Parking rented to external entities
- Religious or worship structures
- Detailed apartment interiors (furniture, appliances)
- Transport infrastructure (bus stops, cab stands)
- Real-time IoT data ingestion or live system deployment

---

## Assumptions

- The residential complex is **fictitious**
- Sensor data and automation signals are **simulated**
- The repository represents **conceptual ontology design only**
- All visitor access is logged via the security desk
- All facilities belong to a single digital twin ecosystem
- Relationship naming follows **RDF-inspired semantic conventions**

---

## References

- Public reference architectures for smart buildings and automation systems
- Industry documentation on IoT-enabled Building Automation Systems (BAS)
