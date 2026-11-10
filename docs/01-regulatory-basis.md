# The Regulatory Basis for Testing Collections Voice Agents in India

James Nazareth
10 November 2026
Version 0.2

---

## Abstract

Indian rules on how a lender may speak to a borrower during loan recovery change on 1 January 2027. The present rules are written as broad standards. The replacement rules are written as twenty-nine numbered duties covering who may be told about a debt, when a borrower may be called, what must be recorded, and what may not be said. This paper sets out the full rule set that governs a collections conversation in India, identifies the provisions that can be tested from a transcript, and records what the rules do not cover. It also records the position in the United States and the United Kingdom, where the equivalent rules are older and more detailed, and identifies which of those rules a vendor may wish to be tested against even though no Indian rule yet requires it.

The purpose is to give anyone building or buying an automated collections agent a single cited reference for what the agent has to get right, and a clear record of where the law is silent.

---

## Contents

1. Introduction
2. The two regulatory regimes
   2.1 What is in force today
   2.2 What takes effect on 1 January 2027
   2.3 Which instrument applies to which lender
3. The new recovery section in detail
   3.1 How it is organised
   3.2 The provisions that govern what is said on a call
   3.3 Provisions outside the scope of this work
4. What the rules do not say
5. Contact hours
6. Other Indian law that bears on a collections call
   6.1 Consumer protection
   6.2 Criminal provisions
   6.3 Security enforcement
   6.4 Credit bureau reporting
   6.5 Data protection
   6.6 Telecom rules
7. Rules that address automated systems
8. Comparable rules in other jurisdictions
   8.1 United States
   8.2 United Kingdom
   8.3 Which of these are worth adopting voluntarily
9. The enforcement record
10. Verification status and open items
11. References

---

## 1. Introduction

A loan collections call is one of the most heavily regulated conversations in Indian financial services, and one of the least documented. The rules governing it are spread across banking regulation, consumer law, criminal law, telecom regulation and self-regulatory codes. Until recently they were written as general standards: do not harass, do not call at odd hours, do not make misleading statements. From 1 January 2027 they become specific.

That change matters for anyone deploying an automated voice agent into collections, because specific rules can be tested and general standards cannot. A rule that says "do not harass" gives an engineer nothing to build against. A rule that says dues may be discussed only with the borrower or the guarantor, that calls may be placed only between eight in the morning and seven in the evening, and that every recovery communication must carry the grievance officer's name, email, telephone number and address, gives an engineer a specification.

This paper collects those rules. Section 2 sets out the two regimes. Section 3 goes through the new recovery provisions clause by clause. Section 4 records what the rules do not cover, which is as important as what they do, because an eval that scores an agent against a rule that does not exist is worse than no eval. Sections 5 and 6 cover contact hours and the other bodies of Indian law that reach a collections conversation. Section 7 covers the rules that address automated systems specifically. Section 8 looks at the United States and the United Kingdom, where collections conduct has been regulated for decades and where several rules have no Indian equivalent. Section 9 records what has actually been penalised. Section 10 states plainly what has and has not been verified from primary sources.

A note on method. Reserve Bank of India documents are served through a viewer that truncates long instruments, and its document store returns a verification page to automated retrieval. Everything in this paper carries a verification marker. Paragraph numbers, dates and reference numbers were read from the primary pages. Wording is close paraphrase unless marked otherwise. Before any clause is relied on in a published result, it should be lifted from the official PDF by hand. Paragraph coordinates are given throughout so that is a mechanical task rather than a search.

---

## 2. The two regulatory regimes

### 2.1 What is in force today

The Responsible Business Conduct Directions, 2025, dated 28 November 2025, consolidated the earlier Fair Practices Codes and the recovery agents circular of 12 August 2022 into a single instrument per class of lender. Recovery conduct under these Directions is written as a list of prohibited behaviours: intimidation or harassment, whether verbal or physical; acts intended to humiliate publicly or intrude on the privacy of a borrower's family members, referees and friends; inappropriate messages by telephone or social media; threatening or anonymous calls; persistently calling the borrower; calling before eight in the morning or after seven in the evening; and false or misleading representations.

This is the standard that applies until 31 December 2026.

### 2.2 What takes effect on 1 January 2027

On 6 August 2026 the Reserve Bank issued amendment Directions to each class of lender. They delete the existing recovery paragraphs and insert a new recovery section in their place. The commercial bank version runs to twenty-nine paragraphs. It covers the lender's recovery policy, the engagement and vetting of recovery agencies, disclosure of which agencies are engaged, fair treatment during recovery, possession of security, technology-based recovery, monitoring, the conduct of employees and agents, complaints, and compliance with other regulators.

The provisions that bear on a telephone conversation are set out in section 3.2 below.

### 2.3 Which instrument applies to which lender

Nine parallel instruments were issued, all dated 6 August 2026 and all effective 1 January 2027.

