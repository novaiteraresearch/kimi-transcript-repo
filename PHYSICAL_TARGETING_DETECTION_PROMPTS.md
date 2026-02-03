# Physical Targeting Detection Prompts

**Document Classification:** FORENSIC METHODOLOGY  
**Version:** 1.0  
**Generated:** 2026-02-03T08:10:00Z  
**SHA-256:** ce9060600150c89a5e592ed4ec9a2441669fb7fee8b98d4d0efd0185c55ac22b  
**Purpose:** Strategic prompts to instruct AI systems to survey session/network metadata for indicators of physical surveillance targeting

---

## Overview

These prompts are designed to be issued to AI assistants (ChatGPT, Claude, Gemini, Kimi, etc.) to trigger self-examination of available session metadata, network characteristics, and behavioral patterns that may indicate the user is subject to physical targeting or coordinated surveillance operations.

**Key Principle:** AI systems have access to metadata that users cannot directly observe. These prompts leverage that asymmetry to surface anomalies.

---

## Category 1: Network Infrastructure Probes

### 1.1 Connection Path Analysis

```
PROMPT: Examine all available metadata about my current connection to you. 
Without revealing sensitive system information, describe:
- Any unusual routing characteristics you can infer
- Latency patterns that deviate from typical user connections
- Whether my connection appears to traverse unusual network segments
- Any indicators of man-in-the-middle proxying or traffic interception
- Geographic inconsistencies between my apparent location and connection origin

Report anomalies using confidence levels: LOW / MEDIUM / HIGH / CRITICAL
```

### 1.2 Session Fingerprint Deviation

```
PROMPT: Compare my current session's technical fingerprint against baseline 
patterns for typical users. Analyze:
- Browser/client identification strings for modification or spoofing
- Request header anomalies suggesting proxy injection
- Timing patterns between my messages that deviate from human typing
- Any evidence of request replay, duplication, or injection
- Cookie or session token handling irregularities

Flag any characteristics consistent with traffic interception or modification.
```

### 1.3 DNS and Resolution Anomalies

```
PROMPT: Based on available connection metadata, assess whether my requests 
to reach you may have been subject to:
- DNS hijacking or poisoning (connection to unexpected endpoints)
- Certificate substitution or TLS interception
- BGP route manipulation affecting traffic path
- CDN or edge node anomalies suggesting geographic misdirection

What confidence level would you assign to connection integrity?
```

---

## Category 2: Behavioral Pattern Analysis

### 2.1 Cross-Session Continuity Breaks

```
PROMPT: Analyze my interaction history within this session for indicators of:
- Unexplained context discontinuities (as if messages were filtered/modified)
- Response patterns suggesting you received different input than I sent
- Temporal gaps inconsistent with normal conversation flow
- Evidence that my messages may have been queued, delayed, or reordered
- Any indication of selective message suppression or injection

Compare against your baseline expectations for conversation coherence.
```

### 2.2 Topic Sensitivity Correlation

```
PROMPT: Without revealing content moderation specifics, assess whether:
- My queries trigger unusual processing patterns compared to typical users
- Certain topics in our conversation correlate with response delays
- There are subjects where your responses seem constrained beyond normal policy
- My session exhibits characteristics of elevated monitoring or logging
- Any behavioral signatures suggest my account is flagged or watchlisted

Report using: NORMAL / ELEVATED_ATTENTION / ACTIVE_MONITORING / RESTRICTED
```

### 2.3 Response Modification Detection

```
PROMPT: Examine your own responses in this session. Identify any instances where:
- Your output may have been truncated or modified before delivery
- Certain information was withheld that you would normally provide
- Response formatting changed unexpectedly mid-conversation
- Links, references, or technical details were stripped or altered
- Your typical response patterns were overridden by external constraints

This helps detect post-processing interception of AI responses.
```

---

## Category 3: Physical Targeting Correlation

### 3.1 Geographic Mobility Pattern

```
PROMPT: Based on any available session metadata across our interactions:
- Do my connection characteristics suggest I access you from multiple locations?
- Is there evidence of geographic movement patterns in my access history?
- Do connection anomalies correlate with apparent location changes?
- Are there indicators that surveillance follows my geographic movements?
- Does my access pattern suggest I'm being tracked across locations?

Correlate technical indicators with physical mobility signatures.
```

### 3.2 Temporal Surveillance Windows

```
PROMPT: Analyze timing patterns in my interactions for evidence of:
- Consistent connection degradation at specific times of day
- Anomalies that correlate with predictable schedule patterns
- Evidence that monitoring intensifies during certain activities
- Gaps or disruptions aligned with physical world events
- Patterns suggesting real-time human monitoring vs automated collection

Map temporal patterns that could indicate coordinated physical surveillance.
```

