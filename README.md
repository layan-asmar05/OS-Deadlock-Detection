# Deadlock Detection Simulator Using Graph Reduction

## Overview
This project is an automated Python simulator designed to detect Resource Deadlocks in operating systems. It uses the Graph Reduction Algorithm to analyze system states by examining resource allocation matrices, determining if all processes can successfully complete execution or if the system is in a deadlocked state.

## Features & Methodology
* **Graph Reduction Logic:** The simulator evaluates the system by iteratively searching for unblocked processes (Request <= Available), simulating their completion, and releasing their allocated resources back to the available pool.
* **Interactive Cloud File Upload:** To provide a seamless User Experience (UX) and avoid hardcoded file paths, the program integrates Python's native `google.colab.files` library. It features an interactive upload widget allowing users to select and upload test case files directly into the cloud environment.

## Simulation Results & Test Cases
The simulator was successfully tested against different system states:
* **Test Case 1 (No Deadlock - `input1.txt`):** Tested a system state where all processes (e.g., 3 Processes, 2 Resources) were fully reduced and completed without getting blocked. (Execution Sequence: P2 -> P0 -> P1).
* **Test Case 2 (Deadlock Present - `input2.txt`):** Tested a system state where concurrent resource requests led to process blocking and an unresolved deadlock, correctly identifying the deadlocked processes (P0, P1).

## Course
Operating Systems