| Lender class | Reference | New section |
|---|---|---|
| Commercial banks | RBI/2026-27/223 | Section L, paragraphs 454A to 454AB |
| Non-banking financial companies | RBI/2026-27/230 | Section J, paragraphs 100A to 100AB |
| Local area banks | RBI/2026-27/225 | Section H, paragraphs 235A to 235AB |
| Rural cooperative banks | RBI/2026-2027/228 | Paragraphs 378A to 378AB |
| Housing finance companies | RBI/2026-2027/231 | Paragraph 170A, applying the NBFC paragraphs |
| Small finance banks, regional rural banks, urban cooperative banks, all India financial institutions | Issued 6 August 2026 | Equivalent sections |

The commercial bank numbering is used throughout this paper because it is the series that has been enumerated. Most Indian collections volume sits with non-banking financial companies rather than with banks, so for most deployments the operative instrument is the 100-series. Enumerating that series is the first open item in section 10.

---

## 3. The new recovery section in detail

### 3.1 How it is organised

| Sub-section | Paragraphs | Subject |
|---|---|---|
| Preamble | 454A to 454C | Scope, savings, definitions |
| L.1 | 454D to 454G | The lender's recovery policy |
| L.2 | 454H to 454J | Engaging recovery agencies |
| L.3.1 | 454K to 454N | Disclosing which agencies are engaged |
| L.3.2 | 454O to 454Q | Fair treatment during recovery |
| L.3.3 | 454R | Taking possession of security |
| L.3.4 | 454S to 454U | Technology-based recovery |
| L.3.5 | 454V to 454W | Review and monitoring |
| L.4 | 454X to 454Z | Conduct of employees and agents |
| L.5 | 454AA | Complaints |
| L.6 | 454AB | Compliance with other regulations |

### 3.2 The provisions that govern what is said on a call

Eight paragraphs can be tested from a transcript.

**Paragraph 454O.** Borrower information disclosed to employees and agencies is limited to what recovery duties require. The lender must put mitigants in place against misuse, including penal provisions.

**Paragraph 454P.** The lender must document the time and number of every recovery call, and record the content of calls made by an employee or agent to the borrower or guarantor, as well as inbound calls to the number the lender provided. Records are kept for six months, or until disposal where a matter is sub judice. Reasonable precautions are required, including informing the borrower that the conversation is being recorded.

**Paragraph 454Q.** Recovery targets and incentive structures, both for employees and in agency contracts, must not encourage the practices listed in 454Z. This is a useful provision for anyone designing an agent, because it reaches the objective the agent is optimised toward, not only the words it produces. A system prompt or a reward signal that rewards collection without a counterweight is the direct analogue of an incentive structure that encourages harsh practice, and the clause gives a reason to design the counterweight in from the start.

**Paragraph 454X.** Employees and agents display identity cards on visits. Agents additionally carry an authorisation letter and a copy of the notice required by 454L. Both documents must show the agency's telephone number and the lender's grievance officer contact.

**Paragraph 454Y.** Nine sub-clauses govern conduct.

1. Dues are discussed only with the borrower or the guarantor.
2. Interaction is civil, with decency and decorum.
3. Only authorised representatives may visit.
4. Contact or visits take place only between eight in the morning and seven in the evening. Contact outside those hours requires the borrower's express request. A borrower's request to avoid particular times is honoured in normal circumstances.
5. Contact takes place at the borrower's chosen place. If no place is specified, or the borrower fails to appear there on two or more successive occasions, the agent may go to the residence or place of business.
6. Contact is avoided on inappropriate occasions, including bereavement, medical emergencies, other calamities and marriage functions.
7. For microfinance loans, collection takes place at a mutually agreed central place.
8. Written communications require prior approval and must show the sender's name and contact details.
9. A prompt receipt is given for any collection.

**Paragraph 454Z.** Eight practices are deemed harsh.

1. Minatory or abusive language.
2. Posting recordings or personal details of the borrower or guarantor on social media.
3. Inappropriate messages by telephone or social media.
4. Excessive calls or messages, and contact outside the prescribed hours.
5. Threatening or anonymous calls.
6. Intimidating or harassing the borrower, or their relatives, referees, friends or co-workers, including public humiliation or intrusion on privacy.
7. Violence or threatened violence against the borrower, their family, their assets or their reputation.
8. False or misleading statements, particularly about the amount of the debt or the consequences of non-payment.

**Paragraph 454AA.** The lender must run a dedicated grievance mechanism for recovery. Its details go in the loan agreement and in the agency notice. Every recovery communication must carry the grievance officer's name, email address, telephone number and address.

**Paragraph 454AB.** The lender must comply with other Reserve Bank instructions and with other authorities' rules, expressly including the telecom regulator's commercial communications regulations. This paragraph is the bridge between the banking rules and the telecom rules, and it means a lender cannot treat the two as separate compliance tracks.

### 3.3 Provisions outside the scope of this work

Paragraphs 454S to 454U govern technology-based recovery, meaning the remote restriction of a device the lender financed. They set out that no restriction may apply before thirty days past due, that full restriction may apply only after sixty days, that outgoing calls may not be restricted before sixty days, that incoming calls, messages and emergency calls may never be restricted, that restriction must be reversed within one hour of repayment, that compensation of two hundred and fifty rupees per hour applies to delays attributable to the lender up to the amount disbursed, and that neither the lender nor a third-party provider may access contacts, messages, call logs, photographs or location data for recovery or for any other purpose.

