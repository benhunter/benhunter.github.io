---
title: Cybersecurity Primer
pubDate: '2025-10-11'
---
# How to Think About Cybersecurity

Cybersecurity is a broad discipline full of jargon and opaque terms. This Primer helps practitioners think holistically about security. Instead of defining every term, the goal is to establish relationships between concepts. This becomes a framework for thinking.

Along the way we ask questions to enrich understanding.

# Security Objectives 

CIA

- Confidentiality
- Integrity
- Availability

The CIA triad is the foundational concept for all cybersecurity.

Ask

- Who is allowed access to information?
- Has information been modified?
- Can the service be used when needed?

# Strategies

Three strategies for understanding Cybersecurity:

- threat-based
- risk-based
- systems-based

Ask

- What will the adversary do?
- What risk can we accept?
- How is the system designed?

## Threat Modeling

Red Teaming

- What can an adversary do?

Insider Threats

- Usually worst case scenario, hard to detect. Attacker wants to hijack real accounts and become the insider.

Attack Surface

- Where are we exposed?

Social Engineering

- People are often the weak link.

## Risk Management

- Assessment
- Authorization
- Compliance

## Systems Engineering

- Data
- Users
- Software
- Hardware
- Network

Understand the system. What is in it, how they interact.

Systems include:

- Data - category, classification, types
- Users - roles, permissions, administrators/privileged/root/super
- Software - where did it come from? supply chain, who made it, what does it do? how is it configured?
- Hardware - inventory, physical access, supply chain, cloud/IaaS
- Network - Ports, Protocols, Services (PPSM)

# When are you secure enough?

Security is rarely provable in a formal, mathematical way.

You are convincing someone else that your system is secure enough. Or someone has to convince you that the system is secure enough.
- meet a specific goal (like a STIG item)
- address some known risk
- overall posture is acceptable
- provide evidence or artifacts
- trace the control through its entire implementation and check against evidence
- who has authority to accept risk

# Principles

- Least Privilege
- Defense in Depth
- Separation of Duties
- Fail safe
	- Deny by default
	- Allow list
	- Redundancy, replication
	- Denial of Service
- Secure by Design
- Simple (economy of mechanism)
- Usable
- Resilient
- Minimize Attack Surface

# Concepts

- Identity
	- Identity Provider
	- Authentication
	- Authorization
- Security boundary, Authorization boundary
- Non-repudiation - proof someone did something
- Trust - Considered risky, be skeptical, always verify
- Zero-Trust - verify every action
- Inheritance - a stack of security objectives where one component depends on another
- Encryption
	- Data in transit
	- Data at rest
	- Data in process
	- Hashing
	- Signatures
- Read versus Write

# Access Control

Who is allowed to access what?

- how do we enforce it?
	- Identity > Authentication > Authorization
	- Business rules
	- Encryption
- how do we know it's working?
	- Audit logs
- how do we know when it's not?
	- Testing, Automated test (unit, integration, etc), Penetration Tests
- what are they allowed to do?
	- Read, Write

Examples of who:
- a person
- a computer
- an identity, role, or group
- could be delegated to person or computer

Access Control patterns
- Passwords
- Key, token, secret. Sometimes API is put in front of it. These are all just passwords.
- OAuth
- SAML
- Kerberos
- PKI
- Permissions models
	- Role Based (RBAC)

# Change Management

- Change Control Board
- ensure all changes maintain the desired security posture of the system

# Incidents & Recovery

- Audit logs
- Monitoring - people checking things
- Alerting - automation checking things
- Backups

# Risk Management Framework

Every system must be Assessed and Authorized. An Authority to Operate (ATO) specifies the controls that must be implemented.

System is defined by a boundary and what is in it.

- Information types
- Who can access
- What components
- Connections. In/out, relationships with other systems

Sound familiar? This is restatement of the Systems Engineering Strategy: understand Data, Users, Software, Hardware, Network

Controls are the safeguards or countermeasures prescribed for an information system or an organization to protect the confidentiality, integrity, and availability of the system and its information.

- 20 control families
- around 1200 unique controls
- Control selection prioritizes which controls to implement
- Control assessment determines whether a control is implemented
- Inheritance makes this manageable
- Informally, a control, simply asks a question.

Risk Assessment

- Threat
- Impact
- Likelihood

STIG

- Secure Technical Implementation Guides (STIG)
- Standardizes the questions to ask during Assessment
- Maps directly to the controls

# Scenarios

- New data type added to an application
- New user personal added to an application
- New network connection from an application
- New application deployed
- New service in cloud account
- New platform in cloud
- New system on tactical hardware
- New plugin to an application

Techniques
- Identify risks
- Build threat model
- Map attack surface
- Design defenses
- Apply security controls

|Risk|Impact|Likelihood|Controls, Mitigations|
|-|-|-|-|
| | | | |

# Links

- https://en.wikipedia.org/wiki/Information_security
- Security principles https://chatgpt.com/share/68e9617a-6f90-800a-899d-f4181e358ba9
- Authentication Protocols https://chatgpt.com/share/68e95cea-0f1c-800a-b64d-50283e814922
