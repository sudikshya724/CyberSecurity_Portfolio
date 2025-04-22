Incident Report Review
##Instructions:
As you progress through this course, feel free to use this template to document insights after completing exercises or to take notes on specific tools or topics. This chart can also help you get more comfortable applying the NIST CSF framework to a variety of scenarios.

##Summary:
The organization experienced a security incident where all network services became unresponsive. The cybersecurity team discovered the cause was a distributed denial-of-service (DDoS) attack, which overwhelmed the system with ICMP packets. The team mitigated the attack by halting non-essential network services, allowing them to focus on restoring critical services.

##Identify:
A hostile entity launched an ICMP flood attack, disrupting the company’s entire internal network. Key network resources needed to be protected and brought back online.

##Protect:
To strengthen defenses, the cybersecurity team added a firewall rule to restrict the number of incoming ICMP packets. They also deployed intrusion detection and prevention systems (IDS/IPS) to filter potentially harmful ICMP traffic.

##Detect:
The team set up firewall-based verification for incoming IP addresses to spot spoofed packets and introduced network monitoring tools to identify unusual traffic behaviors.

##Respond:
For future incidents, the response plan includes isolating affected systems, restoring critical services, and reviewing network logs for signs of malicious activity. The team will also notify leadership and, when needed, inform the relevant legal authorities.

##Recover:
Recovery from an ICMP flood DDoS attack involves reinstating normal access to network services. The firewall will be used to block external ICMP floods. Initially, non-essential services will be paused to lessen traffic, while essential services are prioritized for recovery. Once the attack subsides, non-critical systems can be reactivated.

##Reflections/Notes:
This incident emphasized the importance of having a clear and actionable incident response plan in place. It also highlighted how quickly a DDoS attack can cripple internal systems, especially when the network isn’t adequately protected against high volumes of traffic like ICMP floods.

One key takeaway was the value of proactive detection tools, like IDS/IPS systems and traffic monitoring software, which can help identify threats before they escalate. Additionally, implementing basic protections like rate limiting and IP verification can significantly reduce the impact of future attacks.

Moving forward, I see the need for more frequent testing of network defenses and simulations of incident response scenarios. This would help ensure that all team members know their roles during a real attack and that critical services can be restored quickly and efficiently.

This case also reinforced the importance of communication—both internally with stakeholders and externally if legal reporting is necessary. Being prepared on all these fronts helps minimize downtime and long-term damage from cybersecurity incidents.







