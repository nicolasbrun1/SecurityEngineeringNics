# Week 5

### Grading

Task #|Points|Description|
-----|:---:|----------|
Task 1 | 1 | Bring Your Own Device
Task 2 | 1 | Attacks on CPU Execution
Task 3 | 1 | Securing OS
Task 4 | 1 | Logging 

---

# Tasks

### Task1: Bring your own devices

Following link containing NIST:s [security recommendations for workplace bring your own device](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.1800-22.pdf). On the page 12 is listed following 9 threat events, and your job is to make one A4 sized poster or otherwise shortly summarize what each listed threat event means based on the document or your own research.

- Intrusive application practices: This threat event involves apps with invasive behaviors, such as accessing personal data without consent or tracking user activity. It compromises user privacy and can lead to data misuse.
- Account credential theft through phishing: Phishing refers to deceptive techniques used to trick individuals into revealing their login credentials. Threat actors impersonate trustworthy entities to steal usernames and passwords.
- outdated phones: Using outdated smartphones with unpatched software poses security risks. These devices may have unaddressed vulnerabilities that can be exploited by attackers.
- Sensitive data transmissions: When sensitive information is transmitted over networks without encryption or secure protocols, it's susceptible to interception and unauthorized access, potentially leading to data breaches.
- Brute-force attacks to unlock a phone: In a brute-force attack, attackers repeatedly guess a phone's PIN or password until they gain access. This threatens device security and privacy.
- Application credential storage vulnerability: Applications storing user credentials insecurely may expose sensitive data to malicious actors. It's a risk when apps don't follow secure storage practices.
- Unmanaged device protection: This threat event concerns the lack of security measures on unmanaged devices (e.g., personal devices) accessing enterprise networks, potentially compromising corporate data and networks.
- Lost or stolen data protection: Losing or having a device stolen can lead to data loss or unauthorized access. Protecting data on these devices is crucial to prevent information leaks.
- Protecting enterprise data from being inadvertently backed up to a cloud service: This threat event focuses on the unintentional backup of sensitive enterprise data to unsecured or unauthorized cloud services. It poses data leakage and compliance risks for organizations.

---

