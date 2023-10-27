# Week 7

### Grading

Task #|Points|Description|
-----|:---:|----------|
Task 1 | 1 | Safety Concerns
Task 2 | 1 | Static and Dynamic Analysers 
Task 3 | 1 | Security Certifications
Task 4 | 1 | Tietoturvamerkki
Task 5 | 1 | Showcase

(4 points max)

---

# Tasks

### Task 1: Safety Concerns

In terms of medical equipment and automotive industry mentioned in the Lecture 13, consider the following: 

- Why are new safety concerns sometimes overlooked? 
- What are events that trigger sudden change? 

250 words **maximum**, cite if you use external sources 

[Security Engineering Lecture 13: Safety and Security](https://www.youtube.com/watch?v=uZkQtnHKcJ4) 

Safety concerns in the medical equipment and automotive industries can sometimes be overlooked due to several factors. The complexity and rapid technological advancements in these industries make it challenging to anticipate all potential safety concerns. New technologies can introduce unforeseen risks that were not considered during initial design or regulatory approval processes. Additionally, there is often pressure to minimize costs and maximize efficiency, sometimes prioritizing immediate financial concerns over long-term safety considerations.

Regulatory frameworks may struggle to keep pace with technological advancements, resulting in outdated or inadequate safety regulations that do not address emerging risks. Compliance with existing regulations doesn't always guarantee absolute safety. Human error or oversight in the design, production, or regulation of products can also contribute to safety concerns being missed.

Sudden changes in addressing safety concerns can be triggered by high-profile incidents, leading to investigations, legal actions, and increased scrutiny. Regulatory changes may respond to emerging safety concerns, while consumer awareness and demand for safer products can drive change. Technological breakthroughs and litigation related to safety issues can also prompt companies to take action to address safety concerns.

Stakeholders in both industries must remain vigilant, adaptable, and responsive to emerging safety concerns through proactive risk assessment, ongoing research, and swift action to prevent harm to consumers and patients.
---

### Task 2: Static and Dynamic Analyzers

Explain the difference between static and dynamic analyzers. Explain what the advantages are of using these tools during production.  Pick one of the Static or Dynamic testing methods mentioned in the Lecture 14 and write a brief description of it. 

300 words **maximum**, cite if you use external sources 

[Security Engineering Lecture 14: Assurance and Sustainability](https://www.youtube.com/watch?v=cmWQF2FDlG8) 

Static Analysis:
Static analysis is a white-box testing method that examines the source code, design, and documentation of a software application without executing it. It aims to identify potential issues in the code by analyzing it in a non-runtime context. Static analyzers scan the code for structural and syntactical issues, potential vulnerabilities, and adherence to coding standards. This analysis is typically performed before the software is executed.

Dynamic Analysis:
Dynamic analysis, on the other hand, is a black-box testing method that assesses a software application while it's running. It involves the execution of the software with various inputs to observe its behavior in a runtime environment. Dynamic analyzers identify issues such as runtime errors, memory leaks, performance bottlenecks, and security vulnerabilities that may only become apparent during execution.

Advantages of Using Static and Dynamic Analyzers During Production:

Early Issue Detection: Static analyzers help identify issues in the code during development, even before the software is executed. This allows developers to fix issues at an early stage, reducing the cost and effort required for remediation.

Security Vulnerability Identification: Static analyzers can identify potential security vulnerabilities and compliance issues by examining the code. This is crucial for ensuring that security measures are integrated from the start, reducing the risk of post-production security breaches.

Performance Optimization: Dynamic analyzers help identify runtime performance issues and bottlenecks, enabling developers to optimize code for better system performance.

Memory Leak Detection: Dynamic analyzers can detect memory leaks, which can lead to system instability over time. Identifying and resolving memory leaks is critical for the reliability of a software product.

Real-world Scenario Testing: Dynamic analysis tests the software under real-world scenarios, helping ensure it functions correctly in the intended environment. It's particularly important for identifying issues that

---

### Task 3: Security Certification

Consider the different incentives (both 'Good' and 'Bad' incentives) for Security Certification of a product from the following points of view:

- Potential End User/Buyer of the product 
- Certifying authority (both vendor funded and non-profit) 
- Manufacturer/designer of the product 

400 words **maximum**, cite if you use external sources 

**(EXPLANATIONS)**

- Vendor funded = Applicant pays the certifying authority for the certification process 
- Non-profit = Applicant does not have to pay directly for the certification process 


[Security Engineering Lecture 15: Governance and Regulation](https://www.youtube.com/watch?v=PdMzMHizEaE) 
[Security Engineering Lecture 16: Ian Levy, NCSC - Protecting a country for fun and profit](https://www.youtube.com/watch?v=qv6SS5FhdUk) 

The potential end users/buyers of security-certified products are influenced by various incentives, both good and bad. Good incentives for end users include assured safety, where certification signifies rigorous testing to meet security standards, instilling trust and reducing the risk of cybersecurity threats. Certified products are also associated with reduced risk, as they tend to have fewer vulnerabilities, lowering the chances of data breaches and cyberattacks.

However, a potential bad incentive for end users is the false sense of security. Certification does not guarantee absolute protection against all threats, potentially leading to negligence in following security best practices.

Certifying authorities, whether vendor-funded or non-profit, are also subject to different incentives. Vendor-funded authorities aim for revenue generation, receiving fees from manufacturers for certification processes. This revenue can be reinvested to improve standards and processes. Non-profit certifying authorities focus on public trust, relying on their credibility to uphold rigorous certification standards.

Yet, bad incentives may arise for vendor-funded authorities due to financial pressure to meet revenue targets, potentially compromising thoroughness. They might also face conflicts of interest, being reliant on manufacturers for income, which can lead to bias in favor of vendors.

Manufacturers and designers of products are incentivized by competitive advantage through security certification, which attracts buyers and boosts sales. Going through the certification process can also lead to product improvement, identifying and rectifying security weaknesses for an enhanced user experience.

On the downside, if manufacturers fund certification, they may be tempted to cut corners to reduce costs, potentially leading to rushed or incomplete security assessments. Harm to reputation is another bad incentive, as failing to obtain or having certification revoked can damage a manufacturer's image, potentially leading to deceptive practices.

In conclusion, the security certification process is influenced by a variety of incentives, both positive and negative, for end users, certifying authorities, and product manufacturers. It is imperative for all parties involved to prioritize genuine security, maintain certification integrity, and ensure the safety of end users and the overall security ecosystem.
---

### Task 4: Tietoturvamerkki

You might be familiar with CE-Certification regarding electrical equipment and products. Although it is not a guarantee of safety, you can feel a certain amount of confidence towards the product. Could something similar be possible for Cybersecurity? 

Take a look at Tietoturvamerkki and write an essay answering the following questions: 

- What is Tietoturvamerkki 
- What kind of products does it concern 
- How does a product get a Tietoturvamekki certificate 
- What does the certificate guarantee about the product and what it does not 
- Include your own thoughts about this style of certificate. Would you pay more for a certified product? Do you see any problems regarding the certificate? 

400 words **maximum**. 
Tietoturvamerkki, also known as the Finnish Information Security Certification, is a cybersecurity certification program and mark used in Finland. It is administered by the Finnish Transport and Communications Agency (Traficom) and is designed to assess and certify the information security practices of various products and services. It primarily concerns digital products and services, including software applications, cloud services, and hardware devices that process or store sensitive data. It is applicable to a wide range of sectors, including finance, healthcare, government, and more. To obtain a Tietoturvamerkki certificate, a product or service must undergo a rigorous evaluation process. This typically involves a detailed assessment of its information security practices, including but not limited to data protection, access controls, encryption, and vulnerability management. The evaluation is conducted by accredited third-party auditors who specialize in information security. The certification process assesses compliance with recognized standards, such as ISO 27001, and Finnish national regulations. High Information Security Standards: It assures that the certified product or service meets high information security standards and follows recognized best practices.

-Compliance: Tietoturvamerkki signifies compliance with Finnish and international data protection and cybersecurity regulations.

-Data Protection: It indicates that the product or service effectively protects user data and sensitive information from breaches or unauthorized access.

In conclusion, Tietoturvamerkki is a positive step toward enhancing the cybersecurity of digital products and services. While it provides a valuable level of assurance, it should be seen as just one aspect of an overall cybersecurity strategy. A balanced approach that combines certification with ongoing vigilance and adaptation to emerging threats is crucial to maintaining strong cybersecurity.

FI: https://tietoturvamerkki.fi/fi/tietoturvamerkki-etusivu 

EN: https://tietoturvamerkki.fi/en/cybersecurity-label 


---

### Task 5: Showcase

Choose a Cybersecurity tool of your choice and answer the following questions about it.

Pick a new tool that has not been featured in the course, so the following are forbidden from this task: (Nmap/Zenmap, Wazuh, thc-hydra, BurpSuite, Trivy, Hadolint, Falco)

Name of the tool: Wireshark, https://www.wireshark.org/

Link to the tool website/repository: Wireshark Official Website

Free or Paid tool: Wireshark is an open-source and free tool.

When was the tool created and by who: Wireshark was originally created by Gerald Combs in 1998. It was previously known as Ethereal before the name was changed to Wireshark in 2006.

Is the tool Open Source: Yes, Wireshark is open-source and distributed under the GNU General Public License (GPL).

What is the tool used for: Wireshark is a network protocol analyzer. It is used for capturing, analyzing, and inspecting network traffic in real-time. It allows users to examine data from a live network or from a capture file on disk.

What are its capabilities:

Packet Capture: Wireshark can capture data from networks, whether from wired or wireless connections. It supports a wide range of network protocols.

Live Analysis: You can perform real-time analysis of data packets as they are captured, making it useful for diagnosing network issues or monitoring for suspicious activity.

Deep Inspection: Wireshark provides detailed information about captured packets, including the source and destination addresses, protocols used, and even the content of the data.

Filtering and Search: Users can apply various filters to narrow down the packets they want to inspect, making it easier to focus on specific traffic patterns.

Protocol Support: Wireshark supports a wide array of network protocols, including TCP/IP, HTTP, FTP, DNS, and many more.

Export and Save: You can save captured data to files for further analysis or sharing with others.

VoIP Analysis: Wireshark can also analyze Voice over IP (VoIP) traffic, making it valuable for diagnosing issues in voice communications.

Who would most benefit from this tool: Wireshark is highly beneficial for network administrators, security professionals, system and network engineers, and anyone involved in network troubleshooting, monitoring, or security analysis.

What kind of use case could you yourself have for this tool: As a network administrator or security professional, I might use Wireshark for various purposes, such as diagnosing network performance issues, monitoring for suspicious or malicious network activity, and analyzing network traffic patterns to optimize network performance. Additionally, Wireshark can be a valuable tool for educational purposes and for gaining a deep understanding of network protocols and their behavior.

