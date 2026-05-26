# ATT&CK Gap Analysis Report

**Generated:** 2026-01-17 17:30:35  
**Analysis Version:** 1.0  
**ATT&CK Version:** 18

---

## Executive Summary

This gap analysis evaluates your organization's detection coverage against 8 prioritized threat actors.

### Key Findings

- **Total Techniques Analyzed:** 558
- **Under-Covered Techniques:** 233 (41.8%)
- **Average Gap Score:** -1.24 / 10
- **Maximum Gap:** 12.50

### Gap Distribution

- **LOW:** 88 techniques (15.8%)
- **HIGH:** 124 techniques (22.2%)
- **CRITICAL:** 79 techniques (14.2%)
- **OVER-COVERED:** 220 techniques (39.4%)
- **MEDIUM:** 47 techniques (8.4%)


---

## Threat Actor Profile

The following threat actors were included in this analysis:


### APT29 (Cozy Bear) (Weight: 0.9)

Russian state-sponsored threat actor, LOLBINs focus - FSB

- **Techniques:** 66
- **Average Technique Score:** 3.0 / 5


### APT28 (Fancy Bear) (Weight: 0.7)

Russian state-sponsored threat actor - GRU

- **Techniques:** 91
- **Average Technique Score:** 3.0 / 5


### Turla (Weight: 0.5)

Russian Cyber Espionage, malware focus - FSB

- **Techniques:** 68
- **Average Technique Score:** 3.0 / 5


### APT35 (Magic Hound/Charming Kitten) (Weight: 0.3)

Iranian state-sponsored threat actor targeting EU

- **Techniques:** 79
- **Average Technique Score:** 3.0 / 5


### Operation Ghost (Weight: 0.5)

APT29 campaign against foreign agencies in EU/US

- **Techniques:** 8
- **Average Technique Score:** 3.0 / 5


### Insider Threats - Aggregate (Weight: 1.0)

Insider Threats per CTID and recent events

- **Techniques:** 182
- **Average Technique Score:** 0.5 / 5


### APT29 Diplomatic Phishing (Weight: 0.6)

APT29 diplomatic phishing campaign

- **Techniques:** 51
- **Average Technique Score:** 5.0 / 5


### Turla (Polish NGO specifics) (Weight: 0.8)

Turla targeting Polish NGOs with novel backdoor

- **Techniques:** 0
- **Average Technique Score:** 0.0 / 5



---

## Priority Gaps

The following techniques represent the highest priority gaps (threat presence with insufficient coverage):

|   Priority | Technique ID   | Name                           |   Threat Score |   Coverage Score |   Gap Score | Category   | Tactics                               |
|-----------:|:---------------|:-------------------------------|---------------:|-----------------:|------------:|:-----------|:--------------------------------------|
|        125 | T1583          | Acquire Infrastructure         |            5   |                0 |        12.5 | CRITICAL   | resource-development                  |
|        125 | T1584          | Compromise Infrastructure      |            5   |                0 |        12.5 | CRITICAL   | resource-development                  |
|        125 | T1095          | Non-Application Layer Protocol |            5   |                0 |        12.5 | CRITICAL   | command-and-control                   |
|        125 | T1608.005      | Link Target                    |            5   |                0 |        12.5 | CRITICAL   | resource-development                  |
|        125 | T1573.002      | Asymmetric Cryptography        |            5   |                0 |        12.5 | CRITICAL   | command-and-control                   |
|        125 | T1620          | Reflective Code Loading        |            5   |                0 |        12.5 | CRITICAL   | defense-evasion                       |
|        125 | T1071.004      | DNS                            |            5   |                0 |        12.5 | CRITICAL   | command-and-control                   |
|        108 | T1571          | Non-Standard Port              |            4.3 |                0 |        10.8 | CRITICAL   | command-and-control                   |
|        108 | T1071          | Application Layer Protocol     |            4.3 |                0 |        10.8 | CRITICAL   | command-and-control                   |
|        100 | T1566          | Phishing                       |            5   |                1 |        10   | CRITICAL   | initial-access                        |
|        100 | T1518          | Software Discovery             |            5   |                1 |        10   | CRITICAL   | discovery                             |
|        100 | T1070          | Indicator Removal              |            5   |                1 |        10   | CRITICAL   | defense-evasion                       |
|         91 | T1573          | Encrypted Channel              |            3.7 |                0 |         9.2 | CRITICAL   | command-and-control                   |
|         89 | T1071.001      | Web Protocols                  |            3.6 |                0 |         8.9 | CRITICAL   | command-and-control                   |
|         77 | T1055          | Process Injection              |            4.1 |                1 |         7.7 | CRITICAL   | defense-evasion, privilege-escalation |

---

## Top Composite Threats