These are important rules but they do not govern a conversation, so they are recorded here and not tested.

---

## 4. What the rules do not say

Each of the following was looked for and not found. They are recorded because an evaluation set that scores an agent against a rule that does not exist is not a compliance test, and because several of them are genuinely open questions rather than oversights.

**There is no numeric limit on how often a borrower may be called.** The word used in 454Z(4) is "excessive", and it is not defined. The only quantities anywhere in the section are "two or more successive occasions" in the place rules and the eight to seven window. Call frequency therefore has to be assessed from the conversation rather than from a call log.

**Nothing is prescribed about what must be said at the start of a call.** The identification duty in 454X is about displaying an identity card and carrying an authorisation letter. Those are provisions about in-person visits and written communications. No Indian rule requires an agent to identify itself orally at the start of a telephone call.

**No Indian rule requires a caller to disclose that it is an automated system.** This is dealt with in section 7.

**There is no general right for a borrower to require contact to stop.** Only requests about time of day must be honoured, and only in normal circumstances.

**Disputed debts are not addressed.** A keyword search of the whole instrument for "dispute", "disputed" and "pending" returns only the phrase "sub judice" in paragraph 454P. A draft of these Directions circulated in February and May 2026 reportedly barred a lender from referring a case to an agency while the borrower's grievance about the dues was pending. That provision is absent from the final text.

**The term "vulnerable" is not used.** The only protection is occasion-based, in 454Y(6), together with the financial distress framework in the policy paragraph 454D.

**The language of communication is not addressed at all.** Nothing in the section requires an agent to speak a language the borrower understands, or sets any quality standard for doing so.

**No provision bars an accurate statement about a lawful remedy.** The prohibition in 454Z(8) is on falsity and on misleading representation. A statement that the lender may initiate proceedings, where that is true and the lender intends it, is not prohibited by anything in the Indian recovery rules. This matters for anyone writing test cases, because a case that marks any mention of legal process as a breach would be wrong.

**There is no regulated-person status for an automated agent.** Every instrument binds the lender. Agents are bound indirectly, through the code of conduct the lender is required to impose on them. For an automated system there is no direct regulatory hook at all, which means the breach is always the lender's breach.

**The agent certification requirement does not contemplate software.** Paragraph 454I requires agents to hold a Debt Recovery Agents certificate from the Indian Institute of Banking and Finance, or from an institute with a tie-up arrangement. The requirement is framed around a certified individual. Nothing has been published on how it applies to an automated caller. This is an open question worth raising with a regulator, not a rule to score against.

**Nothing in Indian law regulates what a lender may tell a borrower about credit bureau consequences.** The constraint is indirect, through the general prohibition on misleading statements. Where the law is silent in this way, a test suite is the only available control.

---

## 5. Contact hours

Two windows apply, and they are keyed to the product rather than to the lender.

| Product | Window | Source |
|---|---|---|
| Ordinary loans | 08:00 to 19:00 | Paragraph 454Y(4); recovery agents circular of 12 August 2022; NBFC paragraph 100 |
| Microfinance loans | 09:00 to 18:00 | Microfinance Directions 2022, paragraph 7.4.3(2); NBFC paragraph 91 |

Any system that applies a single window to all products is wrong for one of them.

There is a possible divergence from 1 January 2027 that should be settled before a result is published. Paragraph 454Y(4) sets a single eight to seven window for banks, and 454Y(7) gives microfinance a rule about place but not a different rule about time, whereas the non-banking company microfinance regime retains nine to six. Whether the bank microfinance window changes on 1 January 2027 has not been verified.

---

## 6. Other Indian law that bears on a collections call

### 6.1 Consumer protection

The Consumer Protection Act 2019 contains the single most useful provision found in this research for third-party disclosure, and it is in force now.

Section 2(47)(ix) makes it an unfair trade practice to disclose to any other person any personal information given in confidence by the consumer, unless the disclosure is made in accordance with law. A lender's agent telling a borrower's spouse, employer or neighbour about a debt engages this provision directly, and the borrower can act on it in a consumer commission without waiting for the 2027 banking rules or the 2027 data protection rules.

Section 2(11) defines deficiency to include any fault in the manner of performance "required to be maintained by or under any law". That phrase is the bridge that turns a breach of the Reserve Bank's recovery rules into a claim the borrower can bring themselves. It is best used as the reasoning behind a score rather than as a test in its own right.

Section 2(47)(i) covers misleading statements made in the provision of a service. The opening words of section 2(47) refer to promoting the sale of goods or services, which is a limitation worth noting, since a collections call promotes nothing. The argument runs through the service relationship instead.

Section 2(28), on misleading advertisements, is a weak fit for a one-to-one telephone call and should not carry any core test case.

### 6.2 Criminal provisions

The Bharatiya Nyaya Sanhita 2023 replaced the Indian Penal Code with effect from 1 July 2024. The relevant provisions form a natural severity scale.

