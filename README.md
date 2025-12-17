# Packet Routing Simulator

**DSA Project: Packet Routing Simulator using D3.js**

A simplified, interactive demonstration of packet routing in a Software-Defined Network (SDN). This project visualizes how packets traverse a network using **Dijkstra's Algorithm** for shortest path calculation.

## Features

*   **Dynamic Network Construction**: Define your network topology using a simple text-based edge list (Source, Destination, Cost).
*   **Interactive Visualization**: Drag and drop routers to organize the network layout visually.
*   **Packet Simulation**: Send packets from a source to a destination with a configurable **Time-To-Live (TTL)**.
*   **Routing Logic**:
    *   Automatic calculation of forwarding tables for every router using **Dijkstra's Shortest Path Algorithm**.
    *   TTL decrement logic to simulate real-world packet expiry.
    *   Visual feedback for packet status:
        *   **Queued**: Waiting at a router.
        *   **In-Transit**: Moving between routers.
        *   **Arrived**: Successfully reached destination.
        *   **Dropped**: TTL expired or no route found.
*   **Simulation Controls**: Adjust simulation speed, zoom/pan the graph, and reset the environment.
*   **Inspector**: View the routing/forwarding table for any simple router.

## Technologies Used

*   **HTML5 & CSS3**
*   **JavaScript (ES6+)**
*   **[D3.js (v7)](https://d3js.org/)**: For powerful, dynamic network visualizations.
*   **[Bootstrap 5](https://getbootstrap.com/)**: For responsive UI and styling.

## How to Use

1.  **Define Network Edges**:
    *   Use the text area in the control panel to define connections.
    *   Format: `Source,Destination,Cost` (e.g., `A,B,4`).
    *   The graph updates automatically.

2.  **Send a Packet**:
    *   Enter the **Source** Router ID (e.g., `A`).
    *   Enter the **Destination** Router ID (e.g., `F`).
    *   Set the **TTL** (Time-To-Live).
    *   Click **Send**.

3.  **Control Simulation**:
    *   Use the **Slider** to change the speed (tick duration).
    *   Use **Reset** to clear all packets.
    *   Use **Zoom (+/-)** keys to navigate larger networks.

4.  **Inspect Routers**:
    *   Select a router from the dropdown to see its calculated **Forwarding Table** (Next Hop for each destination).

## Authors

**Group 6**

*   **Armaan Z. Hussain** (Initial Developer & Visualization Architect)
    *   Prototyped initial routing algorithms and graph logic using Python (NetworkX & Matplotlib).
    *   Designed and implemented the interactive D3.js network visualization engine.
    *   Provided reference logic for the web-based simulation architecture.
*   Lakshya Dubey
*   Kannabiran 
*   Pranav Ranjan 

## Live Demo

[Packet Routing Simulator Live Demo]
(https://iamjustincase.github.io/packet_routing_simulator/)
