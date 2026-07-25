# DaveTraceTech

**Track your cards. Stop the fraud.**

DaveTraceTech is an early-stage cybersecurity and card-fraud prevention project founded by **David Aguoru**. It is being developed to help credit and debit card users identify suspicious activity, secure affected cards, understand where their cards were last used and organise useful evidence for authorised fraud investigations.

> **Development status:** DaveTraceTech is currently a working front-end prototype using fictional data. It is not connected to live banks, card networks, police systems, payment processors or location services.

---

## Table of Contents

- [The Problem](#the-problem)
- [The Solution](#the-solution)
- [Core Features](#core-features)
- [How DaveTraceTech Would Work](#how-davetracetech-would-work)
- [Emergency Fake Password Policy](#emergency-fake-password-policy)
- [Perpetrator Attribution](#perpetrator-attribution)
- [Card Location Explained](#card-location-explained)
- [Target Users](#target-users)
- [Banks and Fintech Partnerships](#banks-and-fintech-partnerships)
- [Privacy, Security and Compliance](#privacy-security-and-compliance)
- [Current Prototype](#current-prototype)
- [Technology](#technology)
- [Development Roadmap](#development-roadmap)
- [Business Model](#business-model)
- [Founder](#founder)
- [Disclaimer](#disclaimer)

---

## The Problem

Card-fraud victims may need to review transactions, freeze their card, contact their bank, preserve evidence, submit a report and follow an investigation across several separate services.

This can make responding to fraud stressful, fragmented and time-consuming. Delays may also give criminals further opportunities to attempt transactions or compromise other financial accounts.

DaveTraceTech aims to create one dedicated card-security experience that helps users:

- Detect suspicious card activity earlier.
- Understand why activity has been flagged.
- Secure the affected card.
- Review where and when the card was used.
- Preserve useful transaction information.
- Report the incident through authorised channels.
- Follow the progress of a fraud case.

---

## The Solution

DaveTraceTech is intended to provide a central card-security dashboard that combines fraud alerts, authentication, transaction-location context, emergency security controls and incident case tracking.

The platform is not intended to replace banks, police forces or regulated payment providers. Its purpose is to operate alongside them as a security and evidence-support layer.

When suspicious activity is detected, DaveTraceTech could display:

- The affected card using masked digits.
- The transaction amount.
- The merchant name.
- The transaction time.
- The payment method.
- The available merchant location.
- The reason the activity was flagged.
- A transparent fraud-risk level.
- Options to recognise or report the activity.
- Recommended security actions.

If the user reports an event as unrecognised, DaveTraceTech could create a structured incident timeline and, through a future approved integration, help notify the relevant card issuer.

---

## Core Features

### Real-Time Fraud Alerts

DaveTraceTech is designed to warn users about unusual or potentially unauthorised card activity.

Potential warning signals could include:

- An unusual transaction amount.
- Activity at an unexpected location.
- Repeated declined payments.
- Several transactions within a short period.
- An unfamiliar merchant.
- Suspicious online payment activity.
- A payment made after the card was reported missing.
- Unusual account, device or sign-in behaviour.

Alerts should explain why an event was flagged rather than presenting an unsupported conclusion.

### Card Security Dashboard

The dashboard may display:

- Protected cards.
- Masked card numbers.
- Card status.
- Recent activity.
- Active fraud alerts.
- Open incident cases.
- Security recommendations.
- Transparent fraud-risk scores.

DaveTraceTech should never reveal a full PIN, CVV, security code or complete card number.

### Card Freeze Controls

Through an approved issuer integration, users could freeze or unfreeze an affected card from the DaveTraceTech interface.

The current prototype only simulates this action. It does not send instructions to a bank or payment network.

### Card-Use Location Context

DaveTraceTech is intended to show the available location associated with a card transaction.

This could include:

- Merchant name.
- Merchant address.
- Approximate transaction location.
- Transaction time.
- Transaction amount.
- Payment method.
- Whether the user recognises the activity.

This feature represents the location of card use rather than continuous GPS tracking of the physical card.

### Voice-Verification Concept

The proposed voice-verification feature asks the user to say:

> “I am” followed by their full name.

Voice verification would operate as one authentication factor and would not be treated as infallible proof of identity.

The proposed safeguards include:

- Voice recordings should not be unnecessarily retained.
- Microphone access must require permission.
- Voice verification should be combined with MFA.
- Replay and AI-generated voice attacks must be considered.
- Failed attempts must be rate-limited.
- Users must have an accessible alternative login method.

The current prototype does not record a user’s voice or request microphone access.

### Multi-Factor Authentication

DaveTraceTech is intended to support multiple authentication factors, including:

- A password or secure passcode.
- A registered device.
- A one-time verification code.
- Operating-system biometrics.
- Optional voice verification.
- Additional risk-based security checks.

The proposed policy includes a maximum of three failed verification attempts within a three-hour period.

### Case Tracking

When suspicious activity is reported, DaveTraceTech could create a case containing:

- A unique case reference.
- The affected masked card.
- Disputed transactions.
- Transaction timestamps.
- Merchant and location information.
- The user’s response.
- Security actions taken.
- Communications with authorised organisations.
- Supporting evidence.
- Investigation status.
- Final outcome.

Possible case statuses could include:

- Alert received.
- Awaiting user review.
- Card secured.
- Report prepared.
- Sent to issuer.
- Evidence under review.
- Further information required.
- Resolved.
- Closed.

### Fraud-Awareness Hub

A future version may provide guidance about:

- Card theft.
- Contactless fraud.
- Phishing.
- Smishing.
- Vishing.
- Social engineering.
- Online shopping fraud.
- Account takeover.
- Digital-wallet security.
- Safe fraud-reporting procedures.

---

## How DaveTraceTech Would Work

1. The user securely signs in using MFA and their configured authentication methods.
2. A supported card is connected through an approved banking integration.
3. Authorised services provide relevant transaction or security events.
4. Suspicious activity generates a transparent alert.
5. The user marks the activity as recognised or unrecognised.
6. DaveTraceTech recommends protective actions.
7. The affected card may be secured through an approved issuer API.
8. A structured incident timeline is created.
9. Relevant evidence can support an authorised bank or police investigation.
10. The user can follow the progress and outcome of the case.

DaveTraceTech would not automatically treat a risk score as proof that fraud occurred.

---

## Emergency Fake Password Policy

The **Emergency Fake Password Policy**, or **EFPP**, is a proposed security feature for situations where a user is being threatened or forced to unlock the application.

The user could enter a predefined emergency credential that appears to unlock a believable restricted version of the app. Behind the scenes, an approved production system could initiate a protected response workflow.

Depending on legal, safety and partnership approval, this might include:

- Recording that a duress credential was used.
- Restricting access to sensitive information.
- Displaying a neutral interface.
- Increasing monitoring of subsequent account activity.
- Preparing an alert for an authorised recipient.
- Preserving relevant security-event information.
- Requiring a separately verified recovery process.

The current prototype only demonstrates the interface. It does not contact banks, trusted contacts, police forces or emergency services.

A production version would require:

- Specialist threat modelling.
- Safety and abuse-case testing.
- Clear opt-in setup.
- False-activation procedures.
- Secure recovery controls.
- Bank and partner approval.
- Legal and data-protection review.

EFPP must never be described as guaranteeing personal safety or an emergency-service response.

---

## Perpetrator Attribution

DaveTraceTech is intended to help authorised investigators develop evidence-based leads. It should not claim to identify or accuse a perpetrator automatically.

The proposed feature is called:

> **DaveTrace Investigate — an evidence-correlation and investigative lead system for authorised card-fraud investigations.**

Its purpose would be to help answer:

- Where and when was the card used?
- Which merchant terminal processed the transaction?
- Was the payment contactless, chip-and-PIN, online or an ATM withdrawal?
- Which device, account, IP address or delivery address was involved?
- Are several fraudulent events connected?
- What evidence should the bank or police request next?
- Is there enough information to create an investigative lead?

### Proposed Attribution Process

1. The cardholder reports a transaction as unrecognised.
2. DaveTraceTech creates a tamper-evident case.
3. Authorised transaction and security information is collected.
4. Locations, terminals, accounts, devices and events are correlated.
5. Possible connections are presented as investigative leads.
6. A trained human investigator reviews the result.
7. The bank or police requests additional evidence through lawful channels.
8. Only an authorised organisation verifies the identity of a suspect.

### Possible Evidence Sources

| Evidence source | What it may establish | Main limitation |
|---|---|---|
| Merchant terminal | Where and when a card was used | Does not identify the individual |
| ATM identifier | Location and time of a withdrawal | Requires operator cooperation |
| CCTV | Who may have been present | Requires lawful merchant or police access |
| IP address | Network used for an online event | May be shared, approximate or masked |
| Device fingerprint | Repeated use of the same device | Identifies a device, not necessarily its owner |
| Delivery address | Destination of purchased goods | Could be a drop or innocent address |
| Customer account | Account used for an order | Could be compromised or created using false details |
| Phone or email | Contact details used in a transaction | May be disposable, stolen or falsified |
| Digital-wallet token | Wallet or device involved | Requires issuer or wallet-provider cooperation |
| Witness statement | Context surrounding an incident | May be incomplete or mistaken |

No single signal should be treated as proof of identity.

### Evidence Correlation

DaveTrace Investigate could identify patterns such as:

- Several stolen cards used at the same terminal.
- Multiple disputed orders using the same device.
- Different fraud cases sharing a delivery address.
- One IP address appearing across several suspicious accounts.
- Repeated use of the same phone number or email.
- Transactions following a similar geographical route.
- ATM withdrawals occurring shortly after card theft.
- Multiple suspicious events involving the same digital-wallet token.

These connections would be presented as leads requiring human verification.

### Evidence-Strength Levels

DaveTraceTech should use evidence levels rather than displaying a misleading “perpetrator identified” score.

#### Level 1: Event Located

The merchant, time, transaction channel or ATM has been established.

#### Level 2: Repeat Signal Detected

The same device, terminal, address or other signal appears in multiple suspicious events.

#### Level 3: Investigative Lead

Several independent signals suggest that the events may be connected.

#### Level 4: Identity Lead

An authorised organisation has linked the event to an identifiable account or person, but further verification is required.

#### Level 5: Authority-Verified Identity

A bank, police force or authorised investigator has confirmed the identity using properly obtained evidence.

Every result should explain:

- Which signals contributed.
- Where the information came from.
- How reliable each signal is.
- What alternative explanations exist.
- What evidence remains missing.
- Who reviewed the conclusion.

### CCTV Preservation

DaveTraceTech could create a CCTV preservation notice containing:

- Merchant or ATM location.
- Transaction timestamp.
- Relevant recording window.
- Terminal or ATM reference.
- Case number.

The notice would help an authorised bank or police investigator request that footage be preserved before it is overwritten.

DaveTraceTech would not directly obtain private CCTV without proper authority.

### Online Transaction Tracing

For online card fraud, authorised investigators may need information such as:

- Order-account details.
- Delivery or collection address.
- Device and session identifiers.
- IP logs.
- Account-creation time.
- Delivery-information changes.
- Payment-authentication results.
- Courier tracking.
- Proof-of-delivery information.
- Collection-point CCTV.

DaveTraceTech could organise these requests but should not obtain the information by bypassing merchant security or access controls.

### Secure Evidence Package

DaveTraceTech could generate a structured evidence package containing:

- Case reference.
- Event timeline.
- Transaction references.
- User statement.
- Card-freeze timestamp.
- Merchant and location information.
- Related-event connections.
- Evidence-source descriptions.
- File hashes.
- Access history.
- Outstanding evidence requests.
- Investigator notes.

Each item should record who supplied it, when it was received, whether it was modified, who accessed it and when it should be deleted.

### Human Review

DaveTraceTech must never:

- Publicly name a suspected perpetrator.
- Tell a user that a named person is guilty.
- Report somebody based only on an algorithm.
- Treat an IP address as proof of identity.
- Encourage users to confront a suspected offender.
- Publish a suspect’s photograph, address or personal details.
- Conduct covert facial recognition.
- Make a significant accusation without human review.

The UK GDPR restricts solely automated decisions that have legal or similarly significant effects. Any attribution system would therefore require meaningful human oversight.

### Facial Recognition

Facial recognition should not be an early DaveTraceTech feature.

Using a face to uniquely identify someone involves sensitive biometric processing and creates significant risks involving:

- False matches.
- Bias.
- Innocent people being flagged.
- Surveillance.
- Special-category data.
- Unlawful CCTV reuse.
- Excessive retention.
- Automated accusations.

A safer process would be:

1. DaveTraceTech records that CCTV may exist.
2. Police or another authorised body obtains the footage lawfully.
3. Trained investigators assess the footage.
4. Any biometric comparison takes place within an authorised process rather than the consumer app.

### Product Wording

DaveTraceTech should say:

> DaveTrace Investigate correlates authorised transaction, merchant, device and location signals to help banks and police develop evidence-based leads. It does not accuse or identify individuals without independent human verification.

DaveTraceTech should not claim:

> DaveTraceTech automatically tracks down and identifies fraudsters.

---

## Card Location Explained

Standard credit and debit cards do not normally contain independent GPS technology. DaveTraceTech therefore does not claim to provide continuous physical GPS tracking of an ordinary card.

Its proposed location feature would display available information connected to card use, such as:

- Merchant name and address.
- Transaction time and amount.
- Approximate merchant location.
- ATM location.
- Authorised device or transaction metadata.

Important distinctions include:

- **Physical GPS tracking** requires dedicated hardware.
- **Transaction-location context** may come from merchant information.
- **Device location** requires permission from the device owner.
- **IP-based location** is approximate and may be inaccurate.
- **Transaction location** does not independently identify the person who used the card.

---

## Target Users

DaveTraceTech is intended for:

- Individual credit and debit card users.
- Young adults and first-time cardholders.
- Frequent contactless-payment users.
- Online shoppers.
- Travellers.
- Previous victims of card theft or fraud.
- Banks, fintech companies and card issuers.
- Businesses managing employee cards or expenses.
- Authorised fraud-investigation teams.

---

## Banks and Fintech Partnerships

DaveTraceTech is intended to work alongside banks rather than replace them.

Live functionality would require:

- Formal bank or fintech partnerships.
- Approved APIs.
- Commercial agreements.
- Strong customer authentication.
- Data-sharing agreements.
- Security architecture reviews.
- Penetration testing.
- Data-protection assessments.
- Regulatory and legal review.
- Incident-response procedures.
- Service-level agreements.
- Operational resilience testing.

DaveTraceTech must not be described as endorsed by a bank, card network or police force unless a formal relationship has been established.

---

## Privacy, Security and Compliance

DaveTraceTech is being designed around consent, transparency, data minimisation and secure handling.

Potentially sensitive information may include:

- Transaction details.
- Masked card information.
- Location context.
- Authentication events.
- Device information.
- IP addresses.
- Fraud reports.
- Case evidence.
- Voice or biometric information.
- Information concerning suspected criminal activity.

A production UK service would need to consider:

- UK GDPR.
- Data Protection Act 2018.
- Applicable financial-services requirements.
- Criminal-offence data rules.
- Special-category data requirements.
- Automated-decision restrictions.
- Appropriate consent and lawful bases.
- Data-sharing agreements.
- Retention and deletion obligations.

Processing information about suspected offenders receives additional legal protection. DaveTraceTech would need a documented lawful basis and an applicable condition before processing criminal-offence data.

A **Data Protection Impact Assessment** would likely be required before introducing high-risk processing involving financial, behavioural, biometric or location information.

### Security Controls

A production platform would require:

- Encryption in transit and at rest.
- Secure key management.
- Strong API authentication.
- Least-privilege access.
- Role-based permissions.
- Multi-factor authentication.
- Rate limiting.
- Secure account recovery.
- Audit logging.
- Vulnerability scanning.
- Penetration testing.
- Mobile application security testing.
- Secure backups.
- Incident response.
- Access reviews.
- Retention and deletion procedures.
- Tamper-evident evidence records.

Full card numbers, PINs, CVVs, passwords, private keys and production credentials must never be stored in this public repository.

---

## Current Prototype

The current prototype demonstrates:

- A responsive card-security dashboard.
- Fictional protected cards.
- Fictional transactions.
- Simulated card freezing.
- Fraud-alert review and response.
- Fictional merchant-location context.
- Incident case tracking.
- EFPP simulation.
- MFA settings.
- Voice-verification settings.
- Fraud-risk indicators.
- Mobile and desktop navigation.

The prototype does **not**:

- Connect to real bank accounts.
- Process payments.
- Freeze a real card.
- Track a physical card.
- Record a user’s voice.
- Identify or track a fraudster.
- Access private merchant records.
- Obtain CCTV footage.
- Contact banks, police or emergency services.
- Guarantee that fraud will be prevented or recovered.

All names, transactions, locations, alerts, risk scores and cases displayed in the prototype are fictional.

---

## Technology

The mobile prototype uses:

- React Native.
- Expo.
- JavaScript.
- Responsive cross-platform components.

The website prototype uses:

- HTML.
- CSS.
- JavaScript.

A production platform would require:

- Android and iOS applications.
- A secure backend.
- Identity and access management.
- Encrypted databases.
- Authorised banking APIs.
- Fraud-alert processing.
- Case-management services.
- Evidence and audit systems.
- Consent and privacy management.
- Monitoring and incident response.
- Protected bank, investigator and administrative portals.

Production architecture and technologies may change following security, legal and partnership reviews.

---

## Development Roadmap

### Phase 1: Concept Validation

- Build the website and app prototype.
- Demonstrate fraud-alert workflows.
- Test the EFPP concept.
- Gather user feedback.
- Improve product messaging.
- Research legal and regulatory requirements.

### Phase 2: Technical Planning

- Define product requirements.
- Design the production architecture.
- Conduct threat modelling.
- Map proposed data flows.
- Complete a DPIA.
- Define bank-integration requirements.
- Establish a secure development lifecycle.

### Phase 3: Controlled MVP

- Build secure authentication.
- Develop the protected backend.
- Use synthetic test information.
- Implement case tracking.
- Add tamper-evident event logging.
- Build evidence exports.
- Conduct accessibility and security testing.

### Phase 4: Attribution Assistance

- Introduce transaction and terminal references using test APIs.
- Build authorised evidence-correlation tools.
- Add human investigator review.
- Develop CCTV preservation workflows.
- Test related-event detection using synthetic data.
- Establish lawful evidence-sharing procedures.

### Phase 5: Partnership Pilot

- Secure a bank or fintech partner.
- Complete due diligence.
- Integrate approved APIs.
- Run a controlled pilot.
- Monitor false positives.
- Test support procedures.
- Obtain independent legal and security reviews.

### Phase 6: Public Launch

- Release through official app stores.
- Provide customer support.
- Monitor performance and security.
- Respond to vulnerabilities.
- Expand compatible institutions gradually.
- Continue fraud-awareness education.

Roadmap dates depend on funding, resources, partnerships, technical testing and regulatory approval.

---

## Business Model

Potential revenue streams include:

- Free consumer accounts.
- Premium card-security subscriptions.
- Monthly or annual plans.
- Bank and fintech licensing.
- Enterprise security packages.
- API access.
- White-label integrations.
- Fraud-awareness and training services.
- Partner implementation and support.

---

## Repository Safety

This repository must not contain:

- Real card numbers.
- PINs.
- CVVs or security codes.
- Bank passwords.
- Customer financial records.
- Production API keys.
- Signing certificates.
- Private encryption keys.
- Real fraud evidence.
- Unauthorised location information.
- Identifiable information about suspected offenders.

Use environment variables and an appropriate secret-management system for sensitive configuration.

If credentials are accidentally committed to GitHub, they should be revoked and replaced immediately.

---

## Founder

DaveTraceTech was founded by **David Aguoru**, a Cyber Security and Digital Forensics graduate from Kingston University.

David developed DaveTraceTech from his interest in cybersecurity, financial protection, digital forensics and user-focused fraud prevention.

The project became a finalist in Kingston University’s Bright Ideas Competition among approximately 500 competitors.

---

## Disclaimer

DaveTraceTech is an early-stage prototype. It does not currently provide live banking, payment processing, physical card tracking, fraud investigation, criminal identification or emergency services.

Features described in this README may be simulated, under development or dependent on future partnerships, security testing, legal assessment and regulatory approval.

Transaction locations, IP addresses, device signals, addresses and algorithmic scores do not independently prove a person’s identity or guilt.

Users should contact their bank immediately if a real card or account may have been compromised. Where there is an immediate threat to personal safety, users should contact the appropriate emergency service.

---