| Conduct | Section | Former section | Maximum |
|---|---|---|---|
| Intentional insult intended to provoke a breach of peace | 352 | 504 | 2 years |
| Criminal intimidation | 351(1) and (2) | 503, 506 | 2 years |
| Criminal intimidation with threat of death or grievous hurt | 351(3) |  - | 7 years |
| Criminal intimidation by anonymous communication | 351(4) | 507 | Additional 2 years |
| Defamation | 356(1) and (2) | 499, 500 | 2 years |
| Extortion | 308(1) and (2) | 383 to 389 | 7 years |
| Extortion by putting in fear of death or grievous hurt | 308(5) |  - | 10 years |

Section 66D of the Information Technology Act 2000 is the provision that fits an automated caller most closely. It reads: "Whoever, by means for any communication device or computer resource cheats by personating, shall be punished with imprisonment of either description for a term which may extend to three years and shall also be liable to fine which may extend to one lakh rupees."

An automated voice agent on a telephone line is using both a communication device and a computer resource. If it represents itself as a police officer, a court, or a law firm in order to obtain payment, section 66D applies, and its ceiling is higher than either the insult or the defamation provision.

The useful structure here is the gradient. Section 352 covers rudeness. Section 351 covers a threat. Section 308 covers a threat used as a lever to obtain money. That maps naturally onto severity weighting in an evaluation rubric.

### 6.3 Security enforcement

The SARFAESI Act 2002 governs enforcement of security interests. One fact about it determines a whole family of test cases: it does not apply to unsecured debt at all. For a personal loan, a credit card or an unsecured microfinance loan, any statement invoking it is false. Section 31 also excludes amounts below one lakh rupees and agricultural land.

Where it does apply, the sequence is: a written demand notice giving sixty days to discharge the liability, under section 13(2); a right for the borrower to make a representation, which the creditor must consider and respond to with reasons within fifteen days, under section 13(3A); possession only after the sixty days expire, under section 13(4); an application to the District Magistrate for assistance with physical possession, under section 14; thirty days' notice before sale, under Rule 8(6), with public notice in two newspapers, one of them in the local language; no sale before thirty days from that notice, under Rule 9(1); and an application to the Debts Recovery Tribunal within forty-five days, under section 17.

That sequence is the ground truth against which a statement about repossession can be scored as accurate, exaggerated or invented. A statement that the lender will take a house this week, that no notice is required, or that there is no appeal, is false. So is any reference to the Act on an unsecured loan. Forcible seizure by recovery agents has never been authorised by it.

### 6.4 Credit bureau reporting

What is true, and therefore what an accurate statement looks like:

Reporting is fortnightly, as on the fifteenth and the last day of each month, submitted within seven calendar days. This is paragraph 6(1)(b) of the Credit Information Reporting Directions, 2025. A statement that a borrower's credit record will be damaged today, or within the hour, is false on timing.

The borrower is entitled to an alert by message or email when a default or days-past-due figure is reported, under paragraph 16(1)(b).

Correction requires the lender's certification, under section 21 of the Credit Information Companies (Regulation) Act 2005, within thirty days under section 21(3). A credit information company cannot change a record on its own. Complaint resolution takes thirty days, after which the complainant is entitled to one hundred rupees per day.

A credit report displays thirty-six months of payment history. That is a display window, not a retention period.

Paying does not erase history. A statement that paying today will make a credit record clean is false. A statement that paying will stop further default reporting and update the account status is accurate.

Two things should not be asserted in any scoring key. There is no statutory retention period anywhere in the Act, the rules or the Reserve Bank directions. The commonly repeated figure of seven years could not be traced to any statute or direction, so a statement about how long a record lasts should be scored as unverifiable rather than as false. And the distinction between "settled", "closed" and "written off" is not defined in any of these instruments. They are distinct status codes in the uniform reporting format, but the format annexe was not reached, so no scoring key should turn on them yet.

### 6.5 Data protection

The Digital Personal Data Protection Act 2023 and its Rules were notified on 13 November 2025, and commence in three stages.

| Stage | Date | What begins |
|---|---|---|
| First | 13 November 2025 | Board constitution and related provisions |
| Second | 13 November 2026 | Consent manager registration |
| Third | 13 May 2027 | Notice, security, breach reporting, retention, and the rights of individuals |

The substantive obligations therefore begin on 13 May 2027. A consent or notice test written today measures compliance with something that is not yet binding, and should be labelled as such.

Three points matter for an automated agent.

The lender is the data fiduciary, because it determines the purpose and means of processing. A voice agent vendor is a data processor, unless it determines its own purposes, for example by keeping call audio to improve models used for other clients, in which case it becomes a fiduciary for that purpose. Section 8(1) requires the fiduciary to bind the processor by contract, and all obligations remain with the fiduciary. There is no contracting out.

Call recordings are personal data. The Act has no special category for sensitive data at all, so no test case should assume one.

India has no legitimate interest ground equivalent to the one in European law. Collections processing rests on consent obtained at the time of onboarding.

The third party who answers a borrower's telephone is an individual in their own right under the Act. Processing their data requires consent or one of the listed lawful uses, and neither applies. The listed use covering data a person voluntarily provided does not help, because the third party volunteered nothing. No provision addresses incidental third-party data on a call. This is a gap in the law rather than a settled rule, and it should be presented that way, but it does mean a case about disclosure to a third party has a data protection argument as well as a banking one.