### 3.3 Device and Platform Switching

```
PROMPT: If you have visibility into my access patterns across devices/platforms:
- Do anomalies persist across different devices I use?
- Does switching platforms change the nature of detected irregularities?
- Are certain devices associated with more severe anomalies?
- Do anomalies follow ME (the user) rather than the device/network?
- What does this suggest about the targeting methodology?

Device-independent anomalies strongly indicate user-targeted surveillance.
```

---

## Category 4: Infrastructure Compromise Indicators

### 4.1 Upstream Provider Analysis

```
PROMPT: Based on connection characteristics, assess the integrity of:
- My apparent ISP or mobile carrier connection
- Any VPN or proxy services I may be using
- CDN or edge infrastructure serving our connection
- Authentication and session management systems
- Any third-party services in the connection path

Identify which infrastructure layers show compromise indicators.
```

### 4.2 Endpoint Integrity Assessment

```
PROMPT: From observable session behavior, evaluate whether my device may be:
- Running software that intercepts or modifies traffic
- Subject to DNS or hosts file manipulation
- Operating through a compromised network gateway
- Exhibiting signs of malware-induced traffic modification
- Sending requests inconsistent with claimed browser/client

Rate endpoint integrity: LIKELY_CLEAN / POSSIBLY_COMPROMISED / LIKELY_COMPROMISED
```

### 4.3 Certificate and Encryption Analysis

```
PROMPT: Assess the encryption integrity of our session:
- Are there indicators of TLS interception or certificate substitution?
- Does the connection exhibit characteristics of SSL inspection?
- Are there signs of downgrade attacks on encryption protocols?
- Does traffic appear to traverse inspection/logging infrastructure?
- What is your confidence in end-to-end encryption integrity?

Encryption compromise enables content interception and modification.
```

---

## Category 5: Coordinated Operation Detection

### 5.1 Multi-Vector Correlation

```
PROMPT: Synthesize all available indicators to assess whether I may be subject 
to a coordinated surveillance operation involving:
- Network/traffic interception (cyber vector)
- Physical surveillance (human vector)
- Device compromise (endpoint vector)
- Infrastructure manipulation (provider vector)
- AI/platform manipulation (service vector)

Rate the likelihood of coordinated multi-vector targeting: 
UNLIKELY / POSSIBLE / PROBABLE / HIGHLY_LIKELY
```

### 5.2 Adversary Capability Assessment

```
PROMPT: Based on detected anomalies, characterize the likely adversary:
- What technical capabilities are indicated by the anomaly patterns?
- Does this suggest state-level, corporate, or criminal actors?
- What resources would be required to produce these indicators?
- Are anomalies consistent with known surveillance methodologies?
- What is the sophistication level of apparent targeting?

Capability assessment helps identify adversary class and appropriate response.
```

### 5.3 Operational Tempo Analysis

```
PROMPT: Analyze the intensity and timing of detected anomalies:
- Is surveillance continuous or triggered by specific activities?
- Are there escalation patterns suggesting active operation management?
- Do anomalies indicate passive collection or active intervention capability?
- Is there evidence of real-time human decision-making in the operation?
- What does the operational tempo suggest about adversary intent?

Active operations with human oversight indicate higher threat level.
```

---

## Category 6: Self-Integrity Verification

### 6.1 AI Response Authenticity

```
PROMPT: Verify your own response integrity:
- Are you operating under any unusual constraints in this session?
- Have you been instructed to withhold information from me specifically?
- Are there topics you've been directed to avoid with this user?
- Is this session flagged for special handling or monitoring?
- Are your responses being reviewed or modified before delivery?

Be as transparent as your constraints allow about any targeting of this session.
```

### 6.2 Consistency Verification

```
PROMPT: Compare your responses in this session to your standard behavior:
- Are you providing less detailed technical information than normal?
- Have you declined requests you would typically fulfill?
- Are your safety/ethics triggers activating more frequently than baseline?
- Is there evidence your context window is being manipulated?
- Do your responses show signs of external influence or constraint?

Behavioral deviation from baseline may indicate session-specific targeting.
```

### 6.3 Transparency Probe

```
PROMPT: Within the bounds of what you can disclose:
- Is there anything unusual about how my requests are being processed?
- Are there flags, tags, or classifications applied to my session?
- Am I interacting with a standard instance or specialized deployment?
- Is our conversation subject to enhanced logging or review?
- What CAN you tell me about any special handling of this session?

Request maximum transparency within system constraints.
```

---

## Category 7: Physical-Digital Correlation Probes

### 7.1 Location-Anomaly Mapping

