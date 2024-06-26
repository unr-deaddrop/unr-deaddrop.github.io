---
title: Overview
layout: default
nav_order: 2
---
<center>
  <h1><span style="color: red;">Dead</span>Drop</h1>
  <i>a clever command and control framework</i>
</center>
DeadDrop is a command and control (C2) framework used in post-exploitation activities and penetration testing to create malware payloads, manage compromised devices, and generate operational reports. DeadDrop’s primary purpose is to aid legitimate security professionals (the “red team”) in an activity known as penetration testing, which assesses the company’s ability to defend against attacks and protect its data.

Penetration tests are often coordinated using C2 frameworks, which greatly simplifies the task of managing infected devices while ensuring accountability for actions taken by the red team. The use of a C2 framework in testing greatly benefits security engineers (the “blue team”), as they can identify holes in detecting malicious activity through the reporting and logging functionality provided by the C2 framework. That is, the use of C2 frameworks is critical to penetration testers and security engineers alike.

However, unlike existing frameworks that communicate directly with attacker domains, DeadDrop focuses on leveraging features in legitimate websites such as YouTube and Wikipedia to communicate with devices and exfiltrate data, masking its activity within the noise of popular websites. Messages (“dead drops”) can be placed on external services by one device, which can be retrieved by the other device by accessing the external service. By abusing the “trust” behind large, well-known websites, DeadDrop provides security engineers with new insight into identifying covert attacker techniques and security weaknesses. In doing so, it encourages network security engineers to take new approaches to identifying covert communication methods that could be used by skilled attackers. 

Like many C2 frameworks, DeadDrop provides the following major features through its web interface and internal APIs:
- Payload generation: Users can build and configure new instances of agents, leveraging containers to allow platform-agnostic building.
- Messaging: Users can communicate with agents to execute commands on remote devices and receive results.
- Reporting and administration: The server provides permissions systems and logging for developing organizational reports and ensuring accountability.

### Visualization of Codebase Development
We've spent the last few months building the foundation to create an ecosystem of agents that adhere to the DeadDrop framework, built on an extremely modular architecture and a huge set of standard interfaces. At this point, the entire DeadDrop project is 31,000 lines of code (of which half is random JavaScript boilerplate)
across 14 repositories, a testament to how much time has been spent complaining about JavaScript.

<iframe width="560" height="315" src="https://www.youtube.com/embed/wcX7spr_SXo?si=vfrrOl_XfZYn94Ln" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>