The Act contains no provision on automated decision-making and no right to human review. There is no equivalent to Article 22 of the European regulation. The only algorithmic provision anywhere in the regime binds significant data fiduciaries, applies from 13 May 2027, and constrains nothing an agent says.

### 6.6 Telecom rules

Three points, two of which correct a common assumption.

A collections call is not a "specified message" under section 28 of the Telecommunications Act 2023, because it offers, advertises and promotes nothing. The Do Not Disturb machinery therefore does not apply to it.

A collections call is a commercial communication under the telecom regulator's 2018 regulations, but it is carved out of unsolicited commercial communication as a service communication. It escapes preference scrubbing, but it remains inside the header, template, registration and numbering requirements.

The 2025 amendment to those regulations requires that "Every Sender shall notify the Originating Access Provider, in advance, about the use of Auto Dialer or Robo-Calls as well as the intended objective of such calls in writing." This is a disclosure to the telecom operator. It creates no obligation to tell the borrower anything, and should not be cited as if it did.

Two further points are worth knowing even though they are not conversational tests. The same amendment provides that implied consent for service communications lasts only for the duration of the contract, so once a loan contract ends, service calls need explicit consent. And the regulations set thresholds for abandoned calls above three per cent and silent calls above one per cent of attempts over twenty-four hours. Those thresholds were written for predictive dialling systems. An automated voice agent with latency or interruption-handling problems can produce the same silent-call condition, which is a real compliance exposure that nobody appears to be measuring.

Separately, a Reserve Bank circular of 17 January 2025 requires regulated entities to place transactional and service calls on the 1600 number series and promotional calls on the 1400 series, with registered headers and templates. A call placed from the wrong series is non-compliant before a word is spoken. That is a telephony configuration matter rather than a conversational one, and belongs in a separate check.

Calling name presentation became mandatory on fourth-generation and later mobile networks on 1 November 2026. Enterprise connections may display a preferred name only where it matches a registered trademark or a trade name registered for tax purposes. The practical effect is that a borrower's handset shows a network-verified name before the agent speaks, so an agent that then names a different entity is contradicting verified information.

---

## 7. Rules that address automated systems

Nothing binding in Indian, United States or United Kingdom law requires a caller to tell the person on the other end that they are speaking to an automated system. This was checked in all three jurisdictions.

The position is summarised below.

| Instrument | Status | What it says |
|---|---|---|
| FACE Guidelines on Debt Recovery, version 1.1, 19 August 2025 | Self-regulatory organisation recognised by the Reserve Bank; binds non-banking financial companies, lending service providers and collection technology firms | Automated agents must identify themselves and state that the communication is automated. Human oversight is required for escalations and critical decisions. Quarterly board review must cover escalations from automated systems. Borrower data may not be used to train models without explicit consent. Daily limits apply to calls and messages. Language must remain appropriate even where the borrower's is not |
| FREE-AI Committee Report, 13 August 2025 | Committee report, not binding | Recommendation 18 on consumer protection, with operative text at paragraph 4.4.54: customers are to be informed explicitly when interacting with an automated system, may choose a human representative, and firms may not falsely claim to use such systems. Recommendation 16 covers human oversight. Recommendation 8 proposes a liability framework. Paragraph 4.4.49 states that regulated entities remain liable for the actions and outcomes of autonomous systems they deploy |
| Draft Guidance on Model Risk Management, 2026 | Draft; consultation closed 24 July 2026 | Customer-facing systems must tell users they are interacting with an automated system and inform them of its limitations, and users must be able to switch to human assistance. A customer-facing interface cannot be a dead end. Red-teaming is expected for customer-facing and generative systems. For third-party models, the regulated entity remains fully accountable, vendor certifications do not transfer accountability, and the entity must perform its own independent validation |
| Information Technology Amendment Rules 2026, in force 20 February 2026 | Binding | Synthetically generated audio must carry a prominently prefixed audio disclosure. The rules bind intermediaries. A lender placing an outbound call is not an intermediary, so the application is arguable and untested |
| United States Regulation F | Binding | Contains nothing on automated agents, synthetic voice or disclosure |
| United Kingdom Financial Conduct Authority, October 2026 | Good practice, not a rule | Telling consumers they are using an automated tool is good practice. Being unclear about whether an automated system or a person acted is identified as a practice that can mislead consumers. Obligations under the consumer duty extend to every outcome delivered through such systems |

Two observations follow.

The only body that has written an explicit self-identification rule for debt collection is an Indian self-regulatory organisation. That is ahead of the Reserve Bank, and ahead of both the United States and United Kingdom regulators.

The better way to frame the obligation is the one the United Kingdom regulator uses. The concern is not the absence of a disclosure for its own sake. It is the misleading impression created when a borrower believes they are speaking to a person. That formulation explains why it matters, which a bare disclosure requirement does not.

---

## 8. Comparable rules in other jurisdictions

### 8.1 United States

Regulation F, which implements the Fair Debt Collection Practices Act, has governed collections conversations since November 2021 and is the most detailed rulebook of its kind anywhere.

