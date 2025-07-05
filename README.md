# 🕸️ Spider-Verse Mini-World Database

A multiverse-spanning database system designed to organize and manage the world of Spider-People, villains, missions, and more. Built and normalized through various design phases and implemented via an interactive Python-MySQL interface.

## 👥 Team 50 - Systum

- **Prakhar Singhal** (2022111025)  
- **Chirag Dhamija** (2022101039)  
- **Mohak Somani** (2022101088)  
- **Samagra Bharti** (2022115007)

## 🌐 GitHub Repository

[🔗 Click here to access the repository](https://github.com/argamas23/Spiderverse-Mini-World-Database)

---

## 📌 Project Overview

The Spider-Verse Mini-World Database is a centralized system aimed at improving collaboration among Spider-People across dimensions by managing:

- Character data (Spider-People, Villains, Side Characters)
- Missions and outcomes
- Equipment and resources
- Organizational affiliations
- Research and discoveries
- Inter-dimensional relationships

---

## 📚 Project Phases

### 📍 Phase 1: Conceptualization

- Defined entities: Spider-Person, Villain, Mission, Organization, Side Character
- Designed relationships: mentorship, mission leadership, equipment ownership, etc.
- Proposed user base: Spider-People, scholars, law enforcement, dimensional councils

### 📍 Phase 2: ER Modeling

- Created an ER Diagram using min-max notation
- Added attributes and adjusted weak entities (like Equipment and Research Notes)
- Refined relationship names for clarity

### 📍 Phase 3: Relational Modeling and Normalization

- Developed a Relational Model and normalized up to **Third Normal Form (3NF)**
- Split multi-valued attributes (like abilities and participants) into separate relations
- Streamlined composite keys using surrogate identifiers

### 📍 Phase 4: Implementation

- Built a **Python-based CLI** using `pymysql`, `subprocess`, and `os`
- Created interactive command handlers for:
  - **Insertion**
  - **Deletion**
  - **Update**
  - **Projection**
  - **Aggregation**
  - **Search**
  - **Analytical Reporting**
  - **Free-form SQL execution**

---

## 💻 Functional Overview

### ✅ Supported Operations

| Operation     | Description                                                                 |
|---------------|-----------------------------------------------------------------------------|
| Insert        | Add Spider-People, Villains, Missions, Equipment, etc.                     |
| Delete        | Remove outdated or irrelevant data                                         |
| Update        | Modify entity data (Spider-People, Villains, etc.)                         |
| Search        | Find specific entries by ID (e.g., SpiderPerson's villains or missions)    |
| Project       | Display combinations (e.g., SpiderPeople and their abilities/equipment)    |
| Aggregate     | Perform calculations (e.g., average threat level of villains)              |
| Analyze       | Generate reports (e.g., mission success rates, villain confrontations)     |
| SQL Query     | Direct SQL query execution from user input                                 |

---

## 🧠 Analytical Reports

1. **Villain Opposition Network**: Analyze hero-villain interactions across dimensions.
2. **Mission Efficiency**: Compare Spider-People on successful mission completion.
3. **Equipment Utilization**: Track gadget usage across missions.
4. **Mission Complexity by Dimension**: Assess threat levels dimension-wise.

---

## 🧱 Technical Stack

- **Database**: MySQL
- **Backend**: Python with `pymysql`
- **Tools**: ERD design with dbdiagram.io, CLI-based CRUD system
- **Normalization**: Up to **3NF**
- **Image Handling**: Optional image table for dynamic runtime image mapping

---

## ⚠️ Assumptions & Notes

- Composite keys (e.g., SpiderIdentifier = Real Name + Dimension ID) are handled using surrogate keys in SQL.
- Apostrophes in strings must be escaped (`'` becomes `''`).
- Deletion and reinsertion are used for updating relationship tables to avoid anomalies.
- Primary keys are auto-incremented; deleted keys are not reused.
- Optional fields (e.g., mask names) can be set to `NULL`.

---

## 🚀 Getting Started

### Requirements

- Python 3.x
- MySQL Server
- Python packages: `pymysql`

### Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/argamas23/Spiderverse-Mini-World-Database.git
   cd Data-Applications