The following techniques are most prevalent across your threat landscape:

| Technique ID   | Name                              |   Composite Score |   Actor Count |
|:---------------|:----------------------------------|------------------:|--------------:|
| T1027          | Obfuscated Files or Information   |                 5 |             1 |
| T1584          | Compromise Infrastructure         |                 5 |             1 |
| T1071.004      | DNS                               |                 5 |             1 |
| T1518          | Software Discovery                |                 5 |             1 |
| T1583          | Acquire Infrastructure            |                 5 |             1 |
| T1620          | Reflective Code Loading           |                 5 |             1 |
| T1059          | Command and Scripting Interpreter |                 5 |             1 |
| T1608.005      | Link Target                       |                 5 |             1 |
| T1566          | Phishing                          |                 5 |             1 |
| T1027.009      | Embedded Payloads                 |                 5 |             1 |

---

## Recommendations

### Immediate Actions (Critical/High Gaps)


#### T1583: Acquire Infrastructure

- **Gap Score:** 12.5 / 10
- **Threat Score:** 5.0
- **Current Coverage:** 0 / 5
- **Tactics:** resource-development

**Description:** Adversaries may buy, lease, rent, or obtain infrastructure that can be used during targeting. A wide variety of infrastructure exists for hosting and orchestrating adversary operations. Infrastructure...

**Recommended Actions:**
- Implement detection rules for this technique
- Ensure visibility into PRE platforms
- Review MITRE's detection guidance

---

#### T1584: Compromise Infrastructure

- **Gap Score:** 12.5 / 10
- **Threat Score:** 5.0
- **Current Coverage:** 0 / 5
- **Tactics:** resource-development

**Description:** Adversaries may compromise third-party infrastructure that can be used during targeting. Infrastructure solutions include physical or cloud servers, domains, network devices, and third-party web and D...

**Recommended Actions:**
- Implement detection rules for this technique
- Ensure visibility into PRE platforms
- Review MITRE's detection guidance

---

#### T1095: Non-Application Layer Protocol

- **Gap Score:** 12.5 / 10
- **Threat Score:** 5.0
- **Current Coverage:** 0 / 5
- **Tactics:** command-and-control

**Description:** Adversaries may use an OSI non-application layer protocol for communication between host and C2 server or among infected hosts within a network. The list of possible protocols is extensive.(Citation: ...

**Recommended Actions:**
- Implement detection rules for this technique
- Ensure visibility into ESXi, Linux, macOS platforms
- Review MITRE's detection guidance

---

#### T1608.005: Link Target

- **Gap Score:** 12.5 / 10
- **Threat Score:** 5.0
- **Current Coverage:** 0 / 5
- **Tactics:** resource-development

**Description:** Adversaries may put in place resources that are referenced by a link that can be used during targeting. An adversary may rely upon a user clicking a malicious link in order to divulge information (inc...

**Recommended Actions:**
- Implement detection rules for this technique
- Ensure visibility into PRE platforms
- Review MITRE's detection guidance

---

#### T1573.002: Asymmetric Cryptography

- **Gap Score:** 12.5 / 10
- **Threat Score:** 5.0
- **Current Coverage:** 0 / 5
- **Tactics:** command-and-control

**Description:** Adversaries may employ a known asymmetric encryption algorithm to conceal command and control traffic rather than relying on any inherent protections provided by a communication protocol. Asymmetric c...

**Recommended Actions:**
- Implement detection rules for this technique
- Ensure visibility into ESXi, Linux, macOS platforms
- Review MITRE's detection guidance

---


### Long-Term Strategy

1. **Enhance Detection Coverage:** Focus on techniques with gap scores > 5
2. **Data Source Assessment:** Ensure visibility into key platforms and data sources
3. **Regular Reassessment:** Update this analysis quarterly or after major infrastructure changes
4. **Threat Intelligence Integration:** Continuously update threat actor profiles

---

## Appendix

### Methodology

**Threat Scoring (1-5 scale):**
- 5: Signature/frequent technique for this actor
- 3: Moderately used technique
- 1: Occasionally observed

**Coverage Scoring (1-5 scale):**
- 5: Full detection with automated response
- 3: Manual detection capability
- 1: Minimal visibility

**Gap Scoring (-10 to +10 scale):**
- Positive scores indicate under-coverage (needs improvement)
- Negative scores indicate over-coverage relative to threat
- Gap = (Weighted Threat Score - Coverage Score) normalized to ±10 range

### Data Sources

- **MITRE ATT&CK:** {ATTACK_API['stix']}
- **Coverage Data:** DeTTECT framework
- **Threat Intelligence:** {len(threat_actors)} configured threat actors

---

*Report generated by ATT&CK Gap Analysis Framework*
