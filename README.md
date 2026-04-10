# Smart Elevator Control System ERD

## Overview

This project contains the **ER Diagram** for a multi-building smart elevator control system designed for large-scale infrastructures like corporate towers, malls, airports, hospitals, and high-rise residential complexes.

It supports:

- Multiple buildings connected to a single platform
- Multiple elevators per building
- Floor-level request handling
- Intelligent elevator assignment
- Real-time status monitoring
- Ride history and analytics
- Maintenance tracking

---

## Key Features

- One building → multiple floors and elevators
- One elevator → serves multiple floors
- One floor → can be served by multiple elevators
- One request → assigned to exactly one elevator
- Elevators handle multiple rides daily
- Tracks real-time elevator status (idle, moving, maintenance)
- Maintains complete ride logs for analytics
- Supports maintenance history without overwriting past data

---

## System Design Highlights

- Separation of **static data** (buildings, elevators) and **dynamic data** (requests, rides, status)
- Uses **junction table** for elevator–floor many-to-many relationship
- Clean lifecycle: **Request → Assignment → Ride Log**
- Scalable for high-traffic, real-time systems
- Designed for operational monitoring and performance analysis

---

## Files

- `erd-diagram.png` – ER diagram image
- `schema.txt` or `eraser-code.txt` – ER diagram definition (Eraser format)
- `README.md` – Project documentation
