# Week 1 — Introduction to Cybersecurity

> Beginner-friendly revision notes based on the Cisco Networking Academy *Introduction to Cybersecurity* course. Rewrite examples in your own words after revision.

## 1. What is cybersecurity?

**Cybersecurity** is the practice of protecting systems, networks, applications and data from unauthorised access, misuse, damage, disruption or theft.

It includes:
- **People:** users, administrators, security analysts and attackers.
- **Processes:** policies, backups, incident response and access reviews.
- **Technology:** firewalls, endpoint protection, encryption and monitoring tools.

**Example:** A company uses multi-factor authentication, endpoint protection and backups to reduce the chance and impact of an account compromise or ransomware incident.

### Important terms
| Term | Meaning | Simple example |
|---|---|---|
| Asset | Something valuable that must be protected | Customer database, laptop, source code |
| Threat | A potential cause of harm | Criminal attempting to steal data |
| Vulnerability | A weakness that could be exploited | Unpatched software |
| Exploit | A method or code that takes advantage of a vulnerability | Code abusing a software flaw |
| Risk | The possibility and impact of a threat exploiting a vulnerability | Likelihood of a server being compromised and the damage caused |
| Attack | An attempt to compromise confidentiality, integrity or availability | Phishing email designed to steal credentials |
| Security control | A safeguard that reduces risk | MFA, firewall, backup |

**Remember the relationship:** A threat may exploit a vulnerability; the resulting risk depends on likelihood and impact. An exploit is a way of taking advantage of a weakness.

## 2. The CIA triad

The CIA triad is a core model for information security.

### Confidentiality
Only authorised people or systems should be able to view information.

- Controls: encryption, access permissions, MFA.
- Example: only HR staff can view employee salary records.
- Failure: an attacker reads confidential customer information.

### Integrity
Information should remain accurate, complete and protected from unauthorised changes.

- Controls: hashes, digital signatures, permissions, audit logs.
- Example: a bank transaction amount must not be altered by an unauthorised person.
- Failure: an attacker changes a payment amount in a database.

### Availability
Systems and information should be accessible to authorised users when needed.

- Controls: backups, redundancy, patching, disaster recovery and DDoS protection.
- Example: an online banking service remains available to customers.
- Failure: a denial-of-service attack makes a website unavailable.

**Quick memory trick:** Confidentiality = who can see it; Integrity = can I trust it; Availability = can I access it?

## 3. Organizational data and why attackers target it

Organisations hold valuable information, including:
- Personally identifiable information (PII): information that can identify a person, such as a name combined with contact details or an identification number.
- Financial data: payment details, bank information and transactions.
- Intellectual property: designs, source code, formulas and trade secrets.
- Credentials: usernames, passwords, tokens and authentication secrets.
- Business operations data: internal documents, plans and customer records.

### Data states
- **Data at rest:** stored on a disk, database, phone or backup.
- **Data in transit:** moving across a network.
- **Data in use:** being processed in memory or by an application.

Different states need suitable protections. For example, disk encryption protects stored data, TLS protects data moving between a browser and a website, and access controls protect data being processed.

## 4. Cyber attackers and motivations

An attacker is a person or group attempting to access, disrupt, alter or steal systems or information.

Common categories:
- **Cybercriminals:** seek money through fraud, ransomware or data theft.
- **Insiders:** employees, contractors or trusted users who misuse legitimate access, intentionally or accidentally.
- **Hacktivists:** attack to promote a social or political cause.
- **Nation-state actors:** state-sponsored groups pursuing espionage, disruption or strategic goals.
- **Script kiddies:** inexperienced attackers who use existing tools or scripts without necessarily understanding them.
- **Competitors / industrial spies:** may seek confidential business information.

Motivation matters because it helps an organisation assess likely targets, methods and impact. These labels are broad categories; real-world attribution can be difficult.

## 5. Cyberwarfare

**Cyberwarfare** refers to cyber operations associated with conflict between nations or state-linked actors. Possible targets include government services, critical infrastructure, communications, energy and financial systems.

Do not assume every cyberattack is cyberwarfare. Many attacks are ordinary criminal activity, espionage or disruption.

## 6. Common attack concepts

### Malware
**Malware** means malicious software designed to harm, disrupt, spy on or gain unauthorised access to a device or system.

