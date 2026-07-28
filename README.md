Domain: Computer Networks — Software-Defined Networking (SDN) and Network Traffic Engineering

Problem Statement:
Traditional networks rely on distributed, device-level routing decisions, which makes them slow to detect and recover from link or node failures. This results in downtime, packet loss, and inefficient traffic distribution during disruptions — a critical limitation for modern data center and enterprise networks that demand high availability.

Objective:
To design and evaluate an SDN-based framework capable of automatically detecting network failures and dynamically rerouting traffic — exhibiting "self-healing" behavior — while intelligently balancing load across available paths. The project further investigates whether an adaptive load balancing algorithm offers measurable performance advantages over conventional static routing methods under failure conditions.

Methodology:
A virtual network topology is constructed using Mininet, with a centralized Ryu (OpenFlow) controller governing routing decisions. Two approaches are implemented and evaluated under identical, controlled conditions:

Static/baseline routing (e.g., round-robin or ECMP-style forwarding)
Proposed adaptive routing algorithm, which monitors real-time link statistics and dynamically reroutes traffic in response to congestion or failure

Simulated link and node failures are introduced to test both approaches, with traffic generated using varying patterns (TCP/UDP, steady vs. bursty, single vs. multiple flows) via iperf.

Evaluation Metrics:

Failover/recovery time
Throughput before and after failure
Packet loss during rerouting
Load distribution efficiency across available paths

Expected Contribution:
Quantitative evidence demonstrating the performance gains of adaptive, self-healing load balancing over static routing strategies in SDN environments — positioning the project as a comparative research study rather than a standalone system implementation, with results presented through empirical data, graphs, and statistical comparison.
