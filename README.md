

# Basic Container Terminal Simulation with SimPy

## Context
This project develops a basic simulation of a container terminal operation using the SimPy simulation framework. The goal is to model the process of vessels arriving at the terminal, being serviced by quay cranes, and having their containers transported to the yard by trucks. 

## Assignment Task
The simulation focuses on translating described logistics and operational logic into code, assessing the ability to follow best practices in code development. An object-oriented approach is recommended to structure the simulation, emphasizing code quality and maintainability.

### Key Simulation Details:
- **Vessel Arrivals:** Modeled with an exponential distribution, averaging 5 hours between arrivals. Each vessel carries 150 containers.
- **Berthing Slots:** Limited to 2, requiring arriving vessels to wait if both are occupied.
- **Quay Cranes:** 2 cranes available, each taking 3 minutes to move one container to terminal trucks.
- **Truck Operations:** 3 trucks transporting containers from cranes to the yard, with a 6-minute round trip.

## Approach
- **SimPy Framework:** Utilized for event-driven simulation, employing its components to model terminal operations.
- **Exponential Distribution:** Applied for vessel arrival times, using Python's `random.expovariate`.
- **Concurrency Handling:** SimPy's processes and resources manage the simultaneous operations of berthing, container movement, and truck transportation.
- **Logging:** Event logs are implemented via print statements, including timestamps for tracking simulation progress.

## Technologies Used
   - Python 3.6 or newer.
   - SimPy package (install with `pip install simpy`).





