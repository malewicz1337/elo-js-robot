# Automated Delivery Robot

This project simulates an automated delivery robot navigating through a village to deliver parcels. It is written in JavaScript and demonstrates concepts such as graph theory, state management, and simple AI algorithms.

## Overview

The village is represented as a graph with locations (such as houses, shops, and the post office) as nodes and roads as edges. The robot navigates this graph to deliver parcels from one location to another.

## Components

### Graph Construction

The village map is constructed using a graph data structure. `buildGraph` function takes an array of road strings and converts them into a more usable form.

### Village State

`VillageState` class keeps track of the current state of the robot - its current location and the parcels yet to be delivered.

### Robots

There are different types of robots implemented:

- `randomRobot` - Chooses random directions.
- `routeRobot` - Follows a fixed route.
- `goalOrientedRobot` - Chooses the shortest path to deliver the next parcel.

### Simulation

`runRobot` function takes a `VillageState`, a robot, and a memory state, and runs the simulation until all parcels are delivered.

### Comparison

`compareRobots` function is used to compare the efficiency of different robots by calculating the average number of turns they take to deliver all parcels.

## License

This project is open source and available under the [MIT License](LICENSE).