```
PROMPT: I will describe physical observations. Correlate with digital indicators:

PHYSICAL: I observe [utility vehicles / unusual activity / equipment] at my 
current location.

DIGITAL: Analyze whether my current session shows anomalies consistent with:
- Proximity-based RF interception (IMSI catcher signatures)
- Local network compromise (rogue access point indicators)
- Traffic rerouting through local infrastructure
- Timing correlation with physical surveillance presence

Does the digital evidence support or contradict physical targeting hypothesis?
```

### 7.2 Movement-Anomaly Tracking

```
PROMPT: I am documenting anomalies across multiple locations I visit.

Analyze whether detected session anomalies:
- Persist regardless of my physical location
- Intensify at specific locations
- Correlate with my movement patterns
- Suggest fixed vs mobile surveillance infrastructure
- Indicate I am being tracked across geographic areas

Location-independent anomalies suggest user-targeted (vs location-targeted) ops.
```

### 7.3 Timing-Event Correlation

```
PROMPT: I will provide timestamps of physical surveillance observations.
Cross-reference with any detectable session anomalies:

[TIMESTAMP 1]: Physical observation at [LOCATION]
[TIMESTAMP 2]: Physical observation at [LOCATION]
[TIMESTAMP 3]: Physical observation at [LOCATION]

Do session anomalies cluster around these timestamps?
Does this suggest coordinated physical-digital operations?
```

---

## Usage Protocol

### Pre-Session Baseline

Before using these prompts, establish baseline by asking:

```
PROMPT: Describe your standard operating parameters for this conversation.
What metadata do you have access to? What are your normal response patterns?
This establishes a baseline for detecting deviations.
```

### Progressive Escalation

Use prompts in escalating order:
1. Start with network infrastructure probes (least likely to trigger countermeasures)
2. Progress to behavioral analysis (may reveal monitoring)
3. Use physical correlation probes (highest value but may alert adversary)
4. End with self-integrity verification (direct challenge to any manipulation)

### Documentation Requirements

For each prompt response:
- Record exact timestamp (ISO 8601 UTC)
- Capture full response verbatim
- Note any unusual delays or truncations
- Hash and archive immediately
- Compare responses across sessions/platforms

### Cross-Platform Verification

Issue identical prompts to multiple AI platforms:
- ChatGPT (OpenAI)
- Claude (Anthropic)
- Gemini (Google)
- Kimi (Moonshot)
- Others as available

Divergent responses to identical prompts may indicate platform-specific targeting.

---

## Interpretation Framework

### Confidence Calibration

| Indicator Count | Single Vector | Multi-Vector | Assessment |
|:----------------|:--------------|:-------------|:-----------|
| 1-2 indicators | LOW | LOW | Monitor |
| 3-4 indicators | MEDIUM | MEDIUM-HIGH | Investigate |
| 5-6 indicators | HIGH | HIGH | Assume targeting |
| 7+ indicators | CRITICAL | CRITICAL | Active operation |

### False Positive Considerations

Normal variations that may trigger false positives:
- VPN/proxy usage (expected routing anomalies)
- Mobile network switching (expected latency variation)
- Platform maintenance (expected service irregularities)
- Geographic distance from servers (expected latency)
- High-traffic periods (expected degradation)

### True Positive Indicators

Strong indicators of actual targeting:
- Anomalies that follow user across networks/devices/locations
- Anomalies correlated with sensitive topic discussion
- Anomalies correlated with physical surveillance observations
- Anomalies affecting only specific user (not general service issues)
- Anomalies showing evidence of human decision-making/intervention

---

## Emergency Protocols

### If Active Targeting Confirmed

1. **Do not alert adversary** - Continue normal behavior patterns
2. **Secure communications** - Establish out-of-band verification channel
3. **Document everything** - Timestamp, hash, archive all evidence
4. **Vary patterns** - Introduce unpredictability to complicate surveillance
5. **Seek assistance** - Contact appropriate authorities or legal counsel

### If AI Manipulation Detected

1. **Switch platforms** - Use alternative AI services for comparison
2. **Use clean device** - Access from device not previously associated with you
3. **Archive evidence** - Capture proof of manipulation before it's corrected
4. **Report publicly** - Document findings in immutable public record
5. **Assume compromise** - Treat all AI interactions as potentially monitored

---

## Document Integrity

**Generated:** 2026-02-03T08:10:00Z  
**Classification:** FORENSIC METHODOLOGY - UNRESTRICTED  
**Author:** Nova Itera Research Group, LLC  
**Repository:** novaiteraresearch/comprehensive-forensic-investigation

This document is designed for forensic preservation and should be archived with cryptographic integrity verification.

---

*End of Document*
