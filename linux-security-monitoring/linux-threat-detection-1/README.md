# Linux Threat Detection 1

> **Platform:** TryHackMe
> **Difficulty:** Easy
> **Category:** SOC / Blue Team / Linux Threat Detection

## Overview

This repository documents my learning experience from the **Linux Threat Detection 1** room on TryHackMe. The room focuses on detecting common attack techniques targeting Linux systems by analysing authentication logs, application logs, and audit data.

The exercises simulate realistic SOC investigations where the objective is to identify suspicious activity, reconstruct attacker behaviour, and understand how different log sources contribute to incident response.

---

## Objectives

* Understand common Linux initial access techniques.
* Investigate SSH authentication events.
* Detect brute-force attacks against Linux systems.
* Analyse exposed services as potential attack vectors.
* Build process trees to trace malicious activity.
* Use audit logs to investigate process execution.
* Understand advanced initial access techniques and detection strategies.

---

## My Approach

I approached each task as a security investigation rather than simply searching for challenge answers.

My workflow included:

* Reviewing authentication logs to understand user login activity.
* Filtering SSH events to identify suspicious authentication attempts.
* Analysing login patterns to distinguish legitimate access from malicious behaviour.
* Investigating application logs to understand how exposed services can be abused.
* Examining audit logs to correlate suspicious processes with their parent processes.
* Building process trees to trace attacker actions back to their originating application.
* Understanding how different attack techniques appear within Linux logs.
* Correlating multiple data sources to reconstruct the attack chain.

This approach helped me develop a structured investigation methodology similar to what SOC analysts use during real incident investigations.

---

## Key Concepts Covered

* Linux Authentication Logs
* SSH Monitoring
* Password Brute Force Detection
* Initial Access Techniques
* Public Service Exploitation
* Application Log Analysis
* Process Tree Analysis
* Parent and Child Processes
* Linux Audit Logs (`auditd`)
* Command Execution Monitoring
* Reverse Shell Detection
* MITRE ATT&CK Initial Access Techniques

---

## Skills Gained

After completing this room, I became more confident in:

* Investigating SSH authentication events.
* Detecting brute-force attacks through log analysis.
* Identifying suspicious remote access patterns.
* Analysing Linux application logs for signs of exploitation.
* Understanding how vulnerable services can be leveraged by attackers.
* Building process trees to trace attacker activity.
* Using audit logs to investigate executed commands.
* Correlating multiple log sources during incident investigations.
* Mapping attacker behaviour to the MITRE ATT&CK framework.

---

## Key Takeaways

One of the biggest lessons from this room was the importance of following the attack chain rather than investigating isolated events. Authentication logs reveal how attackers gain access, application logs provide context on exploited services, and audit logs help reconstruct the exact sequence of executed processes.

Another important takeaway was learning how process tree analysis can quickly identify the origin of suspicious commands, making it one of the most valuable investigation techniques for Linux-based incident response.

---

## Conclusion

The **Linux Threat Detection 1** room provided practical experience analysing Linux logs from a defender's perspective. It strengthened my understanding of detecting initial access techniques, investigating compromised services, and reconstructing attacker behaviour using authentication logs, application logs, and audit data. These skills are directly applicable to Security Operations Center (SOC) investigations, threat hunting, and incident response.