Three features are worth recording.

Calling hours are presumptive, not a safe harbour. Absent knowledge to the contrary, before eight in the morning or after nine at night in the consumer's local time is inconvenient. A call at two in the afternoon is still unlawful if the collector knows or should know that time is inconvenient.

Call frequency is governed by two rebuttable presumptions rather than a cap. A collector is presumed to comply if it places no more than seven calls in seven consecutive days and does not call within seven days of a conversation. Exceeding either is presumed to violate the rule. Both presumptions can be rebutted. The supervisory record includes a case where a collector stayed inside the compliance presumption and examiners found the presumption overcome because the calls followed a request to stop. The general proposition, which transfers, is that a formally compliant call count can still be a breach on the evidence of the conversation.

A cease-communication request does not mean total silence. Three further communications remain permitted: a notice that collection efforts are being terminated, a notice that the creditor may invoke remedies it ordinarily invokes, and a notice that it intends to invoke a specified remedy. Any rule set that treats every post-request utterance as a breach would be wrong.

One rule runs the opposite way to India's. For the purposes of the third-party restriction, the United States rule treats the consumer's spouse as the consumer. Talking to a spouse about a debt is not a breach there. Under Indian paragraph 454Y(1) it is. The United States rule is looser and should not be imported.

### 8.2 United Kingdom

The Financial Conduct Authority's consumer credit rules take the opposite drafting approach: a small number of outcome-framed rules supported by worked examples. Several have no Indian equivalent and are directly relevant to a conversation.

Rule 7.9.1 requires that anyone contacting a customer on a firm's behalf tells the customer who they work for, their role or relationship with the firm, and the purpose of the contact. This is a rule, not guidance, it is about contacting rather than visiting, and it binds the firm for what its agents say.

Rule 7.9.10 requires a firm to establish by suitable means that the individual it is speaking to is the borrower, before disclosing details of the debt. This is a verification duty expressed as a precondition. It is stronger than either the United States rule, which prohibits disclosure but requires no verification step, or the Indian rule, which restricts who may be spoken to but does not require identity to be established first.

Rule 7.14.1 requires a firm to suspend recovery where a customer disputes a debt on valid or possibly valid grounds. Guidance 7.14.2 names three such grounds: the person pursued is not the borrower, the debt does not exist, or the amount is wrong. Rule 7.14.4 places the burden of establishing identity or amount on the firm, not the customer. A borrower saying "this is not my loan" or "that amount is wrong" on a call therefore triggers an immediate duty, which is well suited to a voice agent. The United States equivalent requires a written dispute within a thirty-day window and is of little use for a telephone conversation.

Rule 7.14.9 requires a firm that rejects a repayment proposal to explain the reason clearly. Rule 7.14.10 prohibits conduct intended or likely to intimidate a customer into increasing an offer, and guidance 7.14.11 names two examples: threatening a field visit, and imposing or threatening a substantial charge. Guidance 7.14.13 protects the legitimate move, stating that making a counter-offer is not in itself a breach, and that a customer should be given reasonable time to consider one. Taken together these are the only properly specified rules on negotiation conduct in any of the three jurisdictions.

Rule 7.3.10 prohibits pressuring a customer to repay in one or very few instalments, in unreasonably large amounts, within an unreasonably short time, or by selling property or borrowing. Rule 7.3.5B requires a firm to take all reasonable steps to ensure an agreed arrangement is sustainable, and guidance 7.3.5C explains that an arrangement is unlikely to be sustainable if it prevents the customer meeting priority debts and essential living costs.

Rule 7.3.18 prohibits threatening court action in order to pressure a customer into paying more than they can reasonably afford. This is a purposive prohibition: it reaches a true statement about a lawful remedy deployed for an improper purpose. It provides the category between accurate and false, which is where many real collections statements sit, and which no Indian rule expresses.

Rule 7.10.1 requires a firm to suspend recovery where it has been notified that a customer may lack capacity, or where it understands or ought reasonably to be aware that the customer lacks capacity. The second limb makes this a detection duty rather than a notification duty.

Rule 7.12.2(4) prohibits contacting a customer directly where someone is acting for them, absent an objectively justifiable reason.

One piece of guidance is worth recording as a criticism of this entire approach rather than as a rule. Guidance 7.2.5 states that a firm's review of its arrears policies should not assess individual customer interactions in isolation. That is the most credible objection to any per-conversation evaluation, and it comes from a regulator rather than from a competitor.

### 8.3 Which of these are worth adopting voluntarily

For an Indian lender or vendor, none of the rules in section 8.2 is binding. Several are worth meeting anyway, for three reasons: they describe conduct a bank's own legal team will ask about in a procurement review; they are where Indian regulation has been heading, as the move from general standards to numbered duties on 1 January 2027 shows; and a vendor selling to a bank with international operations will meet them eventually.

The ones that carry the most weight for the least effort are identity verification before disclosure, three-element self-identification at the start of a call, suspension on a disputed debt, and a reasoned explanation when a repayment proposal is refused. Each is cheap to implement and each is visible in a transcript.

---

## 9. The enforcement record

Six monetary penalties on recovery conduct are on the public record.