| Type | What it does |
|---|---|
| Virus | Attaches to a file/program and spreads when the infected host is run |
| Worm | Self-propagates across systems or networks |
| Trojan horse | Pretends to be legitimate software but performs malicious actions |
| Ransomware | Locks or encrypts data and demands payment |
| Spyware | Secretly monitors activity or collects information |
| Adware | Displays unwanted advertising; some forms also track users |
| Rootkit | Hides malicious activity and may provide privileged access |
| Keylogger | Records keystrokes, potentially capturing passwords |

### Social engineering
Social engineering manipulates people into revealing information or taking unsafe actions.

- **Phishing:** deceptive messages, often email, that try to steal data or deliver malware.
- **Spear phishing:** phishing tailored to a specific person or organisation.
- **Whaling:** phishing targeting senior executives or other high-value individuals.
- **Vishing:** voice-call-based deception.
- **Smishing:** SMS/text-message-based deception.
- **Pretexting:** inventing a believable story or identity to gain trust.
- **Baiting:** offering something attractive to trick a victim into unsafe action.
- **Tailgating:** following an authorised person into a restricted physical area.

**Warning signs:** unexpected urgency, suspicious links or attachments, requests for passwords or OTPs, mismatched sender addresses, unusual payment instructions and unexpected login prompts.

### Other attack terms
- **DoS (Denial of Service):** attempts to make a service unavailable.
- **DDoS (Distributed Denial of Service):** DoS traffic comes from many systems or sources.
- **Man-in-the-Middle (MitM):** an attacker intercepts or potentially alters communication between parties.
- **Brute-force attack:** repeatedly tries possible passwords or keys.
- **Credential stuffing:** tries username/password pairs leaked from other services.
- **Spoofing:** disguises identity or source information, such as a sender address or IP address.
- **Eavesdropping/sniffing:** capturing network communications; encryption helps protect their contents.
- **SQL injection (SQLi):** malicious input manipulates an application's database query.
- **Cross-site scripting (XSS):** attacker-controlled script executes in another user's browser in the context of a vulnerable website.

## 7. Vulnerabilities, exploits and the attack surface

- **Vulnerability:** a weakness in software, hardware, configuration or process.
- **Exploit:** a technique or code that uses a vulnerability.
- **Patch:** an update that fixes bugs or security weaknesses.
- **Misconfiguration:** an insecure setting, such as a publicly exposed storage bucket.
- **Attack surface:** all the points where an attacker could try to enter or affect a system, including applications, devices, accounts and exposed services.
- **Zero-day vulnerability:** a vulnerability for which a fix is not yet available to the affected users, or which is being exploited before a patch is available. Usage can vary by context.

**Example:** An internet-facing server runs outdated software (vulnerability). An attacker uses a known exploit against it (exploitation). Applying the vendor's security patch reduces that exposure.

## 8. Protecting devices, networks and privacy

### Personal security practices
- Use long, unique passwords; use a password manager.
- Enable MFA wherever possible.
- Install software and operating-system updates.
- Download applications only from trusted sources.
- Back up important files and test recovery.
- Lock devices and enable device encryption.
- Avoid unknown attachments, links and USB devices.
- Use secure Wi-Fi; avoid sensitive activity on untrusted public networks.
- Review app permissions and privacy settings.
- Share only the personal information necessary.

### Authentication vs authorization
- **Authentication:** verifies who you are. Example: signing in with a password and OTP.
- **Authorization:** decides what an authenticated user is allowed to do. Example: a student can view marks but cannot edit them.

### MFA
**Multi-factor authentication** uses two or more different factor types:
- Something you know: password or PIN.
- Something you have: security key or authenticator device.
- Something you are: fingerprint or face recognition.

Two passwords are not two different factor types.

## 9. Organizational protection and security technologies

Organisations combine technical controls, policies, training and monitoring.

| Technology/control | Purpose |
|---|---|
| Firewall | Allows or blocks network traffic based on rules |
| Antivirus / anti-malware | Detects, blocks or removes malicious software |
| IDS | Intrusion Detection System; monitors and alerts on suspicious activity |
| IPS | Intrusion Prevention System; can detect and actively block suspicious traffic |
| VPN | Creates an encrypted tunnel across an untrusted network |
| Encryption | Makes data unreadable without the appropriate key |
| Access control | Limits who can access resources and what they can do |
| Backup | Provides recoverable copies of data |
| SIEM | Collects and correlates security logs/events to support monitoring and investigation |
| Endpoint protection | Helps secure laptops, desktops, servers and other endpoints |

