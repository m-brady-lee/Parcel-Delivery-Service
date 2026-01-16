# WGU PARCEL SERVICE (TRAVELING SALESMAN SOLUTION)

A Python-based terminal application that solves a constrained version of the Traveling Salesman Problem (TSP) using a modified nearest neighbor algorithm. The program simulates a university parcel service tasked with delivering packages efficiently while respecting delivery deadlines, truck constraints, and dynamic package updates.

## OBJECTIVE

To design and implement an efficient delivery routing solution for a parcel service operating under real-world constraints. The system must successfully deliver 40 packages using 3 trucks and 2 drivers, navigate a network of 27 locations, and keep total mileage under 140 miles, while honoring package-specific delivery rules and deadlines.

## PROBLEM STATEMENT

This project models a constrained Traveling Salesman Problem where:

Multiple vehicles operate with staggered departure times

Packages have different delivery deadlines (EOD, 9:00 AM, 10:30 AM)

Certain packages must be delivered together or assigned to specific trucks

Package delivery locations may change dynamically during execution

The solution must ensure all packages are delivered correctly, with accurate status tracking at any point in time.

## SOLUTION OVERVIEW

The application uses a modified nearest neighbor algorithm to determine efficient delivery routes while accounting for package constraints and timing dependencies.

Key characteristics of the solution:

Dynamic route construction per truck

Constraint-aware package assignment

Real-time status tracking for all packages

Mileage optimization within the specified limit

## APPLICATION FEATURES
Package Status Tracking

View the status of an individual package at any time

View the status of all packages at a given time

Status states include:

Heading to Depot

Loaded

In Route

Delivered

Truck Details

Displays:

Start and end times

Total mileage per truck

Delivery route sequence (by vertex)

Shows cumulative mileage across all trucks

Interactive Terminal Menu

The application provides a simple command-line interface with four options:

Check Status of Individual Package

Check Status of All Packages

View Truck Details

Exit the Program

## PACKAGE CONSTRAINTS HANDLED

Time-specific delivery deadlines

Truck-specific package assignments

Grouped delivery requirements

Delayed package availability

Address corrections during runtime

The system updates package statuses and routing logic accordingly to ensure valid deliveries.

DATA STRUCTURES & DESIGN

Hash Table for constant-time package lookup

Graph-based distance model for routing decisions

Truck objects tracking assigned packages, mileage, and time

Package objects storing delivery data, constraints, and status history

Each package maintains a full status timeline, allowing accurate historical lookups.

## ALGORITHM & PERFORMANCE

Routing Strategy: Modified Nearest Neighbor

Time Complexity: O(N²) worst case (acceptable for constrained dataset)

Total Mileage Achieved: 128.60 miles

Mileage Requirement: < 140 miles (met)

The algorithm balances efficiency with constraint satisfaction rather than pure distance minimization.

## TOOLS & TECHNOLOGY

Language: Python

IDE: PyCharm 2024.1.1 (Professional Edition)

Runtime: OpenJDK 17

Platform: macOS

Data Handling: Custom data structures (hash tables, objects)

## SCREENSHOTS
![Package Status Lookup](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Option%201.png)

![All Packages Status View](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Option%202.png)

![Truck Details](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Option%203.png)

![Truck Loading Logic](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Load%20Trucks.png)

![Program Exit](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Option%204.png)

![Location & Distance Data](https://github.com/m-brady-lee/Parcel-Delivery-Service/blob/main/Locations.png)

## KEY TAKEAWAYS

Demonstrates applied algorithm design under real-world constraints

Shows strong understanding of data structures and state management

Emphasizes correctness, traceability, and operational logic

Balances performance optimization with business rules

## NOTES ON DATA USAGE

All data used in this project is instructional and non-proprietary. No real-world delivery data or sensitive information is included.

## FUTURE IMPROVEMENTS

Replace nearest neighbor with heuristic optimization (e.g., simulated annealing)

Add visualization of routes and delivery progression

Improve scalability for larger package sets

Introduce automated testing for constraint validation

## AUTHOR

Michael Lee
📧 m.brady.lee@gmail.com

Student Application Version: V1
Project Date: 06/03/2024