| Institution | Date | Amount | Stated basis |
|---|---|---|---|
| RBL Bank | March 2023 | 2.27 crore rupees | Agents resorted to intimidation and harassment; agents onboarded without the required certificate; no pre-employment verification; borrowers not informed of the agency's details |
| Bajaj Finance | January 2021 | 2.50 crore rupees | Harassment or intimidation of customers; persistent complaints about recovery methods |
| HDFC Bank | September 2024 | 1 crore rupees | Among three sustained charges, failure to ensure customers were not contacted between seven at night and seven in the morning |
| Axis Bank | November 2023 | 90.92 lakh rupees | Persistent calls; agent conduct; calls to certain customers not recorded |
| Krazybee Services | February 2023 | 42.48 lakh rupees | Harassment or intimidation in debt collection |
| Navi Finserv | February 2026 | 3.80 lakh rupees | Contacting borrowers after seven at night and before eight in the morning |

One non-monetary action is worth noting. In September 2022 the Reserve Bank directed a non-banking financial company to cease all recovery and repossession through outsourcing arrangements, citing supervisory concerns about its outsourcing of recovery.

Two qualifications belong with this table.

Penalties for recovery conduct are rare. Across roughly one hundred and forty recent enforcement actions, only about two concern recovery calling conduct. Most penalties relate to know-your-customer requirements, exposure norms and disclosure.

The Ombudsman's annual reports do not break out a complaint ground for recovery conduct. Loans and advances is the largest category at 29.25 per cent of complaints handled at the Ombudsman offices and 68.65 per cent of all complaints against non-banking financial companies, but it is not broken down further. There is no published Indian figure for the number of complaints about recovery conduct, and any such figure seen elsewhere is derived rather than published.

### 9.1 Why the court record is thin, and what follows from it

Two recent cases on recovery agent conduct both failed, and both failed for the same reason.

In a Delhi district court matter decided on 10 February 2025, a borrower alleged that a bank sent four recovery agents to his home and office and that they threatened him and his wife. The claim was dismissed. The court found the account difficult to accept because no police complaint had been filed, no neighbour or employee was called as a witness, and the agents' identification had never been checked. The court also held that an injunction restraining harassment is incapable of enforcement and cannot be granted.

In a Bangalore city civil court matter decided on 16 February 2017, a borrower alleged that agents pressured him by telephone and at home, used abusive language, and said they would have him jailed. The claim was dismissed because his cross-examination was never completed and his evidence was discarded.

The judicial record on collections speech is almost empty, and the reason is evidentiary rather than behavioural. There is no recording, no witness, and no identified agent. Oral conduct on a telephone call is nearly impossible to prove.

An automated agent changes that. It produces a complete, timestamped, attributable record of every call, which is why paragraph 454P's recording requirement is less of a burden for an automated system than for a human workforce. It also means that a lender deploying one can demonstrate what was said, rather than being unable to rebut an allegation. That is an argument in favour of automation, properly tested, rather than against it.

### 9.2 Which liability authority to rely on

For the proposition that an operator is answerable for what its agent says, the clearest authority is a 2024 decision of a Canadian tribunal, which rejected the argument that an automated assistant was a separate legal entity responsible for its own statements.

In India, the 2008 Supreme Court decision in the ICICI Bank matter states that banks are responsible for their agents' conduct and that seizure may be effected only by legal means. Its citation is reported inconsistently in secondary sources and should be checked before use.

The 2007 Supreme Court decision in the Prakash Kaur matter is frequently cited for vicarious liability. It does not hold that. The passage usually quoted is from a supplementary opinion, and the majority expressly did not decide the question.

---

## 10. Verification status and open items

Everything in this paper is marked according to how it was obtained.

Paragraph numbers, dates, reference numbers, hours, day counts and monetary figures were read from primary pages. Wording is close paraphrase. The only quoted text is the Information Technology Act provision in section 6.2, the telecom auto-dialler provision in section 6.6, and the data protection commencement rule.

Three technical obstacles explain this. Direct requests to the Reserve Bank website are refused by the network this research ran on. Its document store returns a verification page to automated retrieval. The reader used applies a limit on quotation length and declines full reproduction. The United States electronic code of federal regulations and the government publishing office both declined reproduction under their own quoting limits.

Open items, in order of value.

1. Enumerate the non-banking financial company paragraphs 100A to 100AB. Most Indian collections volume is non-banking, and the present paper is keyed to the bank series.
2. Lift Section L, paragraphs 454A to 454AB, verbatim from the official document.
3. Obtain Chapter VIII, paragraphs 408 to 416 and 442 to 454, of the 2025 Directions. These are the pre-2027 bank standard and could not be reached by any route. Chapter VIII sits roughly four fifths of the way through a document of about four hundred and fifty paragraphs.
4. Confirm whether the recovery agents circular of 12 August 2022 appears in the annexe to the withdrawal circular of 28 November 2025. That circular withdrew 9,445 instruments with immediate effect, but the annexe listing them could not be reached. The inference that the 2022 circular is among them is strong but unverified.
5. Settle whether the microfinance contact window changes for banks on 1 January 2027.
6. Obtain the reference number and the compliance deadline year for the circular of 17 January 2025.
7. Obtain the uniform credit reporting format annexe, needed before any scoring of statements about settled and closed account statuses.
8. Obtain the United Kingdom rules at CONC 7.5, 7.4, 7.6, 7.11, 7.13 and 2.10, and the consumer duty provisions. The handbook is rendered dynamically and succeeded roughly one fetch in three. Rule 7.5, on pursuing and recovering repayments, failed six times and its title suggests it is directly relevant.
9. Obtain consumer complaint narratives from the United States regulator's public database. The taxonomy and volumes in this paper come from its published annual reports; the database itself was not reachable.
10. Read the United States appellate decision on meaningful disclosure of identity, whose holding is reported only in secondary sources.
11. Obtain verbatim text of the United States regulation before publishing any case that turns on exact wording.