### Defense in depth
A layered security approach. If one control fails, other controls may still reduce the chance or impact of compromise.

Example layers: MFA, endpoint protection, network segmentation, firewall rules, monitoring, backups and staff awareness.

### Security policies
Written rules that explain how an organisation protects information and how users must behave. Examples include password, acceptable-use, access-control, backup and incident-response policies.

## 10. Legal and ethical issues

- Only test systems when you own them or have explicit permission.
- Follow the scope and rules of an authorised lab or assessment.
- Do not access, copy, modify or share other people's data without permission.
- Protect credentials and confidential information.
- Report vulnerabilities responsibly to the system owner through an approved process.
- Follow applicable laws, contracts and organisational policies.

**Ethical hacking** means testing security with permission, within an agreed scope, and reporting findings responsibly. A tool being publicly available does not make every use of it legal.

## 11. Cybersecurity career awareness

Possible entry-level paths include:
- SOC Analyst L1: monitors alerts, reviews logs and escalates incidents.
- Security Analyst: helps assess risks, investigate issues and improve controls.
- Vulnerability Management Analyst: tracks weaknesses and coordinates remediation.
- Junior Penetration Tester: tests authorised systems for weaknesses.
- Security Engineer: designs, implements and maintains security controls.

Foundational skills include networking, operating systems, security concepts, log analysis, communication, documentation and ethical judgement.

## 12. Quick revision — differences to remember

| Pair | Difference |
|---|---|
| Threat vs vulnerability | Potential cause of harm vs weakness that can be exploited |
| Vulnerability vs exploit | Weakness vs method/code that uses the weakness |
| Virus vs worm | Virus attaches to a host file/program; worm can self-propagate |
| IDS vs IPS | Detects and alerts vs detects and can block |
| Authentication vs authorization | Verifies identity vs grants permissions |
| DoS vs DDoS | One/fewer sources vs distributed sources |
| Encryption vs hashing | Reversible with a key vs designed as a one-way digest |
| Data at rest vs in transit | Stored data vs data moving across a network |

## 13. Self-assessment questions

Try answering these without looking at the notes. Target: at least 16/20.

1. What does cybersecurity protect?
2. Explain confidentiality, integrity and availability with one example each.
3. What is the difference between a threat and a vulnerability?
4. What is an exploit?
5. Name four types of malware and explain them.
6. How is a worm different from a virus?
7. What is phishing? How is spear phishing different?
8. What is social engineering?
9. Explain DoS and DDoS.
10. What is a man-in-the-middle attack?
11. What is the difference between authentication and authorization?
12. What does MFA mean? Give two factor types.
13. What is the difference between IDS and IPS?
14. What is a firewall used for?
15. What is defense in depth?
16. Give examples of data at rest, in transit and in use.
17. What is a zero-day vulnerability?
18. Why are software updates important?
19. What is an attack surface?
20. Why must security testing be authorised?

## 14. Practical activity — build your own threat table

Choose a familiar online service (for example, email or online shopping). Do not test or attack it. Fill in this table as a thinking exercise:

| Asset | Possible threat | Weakness to avoid | Protective control |
|---|---|---|---|
| Email account | Account takeover | Reused password | Unique password + MFA |
| Personal files | Data loss / ransomware | No backup | Offline or protected backup |
| Online shopping account | Payment/account fraud | Fake login page | Verify URL + MFA |

## 15. Week 1 completion checklist

- [ ] I can explain the CIA triad without looking.
- [ ] I can distinguish threat, vulnerability, exploit and risk.
- [ ] I can explain common malware types.
- [ ] I can recognise common social-engineering techniques.
- [ ] I can explain firewall, IDS, IPS, VPN and MFA.
- [ ] I completed the 20-question self-assessment.
- [ ] I wrote one practical threat table in my own words.
- [ ] I uploaded my Cisco badge/certificate image or verification link (without exposing private account details).

## Course reference

Cisco Networking Academy — Introduction to Cybersecurity:
https://www.netacad.com/courses/introduction-to-cybersecurity

The current course outline lists five modules: Introduction to Cybersecurity; Attacks, Concepts and Techniques; Protecting Your Data and Privacy; Protecting the Organization; and Will Your Future Be in Cybersecurity?
