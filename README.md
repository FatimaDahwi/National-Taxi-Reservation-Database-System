# National Taxi Reservation Database System

### Course Information
* **Course:** CSCI335 - Database Systems
* **Instructor:** Dr. Bilal Kanso
* **Developer:** Fatima Dahwi
* **Institution:** Lebanese International University (LIU)

---

## 📋 Project Overview
This database system is designed to optimize and enhance the taxi reservation ecosystem across the country[cite: 1]. The platform provides a centralized, user-friendly infrastructure allowing clients to seamlessly browse available taxi companies, reserve ideal vehicles based on capacity/model, and get assigned verified drivers. 

The primary goal is to bridge the gap between taxi companies, branches, independent car owners, drivers, and clients to ensure highly efficient coordination and data integrity.

---

## 🛠️ Tech Stack & Tools
* **Modeling & Design:** ERDPlus (for Entity-Relationship Diagramming & Relational Mapping)
* **RDBMS Engine:** Microsoft SQL Server
* **Management Interface:** MS SQL Server Management Studio (SSMS)
* **Normalization Target:** Third Normal Form (3NF)

---

## 🗺️ System Architecture

### 1. Entity Relationship Diagram (ERD)
The system logic establishes deep tracking between central hubs (Taxi Companies), regional operations (Branches), assets (Taxi Cars), workforce (Drivers/Staff), and service requests (Reservations/Trips).

### 2. Core Entities & Attributes Breakdown
* **Taxi Company:** The primary administrative entity tracking the enterprise's corporate identity (`companyNb`, `CompanyName`, `foundingDate`, `HQaddress`, `HQmanager`, `HQphoneNb`).
* **Branch:** Regional distribution offices executing local reservations (`Branch_ID`, `B_name`, `addresss`, `_B_phoneNb`, `manger`),
* **Car Owner:** Tracks vehicle asset providers who lease fleets to branches (`O_ID`, `O_name`, `O_address`, `O_phoneNb`).
* **Driver:** Logs employee metrics, including operation branch, associated vehicles, and salary structure (`D_ID`, `D_name`, `NetSalary`, `D_address`, `D_phoneNb`).
* **Taxi Car:** Operates with tracking for capacity (`NbOfSeats_`), registration plates (`plateNb`), and model year
* **Reservation & Trip:** Manages logistical workflows, calculating base reservation parameters (pickup details, pricing) alongside transactional `Trip` executions (extra earnings, live dispatching).

---

