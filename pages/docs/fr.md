---
title: Functional Requirements
layout: default
parent: Documentation

## Description
The following section describes every individual functional and non-functional requirement that has been specified throughout the PA documents, including those that we believe are unlikely to be completed this semester. 


### Requirement Levels

| Level | Description                                                                                     | 
|-------|-------------------------------------------------------------------------------------------------|
| 1     | Level 1 requirements are those that we are confident will be done before Spring Break.          |
| 2     | Level 2 requirements are those that we are confident will be done before the final demo.        |
| 3     | Level 3 requirements are those that are nice (or necessary) in industry, but are more uncertain in terms of a timeline.|


### Implemented Requirements (03/24/24)

| ID  | L | Description                                                                                         | Status | Assigned     |
|-----|---|-----------------------------------------------------------------------------------------------------|--------|--------------|
| R01 | 1 | DeadDrop agents shall issue heartbeat messages at a user-defined interval.                          | ✓      | 02/26 Lloyd  |
| R02 | 1 | DeadDrop shall allow the user to build new instances of agents, irrespective of the platform used by the server. | ✓ | 03/08 Lloyd |
| R03 | 1 | DeadDrop shall allow the user to remotely execute shell commands through registered agents.         | ✓      | 03/05 Lloyd  |
| R05 | 1 | DeadDrop shall allow users to remotely connect to the server interface.                              | ✓      | ~2023 Jann   |
| R07 | 1 | DeadDrop shall implement a covert communication protocol that communicates solely over a popular service. | ✓ | ~2023 Keaton |
| R08 | 1 | DeadDrop shall implement a user authentication system.                                               | ✓      | 03/08 Jann/Brian |
| R09 | 1 | DeadDrop shall provide a Svelte web interface, a reference implementation for interacting with all available backend endpoints. | ✓ | ~2023 Brian |
| R10 | 1 | DeadDrop shall provide Pygin, a built-in reference implementation for an agent adhering to all available framework interfaces. | ✓ | ~2024 Lloyd |
| R16 | 1 | Pygin shall execute commands concurrently.                                                            | ✓      | ~2024 Lloyd  |
| R18 | 1 | Pygin shall use supervisord to manage and configure its multi-process requirements.                   | ✓      | ~2023 Lloyd  |
| R19 | 1 | The DeadDrop server shall allow users to display and filter logs without requiring the logs to be exported. | ✓ | 12/01/23 Brian/Jann |
| R20 | 1 | The DeadDrop server shall generate agent public/private key pairs in a cryptographically secure manner. | ✓ | 03/07 Lloyd |
| R22 | 2 | DeadDrop agents shall provide a standard entrypoint script for installation that allows for the discovery of available commands and other metadata as a JSON document. | ✓ | 03/06 Lloyd |
| R29 | 2 | The DeadDrop server shall implement a package manager allowing for the installation and availability of new agents and protocols without requiring assumptions of the server’s directory structure. | ✓ | 02/29 Lloyd |
| R31 | 2 | DeadDrop shall allow users to stand up fake websites to emulate popular services.                      | ✓      | ~2024 Keaton |
| R32 | 2 | DeadDrop shall provide common statistics relating to messages sent and received over secure protocols. | ✓      | ~2024 Keaton/Brian |
| R33 | 3 | Users shall be able to easily add new implementations of communication protocols.                     | ✓      | ~2024 Keaton/Lloyd |
| R44 | 3 | DeadDrop shall handle asynchronous tasking with Celery.    

### Planned Requiremens (3/24/24)

| ID  | L | Description                                                                                         | Status | Assigned     |
|-----|---|-----------------------------------------------------------------------------------------------------|--------|--------------|
| R04 | 1 | DeadDrop shall allow users to export logs to a standardized format.                                 | ◯      | Jann/Brian   |
| R06 | 1 | DeadDrop shall encrypt messages using AES-CBC, with a minimum of a 128-bit key length.              | ◯      | Lloyd        |
| R11 | 1 | DeadDrop shall record all actions initiated by a user or an agent in a standard format.             | ◯      | Brian        |
| R12 | 1 | DeadDrop shall record all data transferred via communication protocols in a standard format.        | ◯      | Jann         |
| R13 | 1 | DeadDrop shall use the Elliptic Curve Digital Signature Algorithm (ECDSA) to verify message integrity.| ◯   | Lloyd        |
| R14 | 1 | Pygin shall bundle itself as a PyInstaller-generated executable.                                   |        | Lloyd        |
| R15 | 1 | Pygin shall contain portable, platform-specific executables for any dependencies needed.           |        | Lloyd        |
| R17 | 1 | Pygin shall provide a command allowing users to execute arbitrary Python code.                     | ◯      | Lloyd        |
| R21 | 1 | The Svelte frontend shall use automated Lighthouse CI tests for accessibility, tracked over time.  |        | Brian        |
| R23 | 2 | DeadDrop shall allow the user to remove and remotely uninstall agents.                             |        | Jann         |
| R24 | 2 | DeadDrop shall implement a “guardrail” system, preventing the framework from acting on user-defined hosts. | | Jann   |
| R25 | 2 | DeadDrop shall implement an “allowlist” system, forcing the framework to act only on user-defined hosts. | | Jann   |
| R26 | 2 | DeadDrop shall perform a user-defined action if an agent is unreachable for a specified number of attempts. | | Keaton |
| R27 | 2 | Pygin shall implement at least one example of a command renderer, whereby the response may be visualized. | | Brian  |
| R28 | 2 | Pygin shall provide the ability to transfer arbitrary files to and from the infected device.       | ◯      | Keaton       |
| R30 | 2 | DeadDrop may automatically visualize well-formatted responses as a graph, chart, tree, etc.        |        | Brian        |
| R34 | 3 | DeadDrop agents shall automatically discover accessible devices from the current device.           |        | Jann         |
| R35 | 3 | DeadDrop agents shall be able to forward messages from other agents without direct internet access.|        | Lloyd        |
| R36 | 3 | DeadDrop agents should not assume the availability of platform-specific binaries.                  |        | Keaton       |
| R37 | 3 | DeadDrop protocol implementations shall expose an easy method to visit the URLs being used.        |        | Keaton       |
| R38 | 3 | DeadDrop shall allow users to open a live terminal session with an agent.                          |        | Keaton/Lloyd |
| R39 | 3 | DeadDrop shall allow users to register “virtual” agents representing discovered machines.          | ◯      | Jann         |
| R40 | 3 | DeadDrop shall allow users to unregister virtual agents.                                           | ◯      | Jann         |
| R41 | 3 | DeadDrop shall allow users to write reusable scripts for sets of commands on an agent.             |        | Jann         |
| R42 | 3 | The Svelte frontend shall provide desktop notifications of completed asynchronous tasks.           |        | Jann/Brian   |
| R43 | 3 | Pygin shall implement a command to steal Discord session tokens for demonstration purposes.        | ◯      | Lloyd        |