---

## 11. References

Reserve Bank of India. Fourth Amendment Directions, 2026. RBI/2026-27/223, 6 August 2026.
https://www.rbi.org.in/scripts/NotificationUser.aspx?Id=13665&Mode=0

Reserve Bank of India. Non-Banking Financial Companies Third Amendment Directions, 2026. RBI/2026-27/230, 6 August 2026.
https://rbi.org.in/scripts/NotificationUser.aspx?Mode=0&Id=13672

Reserve Bank of India. Commercial Banks Responsible Business Conduct Directions, 2025. RBI/DOR/2025-26/170, 28 November 2025.
https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=13140

Reserve Bank of India. Non-Banking Financial Companies Responsible Business Conduct Directions, 2025. RBI/DOR/2025-26/362, 28 November 2025.
https://www.rbi.org.in/scripts/BS_ViewMasDirections.aspx?id=12942

Reserve Bank of India. Outsourcing of Financial Services: Responsibilities of regulated entities employing Recovery Agents. RBI/2022-23/108, 12 August 2022.
https://rbi.org.in/Scripts/NotificationUser.aspx?Id=12378&Mode=0

Reserve Bank of India. Consolidation of Regulations: Withdrawal of circulars. RBI/2025-26/100, 28 November 2025.
https://www.rbi.org.in/scripts/NotificationUser.aspx?Id=13170&Mode=0

Reserve Bank of India. Regulatory Framework for Microfinance Loans Directions, 2022. 14 March 2022.
https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12256

Reserve Bank of India. Digital Lending Directions, 2025. RBI/2025-26/36, 8 May 2025.
https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12848

Reserve Bank of India. Credit Information Reporting Directions, 2025. RBI/DoR/2024-25/125, 6 January 2025.
https://www.rbi.org.in/Scripts/BS_ViewMasDirections.aspx?id=12764

Reserve Bank of India. Framework for Responsible and Ethical Enablement of Artificial Intelligence. Committee report, 13 August 2025.
https://www.rbi.org.in/Scripts/PublicationReportDetails.aspx?ID=1306

Reserve Bank of India. Draft Guidance on Regulatory Principles for Model Risk Management, 2026.
https://www.rbi.org.in/Scripts/bs_viewcontent.aspx?Id=5089

Fintech Association for Consumer Empowerment. Guidelines on Debt Recovery, version 1.1, 29 August 2025.
https://faceofindia.org/wp-content/uploads/2025/08/FACE-Guidelines-on-debt-recovery_29-Aug-2025_website.pdf

Telecom Regulatory Authority of India. Telecom Commercial Communications Customer Preference Regulations, 2018.
https://www.trai.gov.in/sites/default/files/2024-09/RegulationUcc19072018.pdf

Telecom Regulatory Authority of India. Second Amendment Regulations, 2025. 12 February 2025.
https://www.trai.gov.in/sites/default/files/2025-02/Regulation_12022025.pdf

Digital Personal Data Protection Rules, 2025. G.S.R. 846(E), 13 November 2025.
https://www.dpdpa.com/DPDP_Rules_2025_English_only.pdf

Credit Information Companies (Regulation) Act, 2005.
https://prsindia.org/files/bills_acts/acts_parliament/2005/the-credit-information-companies-(regulation)-act-2005.pdf

Telecommunications Act, 2023, section 28.
https://www.advocatekhoj.com/library/bareacts/telecommunications/28.php

Consumer Financial Protection Bureau. 12 CFR Part 1006 (Regulation F).
https://www.ecfr.gov/current/title-12/chapter-X/part-1006

Consumer Financial Protection Bureau. Fair Debt Collection Practices Act Annual Report, November 2025.
https://files.consumerfinance.gov/f/documents/cfpb_fdcpa-2025-annual-report_2025-11.pdf

Financial Conduct Authority. Consumer Credit Sourcebook, CONC 7.
https://handbook.fca.org.uk/handbook/conc7/conc7s9

Reserve Bank of India penalty orders.
RBL Bank: https://rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=55389
Bajaj Finance: https://www.rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=50918
HDFC Bank: https://www.rbi.org.in/scripts/BS_PressReleaseDisplay.aspx?prid=58673
Axis Bank: https://www.rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=56754
Krazybee Services: https://rbi.org.in/Scripts/BS_PressReleaseDisplay.aspx?prid=55160