### Task2: attacks on CPU execution
spectre and meltdown are two original side channel attacks discovered in 2017 that target cpu, and over the years more have been discovered. [This wikipedia article](https://en.wikipedia.org/wiki/Transient_execution_CPU_vulnerability) list some of them. Pick 3 of them to research about how exactly each exploits the system,their differences, which systems they targeted and how they can be mitigated. 

Answer in max 300 words. You are free to use tables or otherwise make to comparison easier to read if you wish.

Spectre variant 1 (Bounds Check Bypass): takes advantage of speculative execution that bypasses conditional branch instructions used for memory access bounds check. results in memory accesses to invalid memory (with out-of-bound index) that are done speculatively before validation checks resolve. Spectre variant 1 is not only about user-controlled array bounds checks. It can affect any conditional checks.

Spectre variant 2 (Branch Target Injection): takes advantage of speculative execution of indirect branches. The indirect branch predictors inside the processor used to guess the target of indirect branches can be influenced by an attacker, causing gadget code to be speculatively executed, thus exposing sensitive data touched by the victim. The attacker can steer speculative indirect branches in the victim to gadget code by poisoning the branch target buffer of a CPU used for predicting indirect branch addresses.
Processors affected by Spectre: Cortex-R7, Cortex-R8, Cortex-A8, Cortex-A9, Cortex-A15, Cortex-A17, Cortex-A57, Cortex-A72, Cortex-A73 and ARM Cortex-A75 cores.
Meltdown Rogue Data Cache Load: The Meltdown technique can enable a user process to read kernel memory. Apply to all modern processors and affect nearly all computing devices and operating systems. All Mac systems and iOS devices are affected, but there are no known exploits impacting customers at the time of this writing. 


---

### Task3: Securing OS
Following is a list of some of the more common vulnerabilities and attack vectors existing in operating systems.  

- Malware and Viruses:
What harm can it cause to you?

Data Theft: Malware and viruses can steal your personal information, financial data, and sensitive documents from your computer, putting you at risk of identity theft or financial loss.
System Instability: Malware can disrupt your computer's normal functioning, causing crashes, slowdowns, and data corruption.
How can you mitigate it?

Antivirus Software: Install reputable antivirus software and keep it up to date to detect and remove malware.
Safe Browsing: Avoid downloading files from untrusted sources and clicking on suspicious links or email attachments.

- Exploiting Software Vulnerabilities: 
What harm can it cause to you?

Unauthorized Access: Exploiting software vulnerabilities can allow attackers to gain unauthorized access to your system or sensitive data.
Data Loss or Corruption: It can result in data loss, data corruption, or even system compromise.
How can you mitigate it?

Regular Updates: Keep your operating system and software up to date with security patches to fix known vulnerabilities.
Network Security: Use firewalls, intrusion detection systems, and network monitoring to detect and block exploit attempts.

- Phishing and Social Engineering:
What harm can it cause to you?

Identity Theft: Phishing and social engineering can trick you into revealing personal and financial information, leading to identity theft.
Unauthorized Account Access: Attackers can gain access to your accounts, including email and banking, if you fall for their tricks.
How can you mitigate it?

Education: Be cautious of unsolicited emails and messages. Verify the sender's identity and don't click on links or download attachments unless you're certain of their legitimacy.
Two-Factor Authentication (2FA): Enable 2FA for your important accounts to add an extra layer of security.

- Drive-by Downloads:
What harm can it cause to you?

Malware Installation: Drive-by downloads can silently install malware on your computer when you visit a compromised website.
Data Theft: It can lead to data theft and unauthorized access if your system is compromised.
How can you mitigate it?

Browser Security: Keep your web browser and plugins up to date to block known vulnerabilities.
Antivirus and Security Software: Use reliable security software that can detect and block malicious downloads.

- Zero-Day Exploits:
What harm can it cause to you?

System Compromise: Zero-day exploits target vulnerabilities that are unknown to the software vendor. They can lead to complete system compromise, data breaches, and unauthorized access.
Data Exfiltration: Attackers can use zero-day exploits to steal sensitive data, intellectual property, or personal information.
How can you mitigate it?

Patch Management: Keep your software and operating systems updated with the latest patches and security updates to minimize the risk of zero-day exploits.
Network Security: Employ intrusion detection systems and network monitoring to detect and respond to suspicious activities.

- USB/Removable Media Attacks:
What harm can it cause to you?

Malware Transmission: Attackers can load malicious software onto USB drives and spread it to your system when you insert the infected device.
Data Theft: USB attacks may target data theft or compromise by copying or altering files on your system.
How can you mitigate it?

USB Scanning: Use antivirus software to scan USB drives for malware before opening files.
User Training: Educate users about the risks associated with inserting unknown or untrusted USB drives into their computers.

- Password Cracking:
What harm can it cause to you?

Unauthorized Access: Password cracking can allow attackers to gain unauthorized access to your accounts, files, or systems.
Data Exposure: Once an attacker has access, they can steal sensitive data or compromise your online presence.
How can you mitigate it?

Strong Passwords: Use complex, unique passwords for each account and change them regularly.
Multi-Factor Authentication (MFA): Enable MFA wherever possible to provide an extra layer of security even if your password is compromised.
Mitigating these threats involves a combination of good security practices, software updates, user education, and the use of security tools and measures to reduce the risk of harm caused by these different types of cyberattacks.

Make short write up about each that answers following questions 
1. What harm can it cause to you?
2. How OS of your choosing (Windows, Mac, Linux) can mitigate it?
     - Function of the OS itself or external tools?


---

### Task4: Logging
Log files are records of events or actions that occur in a system, application, or program. Logs are essential for troubleshooting, debugging, and analyzing the behavior of software or hardware.

Find answers to following questions:
1. What kind of information would be saved into following types of log files

- Application logs
     *Application Errors: Recording of errors or exceptions from apps, crashes, bugs, issues.
     *User activities: Recording of login attempts, actions taken, user preferences.
     *Performance Metrics: Recording of performance related data.
- Event logs
     *System Events: Recording of the constant changes happening on the system, shutting off/on or hardware changes.
     *Security Events: Recording of security related information, login attempts, account management, security policie changes.
     *Application Events: Recording of changes in apps, starting, closing, resource usage.
- Service logs
     *Service Start/Stop: Recording of when a service starts or stops.
     *Service Errors: Recording of information about errors or issues encountered by services
     *Service Performance: Recording of performance data, like response times, resource usage, and overall service health metrics.
- System logs
     *System Events: Recording of system-level events, such as hardware changes, kernel-level errors, or system-wide configuration changes.
     *Resource Usage:  Recording of the utilization of system resources like CPU, memory, and disk space.
     *Security Information: Recording of security-related data, such as authentication and authorization events, as well as access control information.

2. Where in each of the common Operating Systems those logs would be stored (Windows, Mac, Linux(changes per distro so provide in answer which you are using)

     Windows:

     Application Logs: In Windows, application logs are typically stored in the "Event Viewer." You can access this tool by opening the "Event Viewer" from the Control Panel or by searching for it in the Start menu. Application-specific logs may be found under the "Windows Logs" section.

     Event Logs: Windows stores event logs in the "Event Viewer" as well. Security events, system events, and application events are categorized and can be accessed through the "Event Viewer."

     Service Logs: Service logs may be located in various places depending on the services. Some services have their logs in the Windows Event Logs, while others may maintain separate log files in specific directories.

     System Logs: System logs, including system events and resource usage, are also accessible via the "Event Viewer" under the "Windows Logs" section.

     macOS:

     Application Logs: macOS stores application-specific logs in the "/Library/Logs" and "~/Library/Logs" directories. You can use the Console application to view these logs.

     Event Logs: macOS maintains various logs in the "/var/log" directory. System logs, security logs, and other system-level logs are stored here. You can use the "Console" app to access these logs.

     Service Logs: Service logs on macOS are often stored alongside application logs. Specific services may have their logs in the "/Library/Logs" and "~/Library/Logs" directories.

     Linux:
     Linux log file locations can vary by distribution, but there are some common locations:

     Application Logs: Application-specific logs may be found in the "/var/log" directory. Common subdirectories include "/var/log/apache" for Apache web server logs or "/var/log/nginx" for Nginx web server logs. It can also vary based on the application.

     Event Logs: System logs, such as those managed by the syslog service, are usually stored in "/var/log/syslog" or "/var/log/messages" on many Linux distributions.

     Service Logs: Logs for various services can be located in the "/var/log" directory, often in subdirectories specific to the service name, such as "/var/log/mysql" for MySQL database logs.

     System Logs: System logs and kernel messages are typically found in "/var/log" under names like "syslog" or "messages."

3. What kind of threads you could you notice by monitoring each log file?
-Application Log:
     *Application logs can reveal errors, crashes, and exceptions, which are indicators of software bugs or instability.
     *Monitoring user activity within an application can help identify unusual or suspicious actions.
-Event Log:
     *System event logs can provide information about the overall health of the system, including hardware failures, disk errors, and system restarts.
     *Security-related events, such as failed login attempts or changes to security policies, can be detected in event logs.
-Service Log:
     *Service logs can indicate service start and stop events. Frequent service interruptions may signify problems with the service or dependencies.
     *Errors in service logs can alert you to issues that need attention, potentially impacting the service's functionality.
-System Log:
     *System logs can reveal resource usage patterns, such as CPU, memory, and disk space, which can help identify performance issues or resource bottlenecks.
     *Kernel-related log entries can indicate issues at the core of the operating system, such as hardware driver problems or kernel panics.

4. How would you go about monitoring logs on your personal computer?
     If i'm being honest, I don't actually look at any of my logs, maybe it would be a good idea to do it, so I went after information on what it is typically essential to be monitoring, here its what I found:
     Security Events:
     Failed Login Attempts: Monitor for repeated login failures, which could indicate unauthorized access attempts.
     User Account Changes: Watch for changes to user accounts, including new accounts, password changes, or privilege modifications.
     Access Control: Keep an eye on access control events, especially those related to file and directory permissions.
     System Health and Performance:

     Hardware Errors: Check for hardware-related errors, such as disk errors, memory issues, or CPU faults.
     Resource Usage: Monitor CPU, memory, and disk usage to detect performance bottlenecks or resource constraints.
     Kernel Messages: Keep an eye on kernel-related events, like system crashes or driver errors.
     Application Logs:

     Errors and Exceptions: Watch for error messages and exceptions generated by applications, which could indicate software bugs or issues.
     Application Start/Stop: Monitor when applications start or stop to track their availability and potential crashes.
     Service Logs:

     Service Start/Stop: Keep track of service start and stop events to ensure service availability.
     Service Errors: Monitor for service-related errors or crashes, which could affect system functionality.
     Network Activity:

     Network Connections: Track network connections and IP addresses that your computer communicates with. Look for unusual or unauthorized connections.
     Firewall Events: Check for firewall-related logs, especially blocked or allowed traffic.
     File System Changes:

     File Access and Modification: Monitor file and directory access, changes, and modifications to detect unauthorized or suspicious activities.
     File Integrity Checks: Implement file integrity checking mechanisms to ensure files have not been tampered with.
     Software Updates and Patches:

     Monitor for updates and patches: Ensure that your operating system and software are up-to-date to address known security vulnerabilities.
     Application-Specific Logs:

     Depending on the software you use, consider monitoring logs specific to applications you rely on, such as web server logs, database logs, or email server logs.
     Custom Alerts:

     Set up custom alerts for specific events or error messages that are relevant to your system and its operations.
     Archiving and Retention:

     Define a log retention policy that outlines how long logs should be kept, and consider archiving old logs for historical reference.
     The specific logs and log entries you need to monitor will depend on your system's purpose, potential risks, and the applications you use. It's important to regularly review logs and respond to any anomalies or security incidents to maintain the security and performance of your computer system.







remember to list sources for information you use!
ChatGPT
https://blogs.helsinki.fi/students-digital-skills/1-introduction-to-the-use-of-computers/1-1-computer-functionality/operating-system-and-user-interface/
https://www.loggly.com/ultimate-guide/linux-logging-basics/
https://www.zabbix.com/documentation/current/en/manual/config/items/itemtypes/log_items
https://docs.kernel.org/admin-guide/hw-vuln/spectre.html#:~:text=Spectre%20variant%201%20(Bounds%20Check,access%20within%20a%20valid%20range).
https://support.apple.com/en-ph/101886#:~:text=Meltdown%20is%20a%20name%20given,in%20iOS%2011.2%2C%20macOS%2010.13.